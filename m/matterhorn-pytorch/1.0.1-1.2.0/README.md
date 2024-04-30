# Comparing `tmp/matterhorn_pytorch-1.0.1.tar.gz` & `tmp/matterhorn_pytorch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matterhorn_pytorch-1.0.1.tar", last modified: Fri Oct 20 07:52:18 2023, max compression
+gzip compressed data, was "dist/matterhorn_pytorch-1.2.0.tar", last modified: Mon Apr 29 05:05:14 2024, max compression
```

## Comparing `matterhorn_pytorch-1.0.1.tar` & `matterhorn_pytorch-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,77 @@
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.261923 matterhorn_pytorch-1.0.1/
--rw-r--r--   0 amperiawang   (501) staff       (20)      897 2023-08-16 14:32:33.000000 matterhorn_pytorch-1.0.1/LICENSE
--rw-r--r--   0 amperiawang   (501) staff       (20)      197 2023-10-20 07:39:52.000000 matterhorn_pytorch-1.0.1/MANIFEST.in
--rw-r--r--   0 amperiawang   (501) staff       (20)    16622 2023-10-20 07:52:18.261513 matterhorn_pytorch-1.0.1/PKG-INFO
--rw-r--r--   0 amperiawang   (501) staff       (20)    16414 2023-10-20 07:34:51.000000 matterhorn_pytorch-1.0.1/README.md
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.246293 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/
--rw-r--r--   0 amperiawang   (501) staff       (20)      234 2023-10-12 19:17:58.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/api.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)      127 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/base.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)      225 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/base.h
--rw-r--r--   0 amperiawang   (501) staff       (20)    12439 2023-10-19 06:38:02.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/soma.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)     3301 2023-10-18 17:24:50.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/soma.h
--rw-r--r--   0 amperiawang   (501) staff       (20)     2114 2023-10-18 16:36:17.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/stdp.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)      404 2023-10-12 18:49:29.000000 matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/stdp.h
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.249913 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/
--rw-r--r--   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:39:11.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/__init__.py
--rw-r--r--   0 amperiawang   (501) staff       (20)      261 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/api.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)     4329 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/base.cu
--rw-r--r--   0 amperiawang   (501) staff       (20)      225 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/base.h
--rw-r--r--   0 amperiawang   (501) staff       (20)      389 2023-10-12 18:49:29.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/cuda_utils.h
--rw-r--r--   0 amperiawang   (501) staff       (20)      900 2023-10-20 07:45:02.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/setup.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     3835 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/soma.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)     2028 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/soma.h
--rw-r--r--   0 amperiawang   (501) staff       (20)    16987 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/soma_cuda.cu
--rw-r--r--   0 amperiawang   (501) staff       (20)     1413 2023-10-16 12:10:53.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/stdp.cpp
--rw-r--r--   0 amperiawang   (501) staff       (20)      839 2023-10-16 12:10:53.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/stdp.h
--rw-r--r--   0 amperiawang   (501) staff       (20)     3198 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/stdp_cuda.cu
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.250156 matterhorn_pytorch-1.0.1/matterhorn_pytorch/
--rw-r--r--   0 amperiawang   (501) staff       (20)      150 2023-09-07 01:37:24.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/__init__.py
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.253380 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/
--rw-r--r--   0 amperiawang   (501) staff       (20)      254 2023-09-07 01:37:24.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/__init__.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    20742 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/aedat.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     9295 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/hdf5.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     7900 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/nmnist.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    16802 2023-10-03 14:43:11.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/skeleton.py
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.254790 matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/
--rw-r--r--   0 amperiawang   (501) staff       (20)      226 2023-10-04 16:43:46.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/__init__.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    10811 2023-10-20 07:12:51.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/sew.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     4116 2023-10-20 07:12:51.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/ta.py
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.259843 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/
--rw-r--r--   0 amperiawang   (501) staff       (20)      869 2023-10-10 06:36:11.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/__init__.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    10559 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/container.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     4488 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/decoder.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     6816 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/encoder.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    23277 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/layer.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     7619 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/learning.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     2537 2023-10-12 12:22:05.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/skeleton.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    25144 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/soma.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     8883 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/soma_cpp.py
--rw-r--r--   0 amperiawang   (501) staff       (20)     8365 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/soma_cuda.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    10486 2023-10-18 14:30:55.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/surrogate.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    27006 2023-10-20 07:12:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/synapse.py
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.260726 matterhorn_pytorch-1.0.1/matterhorn_pytorch/util/
--rw-r--r--   0 amperiawang   (501) staff       (20)      125 2023-09-04 07:08:01.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/util/__init__.py
--rw-r--r--   0 amperiawang   (501) staff       (20)    15541 2023-10-03 14:18:32.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch/util/plotter.py
-drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2023-10-20 07:52:18.251244 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/
--rw-r--r--   0 amperiawang   (501) staff       (20)    16622 2023-10-20 07:52:18.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 amperiawang   (501) staff       (20)     2032 2023-10-20 07:52:18.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 amperiawang   (501) staff       (20)        1 2023-10-20 07:52:18.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 amperiawang   (501) staff       (20)       56 2023-10-20 07:52:18.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/requires.txt
--rw-r--r--   0 amperiawang   (501) staff       (20)       72 2023-10-20 07:52:18.000000 matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/top_level.txt
--rw-r--r--   0 amperiawang   (501) staff       (20)       38 2023-10-20 07:52:18.262008 matterhorn_pytorch-1.0.1/setup.cfg
--rw-r--r--   0 amperiawang   (501) staff       (20)     3178 2023-10-20 07:51:33.000000 matterhorn_pytorch-1.0.1/setup.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.835989 matterhorn_pytorch-1.2.0/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      897 2023-08-16 14:32:33.000000 matterhorn_pytorch-1.2.0/LICENSE
+-rw-r--r--   0 amperiawang   (501) staff       (20)      197 2023-10-20 07:39:52.000000 matterhorn_pytorch-1.2.0/MANIFEST.in
+-rw-r--r--   0 amperiawang   (501) staff       (20)    16213 2024-04-29 05:05:14.835583 matterhorn_pytorch-1.2.0/PKG-INFO
+-rw-r--r--   0 amperiawang   (501) staff       (20)    15953 2024-04-29 04:59:22.000000 matterhorn_pytorch-1.2.0/README.md
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.809812 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      298 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/api.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)      188 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/base.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)      225 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/base.h
+-rw-r--r--   0 amperiawang   (501) staff       (20)    20694 2024-02-12 15:26:52.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/soma.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)     5154 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/soma.h
+-rw-r--r--   0 amperiawang   (501) staff       (20)     2400 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/stdp.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)      430 2023-12-21 14:16:52.000000 matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/stdp.h
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.813315 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      337 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/api.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)     4558 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/base.cu
+-rw-r--r--   0 amperiawang   (501) staff       (20)      408 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/base.h
+-rw-r--r--   0 amperiawang   (501) staff       (20)      900 2023-10-20 07:45:02.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/setup.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3943 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/soma.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)     2028 2023-10-19 06:34:16.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/soma.h
+-rw-r--r--   0 amperiawang   (501) staff       (20)    16905 2024-02-12 15:26:52.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/soma_cuda.cu
+-rw-r--r--   0 amperiawang   (501) staff       (20)     1556 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/stdp.cpp
+-rw-r--r--   0 amperiawang   (501) staff       (20)      901 2023-12-21 14:16:52.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/stdp.h
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3755 2024-01-04 08:19:50.000000 matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/stdp_cuda.cu
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.813997 matterhorn_pytorch-1.2.0/matterhorn_pytorch/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      959 2024-03-21 16:49:43.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/__func__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)      305 2024-03-21 16:49:43.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/__init__.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.818641 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      254 2023-09-07 01:37:24.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    21381 2024-04-16 07:27:44.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/aedat.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3959 2024-04-16 05:25:57.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/functional.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     9275 2024-04-16 03:53:38.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/hdf5.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     7877 2024-04-16 03:54:06.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/nmnist.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    18717 2024-04-16 07:43:13.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/skeleton.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     1075 2024-04-16 07:32:53.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/transforms.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.820227 matterhorn_pytorch-1.2.0/matterhorn_pytorch/lsm/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      224 2024-03-20 06:27:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/lsm/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     5819 2024-03-20 06:27:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/lsm/functional.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     1657 2024-02-26 07:00:08.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/lsm/io.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    16059 2024-04-12 09:06:50.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/lsm/layer.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.821922 matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      226 2023-10-04 16:43:46.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    10833 2024-02-14 05:41:15.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/sew.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3959 2024-02-14 05:41:15.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/ta.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.827846 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      951 2024-03-23 08:30:40.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     7851 2024-03-29 10:57:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/container.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     6291 2024-03-29 10:57:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/decoder.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     6669 2024-03-29 10:57:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/encoder.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    11666 2024-04-14 10:17:04.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/functional.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    28088 2024-04-12 09:06:50.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/layer.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3749 2024-03-29 16:32:59.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/skeleton.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    31871 2024-04-14 10:14:24.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/soma.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     5056 2024-03-29 15:57:33.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/soma_cpp.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     4570 2024-03-29 15:57:33.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/soma_cuda.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     3483 2024-02-26 07:00:08.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/surrogate.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    28866 2024-03-29 10:57:54.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/synapse.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.829491 matterhorn_pytorch-1.2.0/matterhorn_pytorch/tnn/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      153 2024-02-14 05:41:15.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/tnn/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)      795 2024-01-26 06:17:30.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/tnn/column.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     4619 2024-04-12 08:36:51.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/tnn/component.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    19740 2024-04-16 05:25:00.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/tnn/functional.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.831157 matterhorn_pytorch-1.2.0/matterhorn_pytorch/training/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      159 2024-02-14 05:41:15.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/training/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     9236 2024-03-22 13:38:25.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/training/functional.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.832858 matterhorn_pytorch-1.2.0/matterhorn_pytorch/util/
+-rw-r--r--   0 amperiawang   (501) staff       (20)      151 2024-02-08 16:48:18.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/util/__init__.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)     6771 2024-02-09 06:32:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/util/interpreter.py
+-rw-r--r--   0 amperiawang   (501) staff       (20)    31603 2024-03-01 10:34:56.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch/util/plotter.py
+drwxr-xr-x   0 amperiawang   (501) staff       (20)        0 2024-04-29 05:05:14.815432 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/
+-rw-r--r--   0 amperiawang   (501) staff       (20)    16213 2024-04-29 05:05:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 amperiawang   (501) staff       (20)     2457 2024-04-29 05:05:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 amperiawang   (501) staff       (20)        1 2024-04-29 05:05:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 amperiawang   (501) staff       (20)       60 2024-04-29 05:05:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/requires.txt
+-rw-r--r--   0 amperiawang   (501) staff       (20)       19 2024-04-29 05:05:14.000000 matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 amperiawang   (501) staff       (20)       38 2024-04-29 05:05:14.836076 matterhorn_pytorch-1.2.0/setup.cfg
+-rw-r--r--   0 amperiawang   (501) staff       (20)     4192 2024-04-29 05:04:48.000000 matterhorn_pytorch-1.2.0/setup.py
```

### Comparing `matterhorn_pytorch-1.0.1/LICENSE` & `matterhorn_pytorch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matterhorn_pytorch-1.0.1/PKG-INFO` & `matterhorn_pytorch-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,494 +1,448 @@
-Metadata-Version: 2.1
-Name: matterhorn_pytorch
-Version: 1.0.1
-Summary: Matterhorn is a neo general SNN framework based on PyTorch.
-Home-page: https://github.com/AmperiaWang/Matterhorn
-Author: CAG, IAIR, XJTU, Xi'an, China
-Author-email: ericwang017@stu.xjtu.edu.cn
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: numba
-Requires-Dist: h5py
-Requires-Dist: tqdm
-Requires-Dist: rich
-Requires-Dist: torch
-Requires-Dist: torchvision
-
-# Matterhorn
-
-## 1 General Introduction
-
-![logo](./assets/logo.png)
-
-Matterhorn is a neo general SNN framework based on PyTorch.
-
-## 2 Installation
-
-### Environment
-
-Python(>=3.7.0)
-
-CUDA(>=11.3.0, with CUDNN)
-
-PyTorch(>=1.10.0 and <=1.13.1)
-
-TorchVision(>=0.11.0 and <= 0.13.1)
-
-### Environment Installation
-
-To install PyTorch you can find the command on [https://pytorch.org/get-started/previous-versions/](https://pytorch.org/get-started/previous-versions/).
-
-```sh
-pip install numpy matplotlib numba h5py tqdm rich torch torchvision
-```
-
-### Install Matterhorn
-
-```sh
-git clone https://github.com/AmperiaWang/Matterhorn.git
-cd Matterhorn
-python3 setup.py install
-```
-
-Don't forget to add `sudo` if you are not the root user.
-
-## 3 Module Explanation
-
-### Neurons in SNN
-
-As we're all known, the image below describes what an ANN looks like.
-
-![ANN Structure](./assets/readme_1.png)
-
-**Operation 1** is **synapse function**, which uses weights and bias to calculate those values from previous layer to current layer. Commonly used synapse functions are including full connection layer `nn.Linear`, convolution layer `nn.Conv2D`, etc.
-
-We use an equation to describe the synapse function:
-
-$$Y^{l}=synapse(X^{l-1})$$
-
-Where $l$ here means the number of current layers.
-
-**Operation 2** is **activation function**, which filters information from synapses and sends the filtered information to next layer. Commonly used activation functions are including `nn.ReLU`, `nn.Sigmoid`, etc.
-
-We use an equation to describe the activation function:
-
-$$X^{l}=activation(Y^{l})$$
-
-In conclusion, each of layers in ANN has 2 functions. We can build our ANN model in PyTorch by the code below:
-
-```python
-import torch.nn as nn
-
-model = nn.Sequential(
-    nn.Linear(28 * 28, 10),
-    nn.ReLU()
-)
-```
-
-This is a 1-layer MLP. It can take an image with the size of 28x28 as input and classify it into 10 classes. In this example, two equations of ANN can be represented as below:
-
-$$Y^{l}=W^{l}X^{l-1}+\vec{b}$$
-
-$$X^{l}=ReLU(Y^{l})$$
-
-In SNN, the synapse equation is the same as that in ANN. However, functions in soma are no longer like what is in ANN. In the soma of SNN, there exists a loop in time. The image below describes what an SNN looks like.
-
-![SNN Structure](./assets/readme_2.png)
-
-**Operation 1**, the **synapse function**, calculates spikes from previous layer $O^{l-1}(t)$ thus generates the input potential $X^{l}(t)$.
-
-We use an equation to describe the synapse function:
-
-$$X^{l}(t)=synapse(O^{l-1}(t))$$
-
-By **operation 2**, the input potential, with the history potential, is calculated based on a 1-order differential equation, thus generating the soma potential $U^{l}(t)$. We name it **response function**.
-
-We use an equation to describe the response function:
-
-$$U^{l}(t)=response(H^{l}(t),X^{l}(t))$$
-
-Each spiking neuron model has its unique response differential equation.
-
-For example, in a LIF neuron:
-
-$$\tau \frac{du}{dt}=-(u-u_{rest})+RI$$
-
-Discretizing it into a difference equation, we can get:
-
-$$U^{l}(t)=(1-\frac{1}{\tau})H^{l}(t)+\frac{1}{\tau}u_{rest}+X^{l}(t)$$
-
-**Operation 3** uses Heaviside step function and threshold potential $u_{th}$ to decide whether to generate spikes $O^{l}(t)$. We name it **firing function**.
-
-We use an equation to describe the firing function:
-
-$$O^{l}(t)=spiking(U^{l}(t))$$
-
-Generally, the firing function looks like this.
-
-$$O^{l}(t)=Heaviside(U^{l}(t)-u_{th})$$
-
-Where Heaviside step function returns 1 when input is greater than or equal to 0, returns 0 otherwise.
-
-The aim of **operation 4** is to set refractory time on neurons by output spikes $O^{l}(t)$. We name it **reset function**.
-
-We use an equation to describe reset function:
-
-$$H^{l}(t)=reset(U^{l}(t-1),O^{l}(t-1))$$
-
-Under most occasions we use equation below to reset potential:
-
-$$H^{l}(t)=U^{l}(t-1)[1-O^{l}(t-1)]+u_{rest}O^{l}(t-1)$$
-
-In brief, we use 4 equations to describe SNN neurons. This is what an SNN looks like. The shape of an SNN neuron is like a trumpet. Its synapses transform those spikes from last neuron and pass the input response to soma, in which there is a time loop awaits.
-
-By unfolding SNN neurons on temporal dimension, we can get the spatial-temporal topology network of SNN.
-
-![Spatial-temporal Topology Network of SNN](./assets/readme_3.png)
-
-Like building ANN in PyTorch, we can build our SNN model in Matterhorn by the code below:
-
-```python
-import torch
-import matterhorn_pytorch.snn as snn
-
-snn_model = snn.Temporal(
-    snn.Spatial(
-        snn.Linear(28 * 28, 10),
-        snn.LIF()
-    )
-)
-```
-
-In the code, `Spatial` is one of Matterhorn's containers to represent sequential SNN layers on spatial dimension, and `Temporal` is another Matterhorn's container to repeat calculating potential and spikes on temporal dimension. By using `Spatial` and `Temporal`, an SNN spatial-temporal topology network is built and thus used for training and evaluating.
-
-The built network takes an $n+1$ dimensional `torch.Tensor` as input spike train. It will take the first dimension as time steps, thus calculating through each time step. after that, it will generate a `torch.Tensor` as output spike train, just like what an ANN takes and generates in PyTorch. The only difference, which is also a key point, is that we should encode our information into spike train and decode the output spike train.
-
-### Encoding and Decoding
-
-A spike train is a set of Dirac impulse functions on the axis of time.
-
-$$O(t)=\sum_{t_{i}}δ(t-t_{i})$$
-
-In other words, there will only be 0s and 1s in discrete spike train. Therefore, we can use an $n+1$ dimensional tensor to represent our spike train. For example, if neurons are flattened into a 1-dimensional vector, we can use another dimension to represent time, thus let it be a 2-dimensional matrix to represent the spike train through space and time.
-
-$$
-\begin{matrix}
- & →s \\
-↓t &
-\begin{bmatrix}
-0 & 1 & 1 & 0 & 1 & 0 & 0 & 1 \\
-1 & 0 & 0 & 1 & 0 & 0 & 1 & 1 \\
-1 & 1 & 1 & 1 & 1 & 1 & 0 & 1 \\
-1 & 0 & 1 & 1 & 0 & 1 & 0 & 1 \\
-\end{bmatrix}
-\end{matrix}
-$$
-
-The matrix above shows what a spike train looks like. It has 4 rows, representing 4 time steps. Besides, it has 8 columns, representing 8 output neurons.
-
-To transform our traditional binary information (images, sounds, etc.) into spike train, an encoder is needed. The most commonly used encoder for non-event data is Poisson encoder, which is a kind of rate coding encoder. It sees intensity of a pixel as probability to fire a spike.
-
-You can use Poisson encoder in Matterhorn by the code below:
-
-```python
-import torch
-import matterhorn_pytorch.snn as snn
-
-encoder = snn.PoissonEncoder(
-    time_steps = 32
-)
-```
-
-Then, you can use it by the code below:
-
-```python
-spike_train = encoder(image)
-```
-
-An image with the shape of `[H, W, C]` would be encoded into a spike train with the shape of `[T, H, W, C]`. For example, a MNIST image which shape is `[28, 28]` would be encoded (`T=32`) into a spike train with the shape of `[32, 28, 28]`.
-
-After encoding and processing, the network would generate an output spike train. To get the information, we need to decode. A commonly used decoding method is to count average spikes each output neuron has generated.
-
-$$o_{i}=\frac{1}{T}\sum_{t=1}^{T}{O_{i}^{K}(t)}$$
-
-You can use average decoder in Matterhorn by the code below:
-
-```python
-import torch
-import matterhorn_pytorch.snn as snn
-
-decoder = snn.AvgSpikeDecoder()
-```
-
-It will take first dimension as temporal dimension, and generate statistical results as output. The output can be transported into ANN for further processes.
-
-Matterhorn provides a convenient container `matterhorn.snn.Sequential` to connect all your SNN and ANN models.
-
-```python
-import torch
-import matterhorn_pytorch.snn as snn
-
-model = snn.Sequential(
-    snn.PoissonEncoder(
-        time_steps = time_steps,
-    ),
-    snn.Flatten(),
-    snn.Linear(28 * 28, 10, bias = False),
-    snn.LIF(tau_m = tau, trainable = True),
-    snn.AvgSpikeDecoder()
-)
-```
-
-By now, you have experienced what an SNN looks like and how to build it by Matterhorn. For further experience, you can refer to [examples/2_layer_mlp.py](./examples/2_layer_mlp.py).
-
-```sh
-cd Matterhorn
-python3 examples/2_layer_mlp.py
-```
-
-In most cases, neurons of SNNs can be divided into 1 synapse operation and 3 soma operations. However, there are always some special cases. SRM0 neuron model is one of them, whose response is calculated in each synapse. We can use 5 operations to represent SRM0 neurons, 2 for synapses and 3 for soma:
-
-**Operation 1**: **synapse response function**
-
-$$R_{j}^{l}(t)=(1-\frac{1}{\tau_{m}})R_{j}^{l}(t-1)+O_{j}^{l}(t)$$
-
-**Operation 2**: **synapse function**
-
-$$X_{i}^{l}(t)=\sum_{j}{w_{ij}R_{j}^{l}(t)}$$
-
-**Operation 3**: **response function**
-
-$$U_{i}^{l}(t)=X_{i}^{l}(t)H_{i}^{l}(t)$$
-
-**Operation 4**: **firing function**
-
-$$O_{i}^{l}(t)=Heaviside(U_{i}^{l}(t))$$
-
-**Operation 5**: **reset function**
-
-$$H_{i}^{l}(t)=1-O_{i}^{l}(t-1)$$
-
-With 5 operations resembled we can build a SRM0 neuron. For further experience, you can refer to [examples/2_layer_mlp_with_SRM0.py](./examples/2_layer_mlp_with_SRM0.py).
-
-```sh
-cd Matterhorn
-python3 examples/2_layer_mlp_with_SRM0.py
-```
-
-### Why Should We Need Surrogate Gradient
-
-In spiking neurons, we usually use Heaviside step function $u(t)$ to decide whether to generate a spike:
-
-$$O^{l}(t)=u(U^{l}(t)-u_{th})$$
-
-![Heaviside step function and its derivative, Dirac impulse function](./assets/readme_4.png)
-
-However, Heaviside step function has a derivative that can make everyone headache. Its derivative is Dirac impulse function $\delta (t)$. Dirac impulse function is infinity when x equals to 0, and 0 otherwise. If it is directly used for backpropagation, the gradient must be all damned.
-
-Therefore, some functions must be there to replace Dirac impulse function to join the backpropagation. We call those functions surrogate gradients.
-
-One of the most common surrogate gradients is rectangular function. It is a positive constant when absolute value of x is small enough, and 0 otherwise.
-
-![Use rectangular function as surrogate gradient](./assets/readme_5.png)
-
-Also, functions suitable for surrogate gradient include the derivative of sigmoidal function, Gaussian function, etc.
-
-You can inspect all provided surrogate gradient functions in `matterhorn.snn.surrogate`.
-
-### Learning: BPTT Vs. STDP
-
-Training SNNs could be as easy as training ANNs after gradient problem of Heaviside step function is solved. After we unfold SNNs into a spatial-temporal network, backpropagation through time (BPTT) could be used in SNNs. On spatial dimension, gradients can be propagated through firing function and synapse function, thus neurons of previous layer would receive the gradient; On temporal dimension, the gradient of the next time step can be propagated through firing function and response function, thus soma of previous time would receive the gradient.
-
-![BPTT](./assets/readme_6.png)
-
-Besides BPTT, there is another simple way to train locally in each neuron without supervision, which we call spike-timing-dependent plasticity (STDP). STDP uses precise time differences between input and output spikes to calculate the weight increment.
-
-STDP follows equation below:
-
-$$Δw_{ij}=\sum_{t_{j}}{\sum_{t_{i}}W(t_{i}-t_{j})}$$
-
-where the weight function $W(x)$ is:
-
-$$
-W(x)=
-\left \{
-\begin{aligned}
-A_{+}e^{-\frac{x}{τ_{+}}},x>0 \\\\
-0,x=0 \\\\
--A_{-}e^{\frac{x}{τ_{-}}},x<0
-\end{aligned}
-\right \}.
-$$
-
-![STDP function](./assets/readme_7.png)
-
-By setting parameters $A_{+}$, $τ_{+}$, $A_{-}$ and $τ_{-}$, we can easily train SNNs unsupervised. For further experience, you can refer to [examples/2_layer_mlp_with_stdp.py](./examples/2_layer_mlp_with_stdp.py).
-
-```sh
-cd Matterhorn
-python3 examples/2_layer_mlp_with_stdp.py
-```
-
-**Note:** Please make sure you have installed `matterhorn_cpp_extensions` (or `matterhorn_cuda_extensions` if you have CUDA), otherwise it will be extremely slow.
-
-```sh
-cd matterhorn_cpp_extensions
-python3 setup.py install
-```
-
-if you have CUDA, you can install CUDA version:
-
-```sh
-cd matterhorn_cuda_extensions
-python3 setup.py install
-```
-
-### Neuromorphic Datasets
-
-Matterhorn provides several neuromorphic datasets for training spiking neural networks.
-
-#### NMNIST
-
-We know MNIST. MNIST dataset is for training image classification, consisting of a set of 28x28 pixel grayscale images of handwritten digits (0-9). NMNIST is like MNIST, which is different is that it distorts images and record them into events. The shape of events in NMNIST Dataset is Tx2x34x34.
-
-![NMNIST Dataset](./assets/readme_8.png)
-
-You can use NMNIST dataset in Matterhorn by the code below:
-
-```python
-from matterhorn_pytorch.data import NMNIST
-
-time_steps = 128
-
-train_dataset = NMNIST(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    time_steps = time_steps
-)
-test_dataset = NMNIST(
-    root = "your/data/path",
-    train = False,
-    download = True,
-    time_steps = time_steps
-)
-```
-
-#### CIFAR10-DVS
-
-CIFAR10-DVS dataset records distorted CIFAR-10 image by a DVS camera. The shape of events in CIFAR10-DVS Dataset is Tx2x128x128.
-
-![CIFAR10-DVS Dataset](./assets/readme_9.png)
-
-You can use CIFAR10-DVS Dataset in Matterhorn by the code below:
-
-```python
-from matterhorn_pytorch.data import CIFAR10DVS
-
-time_steps = 128
-
-train_dataset = CIFAR10DVS(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    time_steps = time_steps
-)
-test_dataset = CIFAR10DVS(
-    root = "your/data/path",
-    train = False,
-    download = True,
-    time_steps = time_steps
-)
-```
-
-#### DVS128 Gesture
-
-DVS128 Gesture dataset records gestures from 29 different people under 3 different illuminating conditions by DVS camera. The shape of events in DVS128 Gesture dataset is Tx2x128x128.
-
-![DVS128 Gesture Dataset](./assets/readme_10.png)
-
-You can use DVS128 Gesture dataset in Matterhorn by the code below:
-
-```python
-from matterhorn_pytorch.data import DVS128Gesture
-
-time_steps = 128
-
-train_dataset = DVS128Gesture(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    time_steps = time_steps
-)
-test_dataset = DVS128Gesture(
-    root = "your/data/path",
-    train = False,
-    download = True,
-    time_steps = time_steps
-)
-```
-
-**Warning:** You may have to set parameter `sampling` to save the disk space in your device.
-
-```python
-train_dataset = DVS128Gesture(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    sampling = 600,
-    time_steps = time_steps
-)
-```
-
-Recommended sampling ratio is more than 100 (which means choose one from `sampling` events).
-
-#### Spiking Heidelberg Digits (SHD)
-
-SHD dataset records vocal number from 1 to 10 in both English and German and turns them into events. The shape of events in SHD dataset is Tx700.
-
-![SHD Dataset](./assets/readme_11.png)
-
-You can use SHD dataset in Matterhorn by the code below:
-
-```python
-from matterhorn_pytorch.data import SpikingHeidelbergDigits
-
-time_steps = 128
-
-train_dataset = SpikingHeidelbergDigits(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    time_steps = time_steps
-)
-test_dataset = SpikingHeidelbergDigits(
-    root = "your/data/path",
-    train = False,
-    download = True,
-    time_steps = time_steps
-)
-```
-
-## 4 Neuromorphic Hardware Support
-
-Will come out soon, but not today.
-
-## References
-
-[1] Wei Fang, Yanqi Chen, Jianhao Ding, Zhaofei Yu, Huihui Zhou, Timothée Masquelier, Yonghong Tian, et al. Spikingjelly. [https://github.com/fangwei123456/spikingjelly](https://github.com/fangwei123456/spikingjelly).
-
-```
-@misc{SpikingJelly,
-	title = {SpikingJelly},
-	author = {Fang, Wei and Chen, Yanqi and Ding, Jianhao and Chen, Ding and Yu, Zhaofei and Zhou, Huihui and Timothée Masquelier and Tian, Yonghong and other contributors},
-	year = {2020},
-	howpublished = {\url{https://github.com/fangwei123456/spikingjelly}},
-	note = {Accessed: 2023-08-01},
-}
-```
+# Matterhorn
+
+[Technical Documentation](./docs/en_us/README.md)
+
+[English](./README.md)
+
+[中文](./README_zh_cn.md)
+
+## 1 General Introduction
+
+![logo](./assets/logo.png)
+
+Matterhorn is a novel general neuromorphic computing framework based on PyTorch.
+
+## 2 Installation
+
+This is the brief one, for complete version you can refer to [the tutorial of Matterhorn's installation](./docs/en_us/1_install.md).
+
+### Environment
+
+Python (>= 3.7 and <= 3.9)
+
+CUDA (>= 11.3.0, with CUDNN, optional)
+
+PyTorch (>= 1.10.0 and <= 1.13.1)
+
+TorchVision (>= 0.11.0 and <= 0.13.1)
+
+### Requirement Installation
+
+For Windows version you may have to install GCC as well as G++ through Visual Studio (build tools) and [MinGW](./mingw-get-setup.exe).
+
+Then execute:
+
+```sh
+git clone https://github.com/xjtuiair-cag/Matterhorn.git
+cd Matterhorn
+pip install -r requirements.txt
+```
+
+Don't forget to add `sudo` prefix if you are not the root user.
+
+### Install Matterhorn
+
+```sh
+git clone https://github.com/xjtuiair-cag/Matterhorn.git
+cd Matterhorn
+python3 setup.py develop
+```
+
+Don't forget to add `sudo` if you are not the root user.
+
+## 3 Module Explanation
+
+For the references on specialized variables, functions or modules of SNNs, you can refer to [the detailed version of the document](./docs/en_us/snn/README.md).
+
+### Terms
+
+ANNs - Artificial Neural Networks
+
+SNNs - Spiking Neural Networks
+
+### Neurons in SNNs
+
+As we're all known, the image below describes what ANNs look like.
+
+![ANNs' Structure](./assets/readme_1.png)
+
+**Operation 1** is **synapse function**, which uses weights and bias to calculate those values from previous layer to current layer. Commonly used synapse functions are including full connection layer `nn.Linear`, convolution layer `nn.Conv2D`, etc.
+
+We use an equation to describe the synapse function:
+
+$$Y^{l}=synapse(X^{l-1})$$
+
+Where $l$ here means the number of current layers.
+
+**Operation 2** is **activation function**, which filters information from synapses and sends the filtered information to next layer. Commonly used activation functions are including `nn.ReLU`, `nn.Sigmoid`, etc.
+
+We use an equation to describe the activation function:
+
+$$X^{l}=activation(Y^{l})$$
+
+In conclusion, each of layers in ANNs has 2 functions. We can build our ANN model in PyTorch by the code below:
+
+```python
+import torch.nn as nn
+
+model = nn.Sequential(
+    nn.Linear(28 * 28, 10),
+    nn.ReLU()
+)
+```
+
+This is a 1-layer MLP. It can take an image with the size of 28x28 as input and classify it into 10 classes. In this example, two equations of ANNs can be represented as below:
+
+$$Y^{l}=W^{l}X^{l-1}+\vec{b}$$
+
+$$X^{l}=ReLU(Y^{l})$$
+
+In SNNs, the synapse equation is the same as that in ANNs. However, functions in soma are no longer like what is in ANNs. In the soma of SNNs, there exists a loop in time. The image below describes what SNNs look like.
+
+![SNN Structure](./assets/readme_2.png)
+
+**Operation 1**, the **synapse function**, calculates spikes from previous layer $O^{l-1}(t)$ thus generates the input potential $X^{l}(t)$.
+
+We use an equation to describe the synapse function:
+
+$$X^{l}(t)=synapse(O^{l-1}(t))$$
+
+By **operation 2**, the input potential, with the history potential, is calculated based on a 1-order differential equation, thus generating the soma potential $U^{l}(t)$. We name it **response function**.
+
+We use an equation to describe the response function:
+
+$$U^{l}(t)=response(H^{l}(t-1),X^{l}(t))$$
+
+Each spiking neuron model has its unique response differential equation.
+
+For example, in a LIF neuron:
+
+$$\tau \frac{du}{dt}=-(u-u_{rest})+RI$$
+
+Discretizing it into a difference equation, we can get:
+
+$$U^{l}(t)-H^{l}(t-1)=\frac{1}{\tau}[-[H^{l}(t-1)-u_{rest}]+X^{l}(t)]$$
+
+**Operation 3** uses Heaviside step function and threshold potential $u_{th}$ to decide whether to generate spikes $O^{l}(t)$. We name it **firing function**.
+
+We use an equation to describe the firing function:
+
+$$O^{l}(t)=spiking(U^{l}(t))$$
+
+Generally, the firing function looks like this.
+
+$$O^{l}(t)=Heaviside(U^{l}(t)-u_{th})$$
+
+Where Heaviside step function returns 1 when input is greater than or equal to 0, returns 0 otherwise.
+
+The aim of **operation 4** is to set refractory time on neurons by output spikes $O^{l}(t)$. We name it **reset function**.
+
+We use an equation to describe reset function:
+
+$$H^{l}(t)=reset(U^{l}(t),O^{l}(t))$$
+
+Under most occasions we use equation below to reset potential:
+
+$$H^{l}(t)=U^{l}(t)[1-O^{l}(t)]+u_{rest}O^{l}(t)$$
+
+In brief, we use 4 equations to describe spiking neurons. This is what SNN look like. The shape of a spiking neuron is like a trumpet. Its synapses transform those spikes from last neuron and pass the input response to soma, in which there is a time loop awaits.
+
+By unfolding spiking neurons on temporal dimension, we can get the spatio-temporal topology network of SNNs.
+
+![Spatial-temporal Topology Network of SNNs](./assets/readme_3.png)
+
+Like building ANNs in PyTorch, we can build our SNN model in Matterhorn by the code below:
+
+```python
+import torch
+import matterhorn_pytorch.snn as snn
+
+snn_model = snn.Temporal(
+    snn.Spatial(
+        snn.Linear(28 * 28, 10),
+        snn.LIF()
+    )
+)
+```
+
+In the code, `Spatial` is one of Matterhorn's containers to represent sequential SNN layers on spatial dimension, and `Temporal` is another Matterhorn's container to repeat calculating potential and spikes on temporal dimension. By using `Spatial` and `Temporal`, an spatio-temporal topology network is built and thus used for training and evaluating.
+
+The built network takes an $n+1$ dimensional `torch.Tensor` as input spike train. It will take the first dimension as time steps, thus calculating through each time step. after that, it will generate a `torch.Tensor` as output spike train, just like what ANNs takes and generates in PyTorch. The only difference, which is also a key point, is that we should encode our information into spike train and decode the output spike train.
+
+### Encoding and Decoding
+
+A spike train is a set of Dirac impulse functions on the axis of time.
+
+$$O(t)=\sum_{t_{i}}δ(t-t_{i})$$
+
+In other words, there will only be 0s and 1s in discrete spike train. Therefore, we can use an $n+1$ dimensional tensor to represent our spike train. For example, if neurons are flattened into a 1-dimensional vector, we can use another dimension to represent time, thus let it be a 2-dimensional matrix to represent the spike train through space and time.
+
+$$
+\begin{matrix}
+ & →s \\
+↓t &
+\begin{bmatrix}
+0 & 1 & 1 & 0 & 1 & 0 & 0 & 1 \\
+1 & 0 & 0 & 1 & 0 & 0 & 1 & 1 \\
+1 & 1 & 1 & 1 & 1 & 1 & 0 & 1 \\
+1 & 0 & 1 & 1 & 0 & 1 & 0 & 1 \\
+\end{bmatrix}
+\end{matrix}
+$$
+
+The matrix above shows what a spike train looks like. It has 4 rows, representing 4 time steps. Besides, it has 8 columns, representing 8 output neurons.
+
+To transform our traditional binary information (images, sounds, etc.) into spike train, an encoder is needed. The most commonly used encoder for non-event data is Poisson encoder, which is a kind of rate coding encoder. It sees intensity of a pixel as probability to fire a spike.
+
+You can use Poisson encoder in Matterhorn by the code below:
+
+```python
+import torch
+import matterhorn_pytorch.snn as snn
+
+encoder = snn.PoissonEncoder(
+    time_steps = 32
+)
+```
+
+Then, you can use it by the code below:
+
+```python
+spike_train = encoder(image)
+```
+
+An image with the shape of `[H, W, C]` would be encoded into a spike train with the shape of `[T, H, W, C]`. For example, a MNIST image which shape is `[28, 28]` would be encoded (`T=32`) into a spike train with the shape of `[32, 28, 28]`.
+
+After encoding and processing, the network would generate an output spike train. To get the information, we need to decode. A commonly used decoding method is to count average spikes each output neuron has generated.
+
+$$o_{i}=\frac{1}{T}\sum_{t=1}^{T}{O_{i}^{K}(t)}$$
+
+You can use average decoder in Matterhorn by the code below:
+
+```python
+import torch
+import matterhorn_pytorch.snn as snn
+
+decoder = snn.AvgSpikeDecoder()
+```
+
+It will take first dimension as temporal dimension, and generate statistical results as output. The output can be transported into ANNs for further processes.
+
+Matterhorn provides a convenient container `matterhorn_pytorch.snn.Sequential` to connect all your SNN and ANN models.
+
+```python
+import torch
+import matterhorn_pytorch.snn as snn
+
+model = snn.Sequential(
+    snn.PoissonEncoder(
+        time_steps = time_steps,
+    ),
+    snn.Flatten(),
+    snn.Linear(28 * 28, 10, bias = False),
+    snn.LIF(tau_m = tau, trainable = True),
+    snn.AvgSpikeDecoder()
+)
+```
+
+By now, you have experienced what SNNs look like and how to build it by Matterhorn. For further experience, you can refer to [examples/1_starting.py](./examples/1_starting.py).
+
+```sh
+cd Matterhorn
+python3 examples/1_starting.py
+```
+
+### Why Should We Need Surrogate Gradient
+
+In spiking neurons, we usually use Heaviside step function $u(t)$ to decide whether to generate a spike:
+
+$$O^{l}(t)=u(U^{l}(t)-u_{th})$$
+
+![Heaviside step function and its derivative, Dirac impulse function](./assets/readme_4.png)
+
+However, Heaviside step function has a derivative that can make everyone headache. Its derivative is Dirac impulse function $\delta (t)$. Dirac impulse function is infinity when x equals to 0, and 0 otherwise. If it is directly used for backpropagation, the gradient must be all damned.
+
+Therefore, some functions must be there to replace Dirac impulse function to join the backpropagation. We call those functions surrogate gradients.
+
+One of the most common surrogate gradients is rectangular function. It is a positive constant when absolute value of x is small enough, and 0 otherwise.
+
+![Use rectangular function as surrogate gradient](./assets/readme_5.png)
+
+Also, functions suitable for surrogate gradient include the derivative of sigmoidal function, Gaussian function, etc.
+
+You can inspect all provided surrogate gradient functions in `matterhorn_pytorch.snn.surrogate`.
+
+### Learning: BPTT Vs. STDP
+
+Training SNNs could be as easy as training ANNs after gradient problem of Heaviside step function is solved. After we unfold SNNs into a spatio-temporal network, backpropagation through time (BPTT) could be used in SNNs. On spatial dimension, gradients can be propagated through firing function and synapse function, thus neurons of previous layer would receive the gradient; On temporal dimension, the gradient of the next time step can be propagated through firing function and response function, thus soma of previous time would receive the gradient.
+
+![BPTT](./assets/readme_6.png)
+
+Besides BPTT, there is another simple way to train locally in each neuron without supervision, which we call spike-timing-dependent plasticity (STDP). STDP uses precise time differences between input and output spikes to calculate the weight increment.
+
+STDP follows equation below:
+
+$$Δw_{ij}=\sum_{t_{j}}{\sum_{t_{i}}W(t_{i}-t_{j})}$$
+
+where the weight function $W(x)$ is:
+
+$$
+W(x)=
+\begin{aligned}
+A_{+}e^{-\frac{x}{τ_{+}}},x>0 \\\\
+0,x=0 \\\\
+-A_{-}e^{\frac{x}{τ_{-}}},x<0
+\end{aligned}
+$$
+
+![STDP function](./assets/readme_7.png)
+
+By setting parameters $A_{+}$, $τ_{+}$, $A_{-}$ and $τ_{-}$, we can easily train SNNs unsupervised. For further experience, you can refer to [examples/2_using_stdp.py](./examples/2_using_stdp.py).
+
+```sh
+cd Matterhorn
+python3 examples/2_using_stdp.py
+```
+
+**Note:** Please make sure you have installed `matterhorn_cpp_extensions` (or `matterhorn_cuda_extensions` if you have CUDA), otherwise it will be extremely slow.
+
+```sh
+cd matterhorn_cpp_extensions
+python3 setup.py develop
+```
+
+if you have CUDA, you can install CUDA version:
+
+```sh
+cd matterhorn_cuda_extensions
+python3 setup.py develop
+```
+
+### Neuromorphic Datasets
+
+Matterhorn provides several neuromorphic datasets for training SNNs. You can experience provided neuromorphic dataset in Matterhorn by example [examples/3_convolution_and_event_datasets.py](./examples/3_convolution_and_event_datasets.py).
+
+```sh
+cd Matterhorn
+python3 examples/3_convolution_and_event_datasets.py
+```
+
+#### NMNIST
+
+We know MNIST. MNIST dataset is for training image classification, consisting of a set of 28x28 pixel grayscale images of handwritten digits (0-9). NMNIST is like MNIST, which is different is that it distorts images and record them into events. The shape of events in NMNIST Dataset is `[T, 2, 34, 34]`.
+
+![NMNIST Dataset](./assets/docs/data/readme_4.png)
+
+You can use NMNIST dataset in Matterhorn by the code below:
+
+```python
+from matterhorn_pytorch.data import NMNIST
+
+time_steps = 128
+
+train_dataset = NMNIST(
+    root = "your/data/path",
+    train = True,
+    download = True,
+    time_steps = time_steps
+)
+test_dataset = NMNIST(
+    root = "your/data/path",
+    train = False,
+    download = True,
+    time_steps = time_steps
+)
+```
+
+#### CIFAR10-DVS
+
+CIFAR10-DVS dataset records distorted CIFAR-10 image by a DVS camera. The shape of events in CIFAR10-DVS Dataset is `[T, 2, 128, 128]` .
+
+![CIFAR10-DVS Dataset](./assets/docs/data/readme_1.png)
+
+You can use CIFAR10-DVS Dataset in Matterhorn by the code below:
+
+```python
+from matterhorn_pytorch.data import CIFAR10DVS
+
+time_steps = 128
+
+train_dataset = CIFAR10DVS(
+    root = "your/data/path",
+    train = True,
+    download = True,
+    time_steps = time_steps
+)
+test_dataset = CIFAR10DVS(
+    root = "your/data/path",
+    train = False,
+    download = True,
+    time_steps = time_steps
+)
+```
+
+#### DVS128 Gesture
+
+DVS128 Gesture dataset records gestures from 29 different people under 3 different illuminating conditions by DVS camera. The shape of events in DVS128 Gesture dataset is `[T, 2, 128, 128]` .
+
+![DVS128 Gesture Dataset](./assets/docs/data/readme_2.png)
+
+You can use DVS128 Gesture dataset in Matterhorn by the code below:
+
+```python
+from matterhorn_pytorch.data import DVS128Gesture
+
+time_steps = 128
+
+train_dataset = DVS128Gesture(
+    root = "your/data/path",
+    train = True,
+    download = True,
+    time_steps = time_steps
+)
+test_dataset = DVS128Gesture(
+    root = "your/data/path",
+    train = False,
+    download = True,
+    time_steps = time_steps
+)
+```
+
+#### Spiking Heidelberg Digits (SHD)
+
+SHD dataset records vocal number from 1 to 10 in both English and German and turns them into events. The shape of events in SHD dataset is `[T, 700]`.
+
+![SHD Dataset](./assets/docs/data/readme_3.png)
+
+You can use SHD dataset in Matterhorn by the code below:
+
+```python
+from matterhorn_pytorch.data import SpikingHeidelbergDigits
+
+time_steps = 128
+
+train_dataset = SpikingHeidelbergDigits(
+    root = "your/data/path",
+    train = True,
+    download = True,
+    time_steps = time_steps
+)
+test_dataset = SpikingHeidelbergDigits(
+    root = "your/data/path",
+    train = False,
+    download = True,
+    time_steps = time_steps
+)
+```
+
+## 4 Neuromorphic Hardware Support
+
+Will come out soon, but not today. Sorry.
+
+## References (and Special Thanks to)
+
+[1] Fang W, Chen Y, Ding J, et al. SpikingJelly: An open-source machine learning infrastructure platform for spike-based intelligence[J]. Science Advances, 2023, 9(40): eadi1480.
+
+[2] Fang W, Yu Z, Chen Y, et al. Deep residual learning in spiking neural networks[J]. Advances in Neural Information Processing Systems, 2021, 34: 21056-21069.
+
+[3] Yao M, Gao H, Zhao G, et al. Temporal-wise attention spiking neural networks for event streams classification[C]//Proceedings of the IEEE/CVF International Conference on Computer Vision. 2021: 10221-10230.
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/soma.h` & `matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/soma.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 #ifndef _MATTERHORN_SOMA_H
 #define _MATTERHORN_SOMA_H
 
 #include <ATen/ATen.h>
 #include <vector>
 
+void fp_response_if(at::Tensor u, at::Tensor x, at::Tensor h);
+
+void bp_response_if(at::Tensor grad_u,
+                    at::Tensor grad_x,
+                    at::Tensor grad_h,
+                    at::Tensor u,
+                    at::Tensor x,
+                    at::Tensor h);
+
 void fp_response_lif(at::Tensor u,
                      at::Tensor x,
                      at::Tensor h,
                      at::Tensor tau_m,
                      float u_rest);
 
 void bp_response_lif(at::Tensor grad_u,
@@ -16,14 +25,58 @@
                      at::Tensor grad_tau_m,
                      at::Tensor u,
                      at::Tensor x,
                      at::Tensor h,
                      at::Tensor tau_m,
                      float u_rest);
 
+void fp_response_qif(at::Tensor u,
+                     at::Tensor x,
+                     at::Tensor h,
+                     at::Tensor tau_m,
+                     at::Tensor u_c,
+                     at::Tensor a_0,
+                     float u_rest);
+
+void bp_response_qif(at::Tensor grad_u,
+                     at::Tensor grad_x,
+                     at::Tensor grad_h,
+                     at::Tensor grad_tau_m,
+                     at::Tensor grad_u_c,
+                     at::Tensor grad_a_0,
+                     at::Tensor u,
+                     at::Tensor x,
+                     at::Tensor h,
+                     at::Tensor tau_m,
+                     at::Tensor u_c,
+                     at::Tensor a_0,
+                     float u_rest);
+
+void fp_response_expif(at::Tensor u,
+                       at::Tensor x,
+                       at::Tensor h,
+                       at::Tensor tau_m,
+                       at::Tensor u_t,
+                       at::Tensor delta_t,
+                       float u_rest);
+
+void bp_response_expif(at::Tensor grad_u,
+                       at::Tensor grad_x,
+                       at::Tensor grad_h,
+                       at::Tensor grad_tau_m,
+                       at::Tensor grad_u_t,
+                       at::Tensor grad_delta_t,
+                       at::Tensor u,
+                       at::Tensor x,
+                       at::Tensor h,
+                       at::Tensor tau_m,
+                       at::Tensor u_t,
+                       at::Tensor delta_t,
+                       float u_rest);
+
 void fp_spiking_heaviside(at::Tensor o, at::Tensor u, float u_threshold);
 
 void bp_spiking_rectangular(at::Tensor grad_o,
                             at::Tensor grad_u,
                             at::Tensor o,
                             at::Tensor u,
                             float u_threshold,
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cpp_extensions/stdp.cpp` & `matterhorn_pytorch-1.2.0/matterhorn_cpp_extensions/stdp.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,70 @@
+#ifndef _MATTERHORN_STDP
+#define _MATTERHORN_STDP
+
+
 #include "stdp.h"
 #include <ATen/ATen.h>
 #include <ATen/Functions.h>
 #include <cmath>
 #include <iostream>
 #include <vector>
 
 using namespace std;
 
 /*
 STDP主函数。
-@params:
-    weight_mat: at::Tensor 待更新的权重矩阵，形状为[output_shape,input_shape]
-    input_shape: int 输入向量长度
-    output_shape: int 输出向量长度
-    time_steps: int 时间步长
-    input_spike_train: at::Tensor 输入脉冲序列，形状为[time_steps,input_shape]
-    output_spike_train: at::Tensor 输出脉冲序列，形状为[time_steps,output_shape]
-    a_pos: float STDP参数$A^{+}$
-    tau_pos: float STDP参数$τ^{+}$
-    a_neg: float STDP参数$A^{-}$
-    tau_neg: float STDP参数$τ_{-}$
+Args:
+    weight_mat (at::Tensor): 待更新的权重矩阵，形状为[output_shape,input_shape]
+    input_shape (int): 输入向量长度
+    output_shape (int): 输出向量长度
+    time_steps (int): 时间步长
+    input_spike_train (at::Tensor): 输入脉冲序列，形状为[time_steps,input_shape]
+    output_spike_train (at::Tensor):
+输出脉冲序列，形状为[time_steps,output_shape] a_pos (float): STDP参数$A^{+}$
+    tau_pos (float): STDP参数$τ^{+}$
+    a_neg (float): STDP参数$A^{-}$
+    tau_neg (float): STDP参数$τ_{-}$
 */
 void stdp(at::Tensor weight_mat,
           int input_shape,
           int output_shape,
           int time_steps,
           at::Tensor input_spike_train,
           at::Tensor output_spike_train,
           float a_pos,
           float tau_pos,
           float a_neg,
-          float tau_neg) {
+          float tau_neg,
+          int batch_size = 1) {
     for (int i = 0; i < output_shape; i++) {
         for (int j = 0; j < input_shape; j++) {
             // 去遍历时间，更新权重
-            float weight = 0.0;
-            // 遍历输出脉冲
-            for (int ti = 0; ti < time_steps; ti++) {
-                at::Tensor spike_i = output_spike_train[ti][i];
-                if (spike_i.data<float>()[0] == 0.0) {
-                    continue;
-                }
-                // 遍历输入脉冲
-                for (int tj = 0; tj < time_steps; tj++) {
-                    at::Tensor spike_j = input_spike_train[tj][j];
-                    if (spike_j.data<float>()[0] == 0.0) {
+            at::Tensor weight = weight_mat[i][j];
+            for (int b = 0; b < batch_size; b++) {
+                // 遍历输出脉冲
+                for (int ti = 0; ti < time_steps; ti++) {
+                    at::Tensor spike_i = output_spike_train[ti][b][i];
+                    if (spike_i.data<float>()[0] < 0.5f) {
                         continue;
                     }
-                    int dt = ti - tj;
-                    if (dt > 0) {
-                        weight += a_pos * exp(-dt / tau_pos);
-                    } else if (dt < 0) {
-                        weight += -a_neg * exp(dt / tau_neg);
+                    // 遍历输入脉冲
+                    for (int tj = 0; tj < time_steps; tj++) {
+                        at::Tensor spike_j = input_spike_train[tj][b][j];
+                        if (spike_j.data<float>()[0] < 0.5f) {
+                            continue;
+                        }
+                        float dt = (float)(ti - tj);
+                        if (dt > 0.0f) {
+                            weight += a_pos * powf(1.0f / tau_pos, dt - 1.0f);
+                        } else if (dt < 0.0f) {
+                            weight -= a_neg * powf(1.0f / tau_neg, -dt - 1.0f);
+                        }
                     }
                 }
             }
-            weight_mat[i][j] += weight;
         }
     }
-}
+}
+
+
+#endif
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/setup.py` & `matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/setup.py`

 * *Files identical despite different names*

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/soma.h` & `matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/soma.h`

 * *Files identical despite different names*

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/soma_cuda.cu` & `matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/soma_cuda.cu`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+#ifndef _MATTERHORN_SOMA_CUDA_KERNEL
+#define _MATTERHORN_SOMA_CUDA_KERNEL
+
+
 #include <cmath>
 #include <iostream>
 #include <stdlib.h>
-#include "cuda_utils.h"
-#include "soma.h"
 #include "base.h"
+#include "soma.h"
 #include "base.cu"
 
 /*
 LIF神经元反应函数的前向传播函数。
 $$U_{i}^{l}(t)=H_{i}^{l}(t-1)+\frac{1}{τ_{m}}[-[H_{i}^{l}(t-1)-u_{rest}]+X_{i}^{l}(t)]$$
-@params:
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    x: at::Tensor 输入电位$X^{l}(t)$
-    h: at::Tensor 胞体历史电位$H^{l}(t-1)$
-    tau_m: at::Tensor 时间常数$τ_{m}$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    x (at::Tensor): 输入电位$X^{l}(t)$
+    h (at::Tensor): 胞体历史电位$H^{l}(t-1)$
+    tau_m (at::Tensor): 时间常数$τ_{m}$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void fp_response_lif(float& u,
                                 float x,
                                 float h,
                                 float tau_m,
                                 float u_rest) {
     u = h + (1.0f / tau_m) * (0.0f - (h - u_rest) + x);
@@ -26,104 +29,103 @@
 
 /*
 LIF神经元反应函数的反向传播函数。
 $$\frac{\partial U_{i}^{l}(t)}{\partial H_{i}^{l}(t-1)}=1-\frac{1}{τ_{m}}$$
 $$\frac{\partial U_{i}^{l}(t)}{\partial X_{i}^{l}(t)}=\frac{1}{τ_{m}}$$
 $$\frac{\partial U_{i}^{l}(t)}{\partial
 τ_{m}}=-\frac{1}{τ_{m}^{2}}[-[H_{i}^{l}(t-1)-u_{rest}]+X_{i}^{l}(t)]$$
-@params:
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    grad_x: at::Tensor 输入电位$X^{l}(t)$的梯度
-    grad_h: at::Tensor 胞体历史电位$H^{l}(t-1)$的梯度
-    grad_tau_m: at::Tensor 时间常数$τ_{m}$的梯度
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    h: at::Tensor 胞体历史电位$H^{l}(t)$
-    x: at::Tensor 输入电位$X^{l}(t-1)$
-    tau_m: at::Tensor 时间常数$τ_{m}$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    grad_x (at::Tensor): 输入电位$X^{l}(t)$的梯度
+    grad_h (at::Tensor): 胞体历史电位$H^{l}(t-1)$的梯度
+    grad_tau_m (at::Tensor): 时间常数$τ_{m}$的梯度
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    h (at::Tensor): 胞体历史电位$H^{l}(t)$
+    x (at::Tensor): 输入电位$X^{l}(t-1)$
+    tau_m (at::Tensor): 时间常数$τ_{m}$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void bp_response_lif(float grad_u,
                                 float& grad_x,
                                 float& grad_h,
                                 float& grad_tau_m,
                                 float u,
                                 float x,
                                 float h,
                                 float tau_m,
                                 float u_rest) {
     grad_x += grad_u * (1.0f / tau_m);
     grad_h = grad_u * (1.0f - (1.0f / tau_m));
-    grad_tau_m +=
-        grad_u * (0.0f - (1.0f / (tau_m * tau_m)) * (0.0f - (h - u_rest) + x));
+    grad_tau_m += grad_u * (-1.0f / powf(tau_m, 2.0f)) * (-(h - u_rest) + x);
 }
 
 /*
 Heaviside脉冲函数前向传播函数。
 $$O_{i}^{l}(t)=u[U_{i}^{l}(t)]$$
-@params:
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
+Args:
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
 */
 __device__ void fp_spiking_heaviside(float& o, float u, float u_threshold) {
     o = gef(u, u_threshold);
 }
 
 /*
 矩形窗反向传播函数。
 $$\frac{\partial O_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=u'$$
-@params:
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    a: float 参数$a$
+Args:
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    a (float): 参数$a$
 */
 __device__ void bp_spiking_rectangular(float grad_o,
                                        float& grad_u,
                                        float o,
                                        float u,
                                        float u_threshold,
                                        float a) {
     float ax = u - u_threshold;
     grad_u += grad_o * (1.0f / a) * ltf(absf(ax), a / 2.0f);
 }
 
 /*
 多项式反向传播函数。
 $$\frac{\partial O_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=u'$$
-@params:
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    a: float 参数$a$
+Args:
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    a (float): 参数$a$
 */
 __device__ void bp_spiking_polynomial(float grad_o,
                                       float& grad_u,
                                       float o,
                                       float u,
                                       float u_threshold,
                                       float a) {
-    float ax = u - u_threshold;
-    grad_u += grad_o * (sqrtf(a) / 2.0f - a / 4.0f * ax) * sgnf(2.0f / sqrtf(a) - ax);
+    float ax = absf(u - u_threshold);
+    grad_u += grad_o * (sqrtf(a) / 2.0f - a / 4.0f * ax) * sgnf(2.0f / sqrtf(a) - ax) * ltf(ax, 2.0f / sqrtf(a));
 }
 
 /*
 Sigmoid导数的反向传播函数。
 $$\frac{\partial O_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=u'$$
-@params:
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    a: float 参数$a$
+Args:
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    a (float): 参数$a$
 */
 __device__ void bp_spiking_sigmoid(float grad_o,
                                    float& grad_u,
                                    float o,
                                    float u,
                                    float u_threshold,
                                    float a) {
@@ -131,21 +133,21 @@
     float ex = expf(-ax / a);
     grad_u += grad_o * (1.0f / a) * ex / powf(1.0f + ex, 2.0f);
 }
 
 /*
 高斯反向传播函数。
 $$\frac{\partial O_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=u'$$
-@params:
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    a: float 参数$a$
+Args:
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    a (float): 参数$a$
 */
 __device__ void bp_spiking_gaussian(float grad_o,
                                     float& grad_u,
                                     float o,
                                     float u,
                                     float u_threshold,
                                     float a) {
@@ -153,36 +155,36 @@
     grad_u += grad_o * 1.0f / sqrtf(2.0f * M_PI * a) *
               expf(-powf(ax, 2.0f) / (2.0f * a));
 }
 
 /*
 硬重置前向传播函数。
 $$H_{i}^{l}(t)=U_{i}^{l}(t)[1-O_{i}^{l}(t)]+u_{rest}O_{i}^{l}(t)$$
-@params:
-    h: at::Tensor 胞体历史电位$H^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    h (at::Tensor): 胞体历史电位$H^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void fp_reset_hard(float& h, float u, float o, float u_rest) {
     h = u * (1.0f - o) + u_rest * o;
 }
 
 /*
 硬重置反向传播函数。
 $$\frac{\partial H_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=1-O_{i}^{l}(t)$$
 $$\frac{\partial H_{i}^{l}(t)}{\partial O_{i}^{l}(t)}=-U_{i}^{l}(t)+u_{rest}$$
-@params:
-    grad_h: at::Tensor 胞体历史电位$H^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    h: at::Tensor 胞体历史电位$H^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    grad_h (at::Tensor): 胞体历史电位$H^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    h (at::Tensor): 胞体历史电位$H^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void bp_reset_hard(float grad_h,
                               float& grad_u,
                               float& grad_o,
                               float h,
                               float u,
                               float o,
@@ -190,42 +192,42 @@
     grad_u += grad_h * (1.0f - o);
     grad_o += grad_h * (u_rest - u);
 }
 
 /*
 软重置前向传播函数。
 $$H_{i}^{l}(t)=U_{i}^{l}(t)[1-O_{i}^{l}(t)]+u_{rest}O_{i}^{l}(t)$$
-@params:
-    h: at::Tensor 胞体历史电位$H^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    h (at::Tensor): 胞体历史电位$H^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void fp_reset_soft(float& h,
                               float u,
                               float o,
                               float u_threshold,
                               float u_rest) {
     h = u - (u_threshold - u_rest) * o;
 }
 
 /*
 软重置反向传播函数。
 $$\frac{\partial H_{i}^{l}(t)}{\partial U_{i}^{l}(t)}=1-O_{i}^{l}(t)$$
 $$\frac{\partial H_{i}^{l}(t)}{\partial O_{i}^{l}(t)}=-U_{i}^{l}(t)+u_{rest}$$
-@params:
-    grad_h: at::Tensor 胞体历史电位$H^{l}(t)$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}(t)$的梯度
-    grad_o: at::Tensor 脉冲输出$O^{l}(t)$的梯度
-    h: at::Tensor 胞体历史电位$H^{l}(t)$
-    u: at::Tensor 胞体电位$U^{l}(t)$
-    o: at::Tensor 脉冲输出$O^{l}(t)$
-    u_threshold: float 阈电位$u_{th}$
-    u_rest: float 静息电位$u_{rest}$
+Args:
+    grad_h (at::Tensor): 胞体历史电位$H^{l}(t)$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}(t)$的梯度
+    grad_o (at::Tensor): 脉冲输出$O^{l}(t)$的梯度
+    h (at::Tensor): 胞体历史电位$H^{l}(t)$
+    u (at::Tensor): 胞体电位$U^{l}(t)$
+    o (at::Tensor): 脉冲输出$O^{l}(t)$
+    u_threshold (float): 阈电位$u_{th}$
+    u_rest (float): 静息电位$u_{rest}$
 */
 __device__ void bp_reset_soft(float grad_h,
                               float& grad_u,
                               float& grad_o,
                               float h,
                               float u,
                               float o,
@@ -233,40 +235,38 @@
                               float u_rest) {
     grad_u += grad_h * 1.0f;
     grad_o += grad_h * -(u_threshold - u_rest);
 }
 
 /*
 LIF神经元的前向传播函数。
-@params:
-    o: at::Tensor 脉冲输出$O^{l}$
-    u: at::Tensor 胞体电位$U^{l}$
-    h: at::Tensor 胞体历史电位$H^{l}$
-    x: at::Tensor 输入电位$X^{l}$
-    time_steps: int 总时间步长
-    u_init: at::Tensor 初始胞体电位$H^{l}(-1)$
-    tau_m: at::Tensor 时间常数$τ_{m}$
-    u_rest: float 静息电位$u_{rest}$
-    u_threshold: float 阈电位$u_{th}$
-    reset_mode: int 重置模式，分为硬重置（0）和软重置（1）两种
+Args:
+    o (at::Tensor): 脉冲输出$O^{l}$
+    u (at::Tensor): 胞体电位$U^{l}$
+    h (at::Tensor): 胞体历史电位$H^{l}$
+    x (at::Tensor): 输入电位$X^{l}$
+    time_steps (int): 总时间步长
+    u_init (at::Tensor): 初始胞体电位$H^{l}(-1)$
+    tau_m (at::Tensor): 时间常数$τ_{m}$
+    u_rest (float): 静息电位$u_{rest}$
+    u_threshold (float): 阈电位$u_{th}$
+    reset_mode (int): 重置模式，分为硬重置（0）和软重置（1）两种
 */
 __global__ void fp_lif_cuda_kernel(float* o,
                                    float* u,
                                    float* h,
                                    float* x,
                                    int time_steps,
                                    int shape,
                                    float* u_init,
                                    float* tau_m,
                                    float u_rest,
                                    float u_threshold,
                                    int reset_mode) {
-    int i = blockIdx.y;
-    int j = blockIdx.x * blockDim.x + threadIdx.x;
-    int idx = i * 1024 + j;
+    int idx = blockIdx.x * blockDim.x + threadIdx.x;
     if (idx >= shape) {
         return;
     }
 
     const float tau_m_val = tau_m[0];
     for (int t = 0; t < time_steps; t++) {
         const int cur_idx = t * shape + idx;
@@ -294,17 +294,15 @@
                  float* u_init,
                  float* tau_m,
                  float u_rest,
                  float u_threshold,
                  int reset_mode) {
     cudaError_t err;
 
-    // i = blockIdx.y 为行
-    // j = blockIdx.x * blockDim.x + threadIdx.x 为列
-    dim3 blocks(DIVUP(DIVUP(shape, 1024), THREADS_PER_BLOCK), 1024);
+    dim3 blocks(div_ceil(shape, THREADS_PER_BLOCK));
     dim3 threads(THREADS_PER_BLOCK);
 
     // 调用CUDA核心开始计算
     fp_lif_cuda_kernel<<<blocks, threads, 0>>>(o, u, h, x, time_steps, shape,
                                                u_init, tau_m, u_rest,
                                                u_threshold, reset_mode);
 
@@ -314,33 +312,33 @@
         fprintf(stderr, "CUDA kernel failed : %s\n", cudaGetErrorString(err));
         exit(-1);
     }
 }
 
 /*
 LIF神经元的反向传播函数。
-@params:
-    grad_o: at::Tensor 脉冲输出$O^{l}$的梯度
-    grad_u: at::Tensor 胞体电位$U^{l}$的梯度
-    grad_h: at::Tensor 胞体历史电位$H^{l}$的梯度
-    grad_x: at::Tensor 输入电位$X^{l}$的梯度
-    grad_u_init: at::Tensor 初始胞体电位$H^{l}(-1)$的梯度
-    grad_tau_m: at::Tensor 时间常数$τ_{m}$的梯度
-    time_steps: int 总时间步长
-    o: at::Tensor 脉冲输出$O^{l}$
-    u: at::Tensor 胞体电位$U^{l}$
-    h: at::Tensor 胞体历史电位$H^{l}$
-    x: at::Tensor 输入电位$X^{l}$
-    u_init: at::Tensor 初始胞体电位$H^{l}(-1)$
-    tau_m: at::Tensor 时间常数$τ_{m}$
-    u_rest: float 静息电位$u_{rest}$
-    u_threshold: float 阈电位$u_{th}$
-    spiking_mode: int 替代梯度模式
-    a: float 参数$a$
-    reset_mode: int 重置模式，分为硬重置（0）和软重置（1）两种
+Args:
+    grad_o (at::Tensor): 脉冲输出$O^{l}$的梯度
+    grad_u (at::Tensor): 胞体电位$U^{l}$的梯度
+    grad_h (at::Tensor): 胞体历史电位$H^{l}$的梯度
+    grad_x (at::Tensor): 输入电位$X^{l}$的梯度
+    grad_u_init (at::Tensor): 初始胞体电位$H^{l}(-1)$的梯度
+    grad_tau_m (at::Tensor): 时间常数$τ_{m}$的梯度
+    time_steps (int): 总时间步长
+    o (at::Tensor): 脉冲输出$O^{l}$
+    u (at::Tensor): 胞体电位$U^{l}$
+    h (at::Tensor): 胞体历史电位$H^{l}$
+    x (at::Tensor): 输入电位$X^{l}$
+    u_init (at::Tensor): 初始胞体电位$H^{l}(-1)$
+    tau_m (at::Tensor): 时间常数$τ_{m}$
+    u_rest (float): 静息电位$u_{rest}$
+    u_threshold (float): 阈电位$u_{th}$
+    spiking_mode (int): 替代梯度模式
+    a (float): 参数$a$
+    reset_mode (int): 重置模式，分为硬重置（0）和软重置（1）两种
 */
 __global__ void bp_lif_cuda_kernel(float* grad_o,
                                    float* grad_u,
                                    float* grad_h,
                                    float* grad_x,
                                    float* grad_u_init,
                                    float* grad_tau_m,
@@ -353,17 +351,15 @@
                                    float* u_init,
                                    float* tau_m,
                                    float u_rest,
                                    float u_threshold,
                                    int spiking_mode,
                                    float a,
                                    int reset_mode) {
-    int i = blockIdx.y;
-    int j = blockIdx.x * blockDim.x + threadIdx.x;
-    int idx = i * 1024 + j;
+    int idx = blockIdx.x * blockDim.x + threadIdx.x;
     if (idx >= shape) {
         return;
     }
 
     const float tau_m_val = tau_m[0];
     float cur_grad_h = 0.0f;
     for (int t = time_steps - 1; t >= 0; t--) {
@@ -395,15 +391,15 @@
                 break;
             case SURROGATE_GAUSSIAN:
                 bp_spiking_gaussian(grad_o[cur_idx], grad_u[cur_idx],
                                     o[cur_idx], u[cur_idx], u_threshold, a);
                 break;
         }
         bp_response_lif(grad_u[cur_idx], grad_x[cur_idx], cur_grad_h,
-                        grad_tau_m[0], u[cur_idx], x[cur_idx], last_h,
+                        grad_tau_m[idx], u[cur_idx], x[cur_idx], last_h,
                         tau_m_val, u_rest);
         if (t) {
             grad_h[cur_idx - shape] = cur_grad_h;
         } else {
             grad_u_init[idx] = cur_grad_h;
         }
     }
@@ -426,25 +422,26 @@
                  float u_rest,
                  float u_threshold,
                  int spiking_mode,
                  float a,
                  int reset_mode) {
     cudaError_t err;
 
-    // i = blockIdx.y 为行
-    // j = blockIdx.x * blockDim.x + threadIdx.x 为列
-    dim3 blocks(DIVUP(DIVUP(shape, 1024), THREADS_PER_BLOCK), 1024);
+    dim3 blocks(div_ceil(shape, THREADS_PER_BLOCK));
     dim3 threads(THREADS_PER_BLOCK);
 
     // 调用CUDA核心开始计算
     bp_lif_cuda_kernel<<<blocks, threads, 0>>>(
         grad_o, grad_u, grad_h, grad_x, grad_u_init, grad_tau_m, time_steps,
         shape, o, u, h, x, u_init, tau_m, u_rest, u_threshold, spiking_mode, a,
         reset_mode);
 
     // 返回计算结果
     err = cudaGetLastError();
     if (cudaSuccess != err) {
         fprintf(stderr, "CUDA kernel failed : %s\n", cudaGetErrorString(err));
         exit(-1);
     }
-}
+}
+
+
+#endif
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_cuda_extensions/stdp.h` & `matterhorn_pytorch-1.2.0/matterhorn_cuda_extensions/stdp.h`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
              int output_shape,
              int time_steps,
              at::Tensor input_spike_train,
              at::Tensor output_spike_train,
              float a_pos,
              float tau_pos,
              float a_neg,
-             float tau_neg);
+             float tau_neg,
+             int batch_size);
 
 void stdp_cuda(float* weight_mat,
                int input_shape,
                int output_shape,
                int time_steps,
                float* input_spike_train,
                float* output_spike_train,
                float a_pos,
                float tau_pos,
                float a_neg,
-               float tau_neg);
+               float tau_neg,
+               int batch_size);
 
 #endif
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/aedat.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/aedat.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,24 @@
 """
 AEDAT类数据集（后缀名为.aedat）。
 """
 
 
 import numpy as np
 import torch
-import torch.nn as nn
 import os
 import re
 import shutil
-import random
 from torchvision.datasets.utils import check_integrity, download_url, extract_archive
-from typing import Any, List, Tuple, Union, Callable, Optional
+from typing import Iterable, Union, Callable, Optional
 from urllib.error import URLError
 from zipfile import BadZipFile
 from rich import print
 from rich.progress import track
 from matterhorn_pytorch.data.skeleton import EventDataset2d
-from numba import jit
-try:
-    from rich import print
-except:
-    pass
 
 
 class AEDAT(EventDataset2d):
     original_data_polarity_exists = True
     original_size = (1, 2, 128, 128)
     mirrors = []
     resources = []
@@ -35,113 +28,121 @@
     y_shift = 16
     x_mask = 0x000007FF
     x_shift = 1
     p_mask = 0x00000001
     p_shift = 0
     
     
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True, endian: str = ">", datatype: str = "u4", clipped: Optional[Union[Tuple, int]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True, endian: str = ">", datatype: str = "u4") -> None:
         """
         原始数据后缀名为.aedat的数据集
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            time_steps: int 最终的数据集总共含有多少个时间步
-            width: int 最终数据集的宽度
-            height: int 最终数据集的高度
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            endian: str 大端还是小端，">"代表大端存储，"<"代表小端存储
-            datatype: str 数据类型，如u4表示uint32
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            width (int): 最终数据集的宽度
+            height (int): 最终数据集的高度
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
+            endian (str): 大端还是小端，">"代表大端存储，"<"代表小端存储
+            datatype (str): 数据类型，如u4表示uint32
         """
         self.endian = endian
         self.datatype = datatype
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count,
             t_size = time_steps,
             y_size = height,
             x_size = width,
-            polarity = polarity,
-            clipped = clipped 
+            polarity = polarity
         )
 
 
-    def filename_2_data(self, filename: str) -> np.ndarray:
+    @staticmethod
+    def filename_to_data(filename: str, dtype: str) -> np.ndarray:
         """
         输入文件名，读取文件内容。
-        @params:
-            filename: str 文件名
-        @return:
-            data: np.ndarray 文件内容（数据）
+        Args:
+            filename (str): 文件名
+            dtype (str): 数据类型
+        Returns:
+            data (np.ndarray): 文件内容（数据）
         """
         data_str = ""
         with open(filename, 'rb') as f:
             data_str = f.read()
             lines = data_str.split(b'\n')
             for line in range(len(lines)):
                 if not lines[line].startswith(b'#'):
                     break
             lines = lines[line:]
             data_str = b'\n'.join(lines)
-        data = np.fromstring(data_str, dtype = self.endian + self.datatype)
+        data = np.fromstring(data_str, dtype = dtype)
         return data
     
     
-    def data_2_tpyx(self, data: np.ndarray) -> np.ndarray:
+    @staticmethod
+    def data_to_tpyx(data: np.ndarray, p_shift: int, p_mask: int, y_shift: int, y_mask: int, x_shift: int, x_mask: int) -> np.ndarray:
         """
         将数据分割为t,p,y,x数组。
-        @params:
-            data: np.ndarray 数据，形状为[2n]
-        @return:
-            data_tpyx: np.ndarray 分为t,p,y,x的数据，形状为[n, 4]
+        Args:
+            data (np.ndarray): 数据，形状为[2n]
+            p_shift (int): 极性p的偏移量
+            p_mask (int): 极性p的掩膜
+            y_shift (int): 坐标y的偏移量
+            y_mask (int): 坐标y的掩膜
+            x_shift (int): 坐标x的偏移量
+            x_mask (int): 坐标x的掩膜
+        Returns:
+            data_tpyx (np.ndarray): 分为t,p,y,x的数据，形状为[n, 4]
         """
         res = np.zeros((data.shape[0] // 2, 4), dtype = "uint32")
         xyp = data[::2]
         t = data[1::2]
         res[:, 0] = t
-        res[:, 1] = self.extract(xyp, self.p_mask, self.p_shift)
-        res[:, 2] = self.extract(xyp, self.y_mask, self.y_shift)
-        res[:, 3] = self.extract(xyp, self.x_mask, self.x_shift)
+        res[:, 1] = AEDAT.clip_bits(xyp, p_mask, p_shift)
+        res[:, 2] = AEDAT.clip_bits(xyp, y_mask, y_shift)
+        res[:, 3] = AEDAT.clip_bits(xyp, x_mask, x_shift)
         res = res[np.argsort(res[:, 0])]
-        if self.sampling > 1:
-            res = res[::self.sampling]
         return res
     
     
     def label(self, key: str) -> int:
         """
         返回该文件对应的标签。
-        @params:
-            key: str 关键词
-        @return:
-            label: int 文件的标签
+        Args:
+            key (str): 关键词
+        Returns:
+            label (int): 文件的标签
         """
         if key in self.labels:
             return self.labels.index(key)
         return -1
     
     
     def is_train(self, label: int, index: int = 0) -> bool:
         """
         从路径、文件名和索引判断是否是训练集。
-        @params:
-            label: int 标签
-            index: int 文件的索引
-        @return:
-            is_train: bool 是否为训练集
+        Args:
+            label (int): 标签
+            index (int): 文件的索引
+        Returns:
+            is_train (bool): 是否为训练集
         """
         return True
 
 
 class CIFAR10DVS(AEDAT):
     original_data_polarity_exists = True
     original_size = (1, 2, 128, 128)
@@ -163,49 +164,59 @@
     y_shift = 8
     x_mask = 0x007F
     x_shift = 1
     p_mask = 0x0001
     p_shift = 0
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True, clipped: Optional[Union[Tuple, int]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True) -> None:
         """
         CIFAR-10 DVS数据集，将CIFAR10数据集投影至LCD屏幕后，用事件相机录制的数据集
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            time_steps: int 最终的数据集总共含有多少个时间步
-            width: int 最终数据集的宽度
-            height: int 最终数据集的高度
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            width (int): 最终数据集的宽度
+            height (int): 最终数据集的高度
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
         """
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count,
             time_steps = time_steps,
             width = width,
             height = height,
             polarity = polarity,
             endian = ">",
             datatype = "u4"
         )
-        if isinstance(clipped, Tuple):
-            assert clipped[1] > clipped[0], "Clip end must be larger than clip start."
-        self.clipped = clipped
+
+
+    def is_train(self, label: int, index: int = 0) -> bool:
+        """
+        从路径、文件名和索引判断是否是训练集。
+        Args:
+            label (int): 标签
+            index (int): 文件的索引
+        Returns:
+            is_train (bool): 是否为训练集
+        """
+        return index < 900
 
 
     def download(self) -> None:
         """
         下载CIFAR-10 DVS数据集
         """
         if self.check_exists():
@@ -226,15 +237,15 @@
                 except URLError as error:
                     print("[red]Error in file %s downloaded from %s:\r\n\r\n    %s\r\n\r\nPlease manually download it.[/red]" % (os.path.join(self.raw_folder , filename), url, error))
                     is_downloaded = False
             if is_downloaded:
                 print("[green]Successfully downloaded %s.[/green]" % (os.path.join(self.raw_folder, filename),))
     
 
-    def unzip(self) -> None:
+    def extract(self) -> None:
         """
         解压下载下来的压缩包。
         """
         zip_file_list = os.listdir(self.raw_folder)
         if not os.path.isdir(self.extracted_folder):
             os.makedirs(self.extracted_folder, exist_ok = True)
         extracted_folder_list = os.listdir(self.extracted_folder)
@@ -250,48 +261,37 @@
             except BadZipFile as e:
                 print("[red]Error in unzipping file %s:\r\n\r\n    %s\r\n\r\nPlease manually fix the problem.[/red]" % (filename, e))
                 error_occured = True
         if error_occured:
             raise RuntimeError("There are error(s) in unzipping files.")
 
 
-    def is_train(self, label: int, index: int = 0) -> bool:
-        """
-        从路径、文件名和索引判断是否是训练集。
-        @params:
-            label: int 标签
-            index: int 文件的索引
-        @return:
-            is_train: bool 是否为训练集
-        """
-        return index < 900
-
-
-    def load_data(self) -> np.ndarray:
+    def process(self) -> np.ndarray:
         """
         加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
+        Returns:
+            data_label (np.ndarray): 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
         """
-        list_filename = os.path.join(self.processed_folder, "__main__.csv")
+        list_filename = os.path.join(self.processed_folder, self.idx_filename)
         if os.path.isfile(list_filename):
             file_list = np.loadtxt(list_filename, dtype = "uint32", delimiter = ",")
             return file_list
-        self.unzip()
+        self.extract()
+        self.clear_processed()
         os.makedirs(self.processed_folder, exist_ok = True)
         file_list = []
         file_idx = 0
         for label_str in self.labels:
             label = self.label(label_str)
             aedat_files = os.listdir(os.path.join(self.extracted_folder, label_str))
             aedat_file_count = len(aedat_files)
             for filename in track(aedat_files, description = "Processing label %s" % (label_str,)):
-                raw_data = self.filename_2_data(os.path.join(self.extracted_folder, label_str, filename))
-                event_data = self.data_2_tpyx(raw_data)
-                self.save_event_data(file_idx, event_data)
+                raw_data = AEDAT.filename_to_data(os.path.join(self.extracted_folder, label_str, filename), self.endian + self.datatype)
+                event_data = AEDAT.data_to_tpyx(raw_data, self.p_shift, self.p_mask, self.y_shift, self.y_mask, self.x_shift, self.x_mask)
+                self.create_processed(file_idx, event_data)
                 file_list.append([file_idx, label, 1 if self.is_train(label, file_idx % aedat_file_count) else 0])
                 file_idx += 1
         file_list = np.array(file_list, dtype = "uint32")
         np.savetxt(list_filename, file_list, fmt = "%d", delimiter = ",")
         return file_list
 
 
@@ -308,104 +308,50 @@
     y_shift = 2
     x_mask = 0x1FFF
     x_shift = 17
     p_mask = 0x0001
     p_shift = 1
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True, clipped: Optional[Union[Tuple, int]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, time_steps: int = 128, width: int = 128, height: int = 128, polarity: bool = True) -> None:
         """
         DVS128 Gesture数据集，用事件相机录制手势形成的数据集
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            time_steps: int 最终的数据集总共含有多少个时间步
-            width: int 最终数据集的宽度
-            height: int 最终数据集的高度
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            width (int): 最终数据集的宽度
+            height (int): 最终数据集的高度
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
         """
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count,
             time_steps = time_steps,
             width = width,
             height = height,
             polarity = polarity,
             endian = "<",
             datatype = "u4"
         )
-        if isinstance(clipped, Tuple):
-            assert clipped[1] > clipped[0], "Clip end must be larger than clip start."
-        self.clipped = clipped
-
-
-    def download(self) -> None:
-        """
-        下载CIFAR-10 DVS数据集
-        """
-        if self.check_exists():
-            return
-        os.makedirs(self.raw_folder, exist_ok = True)
-        for fileurl, filename, md5 in self.resources:
-            if os.path.isfile(os.path.join(self.raw_folder, filename)):
-                print("[blue]File %s has already existed.[/blue]" % (os.path.join(self.raw_folder, filename),))
-                continue
-            for mirror in self.mirrors:
-                url = mirror + fileurl
-                # 本来就下不了，试过好几次了，所以直接报错完事
-                print("[red]Cannot download file %s from %s, please manually download it.[/red]" % (os.path.join(self.raw_folder, filename), url))
-
-
-    def unzip(self) -> None:
-        """
-        解压下载下来的压缩包。
-        """
-        if os.path.isdir(self.extracted_folder):
-            print("[blue]Files are already unzipped.[/blue]")
-            return
-        os.makedirs(self.extracted_folder, exist_ok = True)
-        filename = "DvsGesture.tar.gz"
-        error_occured = False
-        print("[blue]Trying to unzip file %s ...[/blue]" % (filename,))
-        try:
-            extract_archive(os.path.join(self.raw_folder, filename), self.extracted_folder)
-            print("[green]Sussessfully unzipped file %s.[/green]" % (filename,))
-        except BadZipFile as e:
-            print("[red]Error in unzipping file %s:\r\n\r\n    %s\r\n\r\nPlease manually fix the problem.[/red]" % (filename, e))
-            error_occured = True
-        if error_occured:
-            shutil.rmtree(self.extracted_folder)
-            raise RuntimeError("There are error(s) in unzipping files.")
-
 
-    def is_train(self, label: int, index: int = 0) -> bool:
-        """
-        从路径、文件名和索引判断是否是训练集。
-        @params:
-            label: int 标签
-            index: int 文件的索引
-        @return:
-            is_train: bool 是否为训练集
-        """
-        return index < 24
-    
 
     @staticmethod
-    @jit(nopython=True)
     def skip_header(data: np.ndarray, mask: np.ndarray) -> np.ndarray:
         cursor = 0
         while cursor < len(data):
             header = data[cursor:cursor + 7]
             event_type = (header[0] >> 16) & 0xFFFF # 1
             event_source = header[0] & 0xFFFF # 1
             event_size = header[1] # 8
@@ -422,65 +368,119 @@
                 if event_ts_overflow:
                     data[cursor + 1:end:2] += event_ts_overflow << 31
             cursor += event_capacity * event_size // 4
         data = data[mask]
         return data
     
 
-    def filename_2_data(self, filename: str) -> np.ndarray:
+    @staticmethod
+    def filename_to_data(filename: str, dtype: str) -> np.ndarray:
         """
         输入文件名，读取文件内容。
-        @params:
-            filename: str 文件名
-        @return:
-            data: np.ndarray 文件内容（数据）
+        Args:
+            filename (str): 文件名
+            dtype (str): 数据类型
+        Returns:
+            data (np.ndarray): 文件内容（数据）
         """
         data_str = ""
         with open(filename, 'rb') as f:
             data_str = f.read()
             lines = data_str.split(b'\n')
             for line in range(len(lines)):
                 if not lines[line].startswith(b'#'):
                     break
             lines = lines[line:]
             data_str = b'\n'.join(lines)
-            data = np.fromstring(data_str, dtype = self.endian + self.datatype)
+            data = np.fromstring(data_str, dtype = dtype)
             data = DVS128Gesture.skip_header(data, np.zeros(data.shape, dtype = "bool"))
         return data
 
 
-    def load_data(self) -> np.ndarray:
+    def is_train(self, label: int, index: int = 0) -> bool:
+        """
+        从路径、文件名和索引判断是否是训练集。
+        Args:
+            label (int): 标签
+            index (int): 文件的索引
+        Returns:
+            is_train (bool): 是否为训练集
+        """
+        return index < 24
+
+
+    def download(self) -> None:
+        """
+        下载CIFAR-10 DVS数据集
+        """
+        if self.check_exists():
+            return
+        os.makedirs(self.raw_folder, exist_ok = True)
+        for fileurl, filename, md5 in self.resources:
+            if os.path.isfile(os.path.join(self.raw_folder, filename)):
+                print("[blue]File %s has already existed.[/blue]" % (os.path.join(self.raw_folder, filename),))
+                continue
+            for mirror in self.mirrors:
+                url = mirror + fileurl
+                # 本来就下不了，试过好几次了，所以直接报错完事
+                print("[red]Cannot download file %s from %s, please manually download it.[/red]" % (os.path.join(self.raw_folder, filename), url))
+
+
+    def extract(self) -> None:
+        """
+        解压下载下来的压缩包。
+        """
+        if os.path.isdir(self.extracted_folder):
+            print("[blue]Files are already unzipped.[/blue]")
+            return
+        os.makedirs(self.extracted_folder, exist_ok = True)
+        filename = "DvsGesture.tar.gz"
+        error_occured = False
+        print("[blue]Trying to unzip file %s ...[/blue]" % (filename,))
+        try:
+            extract_archive(os.path.join(self.raw_folder, filename), self.extracted_folder)
+            print("[green]Sussessfully unzipped file %s.[/green]" % (filename,))
+        except BadZipFile as e:
+            print("[red]Error in unzipping file %s:\r\n\r\n    %s\r\n\r\nPlease manually fix the problem.[/red]" % (filename, e))
+            error_occured = True
+        if error_occured:
+            shutil.rmtree(self.extracted_folder)
+            raise RuntimeError("There are error(s) in unzipping files.")
+
+
+    def process(self) -> np.ndarray:
         """
         加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
+        Returns:
+            data_label (np.ndarray): 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
         """
-        list_filename = os.path.join(self.processed_folder, "__main__.csv")
+        list_filename = os.path.join(self.processed_folder, self.idx_filename)
         if os.path.isfile(list_filename):
             file_list = np.loadtxt(list_filename, dtype = "uint32", delimiter = ",")
             return file_list
-        self.unzip()
+        self.extract()
+        self.clear_processed()
         aedat_file_dir = os.path.join(self.extracted_folder, "DvsGesture")
         aedat_files = os.listdir(aedat_file_dir)
         os.makedirs(self.processed_folder, exist_ok = True)
         file_list = []
         file_idx = 0
         for filename in track(aedat_files, description = "Processing"):
             if not filename.endswith(".aedat"):
                 continue
-            raw_data = self.filename_2_data(os.path.join(aedat_file_dir, filename))
-            event_data = self.data_2_tpyx(raw_data)
+            raw_data = DVS128Gesture.filename_to_data(os.path.join(aedat_file_dir, filename), self.endian + self.datatype)
+            event_data = DVS128Gesture.data_to_tpyx(raw_data, self.p_shift, self.p_mask, self.y_shift, self.y_mask, self.x_shift, self.x_mask)
             event_data[:, 2] = self.original_size[2] - 1 - event_data[:, 2]
             event_data[:, 3] = self.original_size[3] - 1 - event_data[:, 3]
             class_info = np.loadtxt(os.path.join(aedat_file_dir, filename.replace(".aedat", "_labels.csv")), dtype = "uint32", delimiter = ",", skiprows = 1)
             for label, start, end in class_info:
                 data = event_data[(event_data[:, 0] >= start) & (event_data[:, 0] < end)]
                 data[:, 0] = data[:, 0] - start
                 user_id = re.search(r"user([0-9]+)", filename)
                 user_id = user_id.group(1)
                 is_train = self.is_train(label, int(user_id))
-                self.save_event_data(file_idx, event_data)
+                self.create_processed(file_idx, event_data)
                 file_list.append([file_idx, label - 1, 1 if is_train else 0])
                 file_idx += 1
         file_list = np.array(file_list, dtype = "uint32")
         np.savetxt(list_filename, file_list, fmt = "%d", delimiter = ",")
         return file_list
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/hdf5.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/hdf5.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,85 +3,74 @@
 HDF5类数据集（后缀名为.h5）。
 """
 
 
 import numpy as np
 import torch
 import os
-import random
 import h5py
 from torchvision.datasets.utils import check_integrity, download_url, extract_archive
-from typing import Any, List, Tuple, Union, Callable, Optional
+from typing import Iterable, Union, Callable, Optional
 from urllib.error import URLError
 from zipfile import BadZipFile
 from rich import print
 from rich.progress import track
 from matterhorn_pytorch.data.skeleton import EventDataset1d
-try:
-    from rich import print
-except:
-    pass
 
 
 class HDF5(EventDataset1d):
     original_data_polarity_exists = True
     training_file = "training.pt"
     test_file = "test.pt"
     original_size = (1, 2, 128)
     mirrors = []
     resources = []
     labels = []
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, precision: int = 1e9, time_steps: int = 128, length: int = 128, clipped: Optional[Union[Tuple, float]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, precision: int = 1e9, time_steps: int = 128, length: int = 128) -> None:
         """
         原始数据后缀名为.hdf5的数据集
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            precision: int 最终数据集的时间精度
-            time_steps: int 最终的数据集总共含有多少个时间步
-            length: int 最终数据集的空间精度
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            precision (int): 最终数据集的时间精度
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            length (int): 最终数据集的空间精度
         """
         self.precision = precision
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
+            count = count,
             t_size = time_steps,
             x_size = length,
-            polarity = False,
-            clipped = clipped
+            polarity = False
         )
 
 
-    def load_data(self) -> np.ndarray:
-        """
-        加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
-        """
-        return None
-
-
-    def filename_2_data(self, filename: str) -> h5py.File:
+    @staticmethod
+    def filename_to_data(filename: str) -> h5py.File:
         """
         输入文件名，读取文件内容。
-        @params:
-            filename: str 文件名
-        @return:
-            data: np.ndarray 文件内容（数据）
+        Args:
+            filename (str): 文件名
+        Returns:
+            data (np.ndarray): 文件内容（数据）
         """
         data = h5py.File(filename, "r")
         return data
 
 
 class SpikingHeidelbergDigits(HDF5):
     original_data_polarity_exists = False
@@ -90,42 +79,42 @@
     resources = [
         ('shd_train.h5.zip', 'shd_train.h5.zip', 'f3252aeb598ac776c1b526422d90eecb'),
         ('shd_test.h5.zip', 'shd_test.h5.zip', '1503a5064faa34311c398fb0a1ed0a6f')
     ]
     labels = ["zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine", "null", "eins", "zwei", "drei", "vier", "fünf", "sechs", "sieben", "acht", "neun"]
     
     
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, precision: int = 1e9, time_steps: int = 128, length: int = 700, clipped: Optional[Union[Tuple, float]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, precision: float = 1e9, time_steps: int = 128, length: int = 700) -> None:
         """
         Spiking Heidelberg Digits数据集，记录下英文和德语的0-9（总共20类），并转换成长度为700的脉冲。
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            precision: int 最终数据集的时间精度
-            time_steps: int 最终的数据集总共含有多少个时间步
-            length: int 最终数据集的空间精度
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            precision (float): 最终数据集的时间精度
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            length (int): 最终数据集的空间精度
         """
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count,
             precision = precision,
             time_steps = time_steps,
-            length = length,
-            clipped = clipped
+            length = length
         )
         
     
     def download(self) -> None:
         """
         下载数据集。
         """
@@ -147,15 +136,15 @@
                 except URLError as error:
                     print("[red]Error in file %s downloaded from %s:\r\n\r\n    %s\r\n\r\nPlease manually download it.[/red]" % (os.path.join(self.raw_folder , filename), url, error))
                     is_downloaded = False
             if is_downloaded:
                 print("[green]Successfully downloaded %s.[/green]" % (os.path.join(self.raw_folder, filename),))
 
 
-    def unzip(self) -> None:
+    def extract(self) -> None:
         """
         解压下载下来的压缩包。
         """
         zip_file_list = os.listdir(self.raw_folder)
         if not os.path.isdir(self.extracted_folder):
             os.makedirs(self.extracted_folder, exist_ok = True)
         extracted_folder_list = os.listdir(self.extracted_folder)
@@ -171,41 +160,40 @@
             except BadZipFile as e:
                 print("[red]Error in unzipping file %s:\r\n\r\n    %s\r\n\r\nPlease manually fix the problem.[/red]" % (filename, e))
                 error_occured = True
         if error_occured:
             raise RuntimeError("There are error(s) in unzipping files.")
 
 
-    def load_data(self) -> np.ndarray:
+    def process(self) -> np.ndarray:
         """
         加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
+        Returns:
+            data_label (np.ndarray): 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
         """
-        list_filename = os.path.join(self.processed_folder, "__main__.csv")
+        list_filename = os.path.join(self.processed_folder, self.idx_filename)
         if os.path.isfile(list_filename):
             file_list = np.loadtxt(list_filename, dtype = "uint32", delimiter = ",")
             return file_list
-        self.unzip()
+        self.extract()
+        self.clear_processed()
         os.makedirs(self.processed_folder, exist_ok = True)
         file_list = []
         file_idx = 0
         for is_train in range(2):
             is_train_str = "train" if is_train else "test"
-            raw_data = self.filename_2_data(os.path.join(self.extracted_folder, "shd_%s.h5" % (is_train_str,)))
+            raw_data = SpikingHeidelbergDigits.filename_to_data(os.path.join(self.extracted_folder, "shd_%s.h5" % (is_train_str,)))
             label_list = raw_data["labels"][:]
             for idx in track(range(len(label_list)), description = "Processing %sing set" % (is_train_str,)):
                 t = np.floor(raw_data["spikes"]["times"][idx] * self.precision).astype("uint32")
                 x = raw_data["spikes"]["units"][idx]
                 event_data = np.zeros((len(x), 2), dtype = "uint32")
                 event_data[:, 0] = t
                 event_data[:, 1] = x
-                res = res[np.argsort(res[:, 0])]
-                if self.sampling > 1:
-                    event_data = event_data[::self.sampling]
+                event_data = event_data[np.argsort(event_data[:, 0])]
                 label = label_list[idx]
-                self.save_event_data(file_idx, event_data)
+                self.create_processed(file_idx, event_data)
                 file_list.append([file_idx, label, is_train])
                 file_idx += 1
         file_list = np.array(file_list, dtype = "uint32")
         np.savetxt(list_filename, file_list, fmt = "%d", delimiter = ",")
         return file_list
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/nmnist.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/nmnist.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,72 +3,101 @@
 NMNIST数据集。
 """
 
 
 import numpy as np
 import torch
 import os
-import random
 from torchvision.datasets.utils import check_integrity, download_url, extract_archive
-from typing import Any, List, Tuple, Union, Callable, Optional
+from typing import Iterable, Union, Callable, Optional
 from urllib.error import URLError
 from zipfile import BadZipFile
 from rich import print
 from rich.progress import track
 from matterhorn_pytorch.data.skeleton import EventDataset2d
-try:
-    from rich import print
-except:
-    pass
 
 
 class NMNIST(EventDataset2d):
     original_data_polarity_exists = True
     original_size = (1, 2, 34, 34)
     mirrors = ["https://data.mendeley.com/public-files/datasets/468j46mzdv/files/"]
     resources = [
         ("39c25547-014b-4137-a934-9d29fa53c7a0/file_downloaded", "Train.zip", "20959b8e626244a1b502305a9e6e2031"),
         ("05a4d654-7e03-4c15-bdfa-9bb2bcbea494/file_downloaded", "Test.zip", "69ca8762b2fe404d9b9bad1103e97832")
     ]
     labels = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]
     
     
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, time_steps: int = 128, width: int = 34, height: int = 34, polarity: bool = True, clipped: Optional[Union[Tuple, int]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, time_steps: int = 128, width: int = 34, height: int = 34, polarity: bool = True) -> None:
         """
         NMNIST数据集，将MNIST数据集动态变换后，转为事件的形式。
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            time_steps: int 最终的数据集总共含有多少个时间步
-            width: int 最终数据集的宽度
-            height: int 最终数据集的高度
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            time_steps (int): 最终的数据集总共含有多少个时间步
+            width (int): 最终数据集的宽度
+            height (int): 最终数据集的高度
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
         """
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count,
             t_size = time_steps,
             y_size = height,
             x_size = width,
-            polarity = polarity,
-            clipped = clipped
+            polarity = polarity
         )
 
 
+    @staticmethod
+    def filename_to_data(filename: str) -> np.ndarray:
+        """
+        输入文件名，读取文件内容。
+        Args:
+            filename (str): 文件名
+        Returns:
+            data (np.ndarray): 文件内容（数据）
+        """
+        data_str = ""
+        with open(filename, 'rb') as f:
+            data_str = f.read()
+        data = np.fromstring(data_str, dtype = ">u1")
+        return data
+
+
+    @staticmethod
+    def data_to_tpyx(data: np.ndarray) -> np.ndarray:
+        """
+        将数据分割为t,p,y,x数组。
+        Args:
+            data (np.ndarray): 数据，形状为[5n]
+        Returns:
+            data_tpyx (np.ndarray): 分为t,p,y,x的数据，形状为[n, 4]
+        """
+        res = np.zeros((data.shape[0] // 5, 4), dtype = "uint32")
+        res[:, 0] = ((data[2::5] & 0x7f) << 16) + (data[3::5] << 8) + data[4::5]
+        res[:, 1] = data[2::5] >> 7
+        res[:, 2] = 33 - data[1::5]
+        res[:, 3] = data[::5]
+        res = res[np.argsort(res[:, 0])]
+        return res
+
+
     def download(self) -> None:
         """
         下载数据集。
         """
         if self.check_exists():
             return
         os.makedirs(self.raw_folder, exist_ok = True)
@@ -87,15 +116,15 @@
                 except URLError as error:
                     print("[red]Error in file %s downloaded from %s:\r\n\r\n    %s\r\n\r\nPlease manually download it.[/red]" % (os.path.join(self.raw_folder , filename), url, error))
                     is_downloaded = False
             if is_downloaded:
                 print("[green]Successfully downloaded %s.[/green]" % (os.path.join(self.raw_folder, filename),))
 
 
-    def unzip(self) -> None:
+    def extract(self) -> None:
         """
         解压下载下来的压缩包。
         """
         zip_file_list = os.listdir(self.raw_folder)
         if not os.path.isdir(self.extracted_folder):
             os.makedirs(self.extracted_folder, exist_ok = True)
         extracted_folder_list = os.listdir(self.extracted_folder)
@@ -111,70 +140,37 @@
             except BadZipFile as e:
                 print("[red]Error in unzipping file %s:\r\n\r\n    %s\r\n\r\nPlease manually fix the problem.[/red]" % (filename, e))
                 error_occured = True
         if error_occured:
             raise RuntimeError("There are error(s) in unzipping files.")
 
 
-    def filename_2_data(self, filename: str) -> np.ndarray:
-        """
-        输入文件名，读取文件内容。
-        @params:
-            filename: str 文件名
-        @return:
-            data: np.ndarray 文件内容（数据）
-        """
-        data_str = ""
-        with open(filename, 'rb') as f:
-            data_str = f.read()
-        data = np.fromstring(data_str, dtype = ">u1")
-        return data
-
-
-    def data_2_tpyx(self, data: np.ndarray) -> np.ndarray:
-        """
-        将数据分割为t,p,y,x数组。
-        @params:
-            data: np.ndarray 数据，形状为[5n]
-        @return:
-            data_tpyx: np.ndarray 分为t,p,y,x的数据，形状为[n, 4]
-        """
-        res = np.zeros((data.shape[0] // 5, 4), dtype = "uint32")
-        res[:, 0] = ((data[2::5] & 0x7f) << 16) + (data[3::5] << 8) + data[4::5]
-        res[:, 1] = data[2::5] >> 7
-        res[:, 2] = self.original_size[2] - 1 - data[1::5]
-        res[:, 3] = data[::5]
-        res = res[np.argsort(res[:, 0])]
-        if self.sampling > 1:
-            res = res[::self.sampling]
-        return res
-
-
-    def load_data(self) -> np.ndarray:
+    def process(self) -> np.ndarray:
         """
         加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
+        Returns:
+            data_label (np.ndarray): 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
         """
-        list_filename = os.path.join(self.processed_folder, "__main__.csv")
+        list_filename = os.path.join(self.processed_folder, self.idx_filename)
         if os.path.isfile(list_filename):
             file_list = np.loadtxt(list_filename, dtype = "uint32", delimiter = ",")
             return file_list
-        self.unzip()
+        self.extract()
+        self.clear_processed()
         os.makedirs(self.processed_folder, exist_ok = True)
         file_list = []
         file_idx = 0
         for is_train in range(2):
             is_train_str = "Train" if is_train else "Test"
             for label in track(range(len(self.labels)), description = "Processing %sing set" % (is_train_str.lower(),)):
                 label_str = self.labels[label]
                 raw_file_dir = os.path.join(self.extracted_folder, is_train_str, label_str)
                 raw_file_list = os.listdir(raw_file_dir)
                 for raw_filename in raw_file_list:
-                    raw_data = self.filename_2_data(os.path.join(raw_file_dir, raw_filename))
-                    event_data = self.data_2_tpyx(raw_data)
-                    self.save_event_data(file_idx, event_data)
+                    raw_data = NMNIST.filename_to_data(os.path.join(raw_file_dir, raw_filename))
+                    event_data = NMNIST.data_to_tpyx(raw_data)
+                    self.create_processed(file_idx, event_data)
                     file_list.append([file_idx, label, is_train])
                     file_idx += 1
         file_list = np.array(file_list, dtype = "uint32")
         np.savetxt(list_filename, file_list, fmt = "%d", delimiter = ",")
         return file_list
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/data/skeleton.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/data/skeleton.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,423 +4,489 @@
 """
 
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 from torchvision.datasets.utils import check_integrity
-from typing import Tuple, Union, Callable, Optional
+from typing import Tuple, Iterable, Union, Callable, Optional
+from rich import print
+from rich.progress import track
 import os
-import random
-try:
-    from rich import print
-except:
-    pass
+import json
+import time
+import shutil
+import multiprocessing
+from concurrent.futures import ThreadPoolExecutor, wait
+import hashlib
+import matterhorn_pytorch.data.functional as DF
 
 
 class EventDataset(Dataset):
+    idx_filename = "__main__.csv"
     original_data_polarity_exists = False
     original_size = (1,)
     mirrors = []
     resources = []
     labels = []
+    shape = None
     data_target = []
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False) -> None:
         """
         事件数据集框架
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
         """
         super().__init__()
         self.root = root
         self.transform = transform
         self.target_transform = target_transform
         self.train = train
-        self.sampling = sampling
+        self.cached = cached
+        self.cache_dtype = cache_dtype
         self.count = count
         if download:
             self.download()
         self.pre_process()
 
 
     @property
     def raw_folder(self) -> str:
         """
         刚下载下来的数据集所存储的地方。
-        @return:
-            str 数据集存储位置
+        Returns:
+            res (str): 数据集存储位置
         """
         return os.path.join(self.root, self.__class__.__name__, "raw")
 
 
     @property
     def extracted_folder(self) -> str:
         """
         解压过后的数据集所存储的地方。
-        @return:
-            str 数据集存储位置
+        Returns:
+            res (str): 数据集存储位置
         """
         return os.path.join(self.root, self.__class__.__name__, "extracted")
 
 
     @property
     def processed_folder(self) -> str:
         """
         处理过后的数据集所存储的地方。
-        @return:
-            str 数据集存储位置
+        Returns:
+            res (str): 数据集存储位置
         """
-        return os.path.join(self.root, self.__class__.__name__, "processed", "%d" % (self.sampling,))
+        return os.path.join(self.root, self.__class__.__name__, "processed")
+
+
+    @property
+    def cached_folder(self) -> str:
+        """
+        张量缓存所存储的地方。
+        Returns:
+            res (str): 张量缓存位置
+        """
+        return os.path.join(self.root, self.__class__.__name__, "cached")
+
+
+    @property
+    def cache_tag(self) -> str:
+        """
+        张量缓存标签。
+        Returns:
+            res (str): 张量缓存标签
+        """
+        appendix = "_%s" % (str(self.cache_dtype))
+        if self.transform is not None:
+            appendix += "_" + hashlib.md5(repr(self.transform).encode("utf-8")).hexdigest()
+        if self.count:
+            appendix += "_count"
+        return "x".join([str(i) for i in self.shape]) + appendix
 
 
     def check_exists(self) -> bool:
         """
         检查是否存在。
-        @return:
-            if_exist: bool 是否存在
+        Returns:
+            if_exist (bool): 是否存在
         """
         return all(
             check_integrity(os.path.join(self.raw_folder, filename)) for fileurl, filename, md5 in self.resources
         )
 
 
-    def download(self) -> None:
+    @staticmethod
+    def clip_bits(data: np.ndarray, mask: int, shift: int) -> np.ndarray:
         """
-        下载数据集。
+        从事件数据中提取x,y,p值所用的函数。
+        Args:
+            data (np.ndarray): 事件数据
+            mask (int): 对应的掩模
+            shift (int): 对应的偏移量
+        Returns:
+            data (np.ndarray): 处理后的数据（x,y,p）
         """
-        return
+        return (data >> shift) & mask
 
 
-    def extract(self, data: np.ndarray, mask: int, shift: int) -> np.ndarray:
+    def create_processed(self, data_idx: int, event_data: np.ndarray) -> bool:
         """
-        从事件数据中提取x,y,p值所用的函数。
-        @params:
-            data: np.ndarray 事件数据
-            mask: int 对应的掩模
-            shift: int 对应的偏移量
-        @return:
-            data: np.ndarray 处理后的数据（x,y,p）
+        将预处理的数据存储至文件中。
+        Args:
+            data_idx (int): 数据序号
+            event_data (np.ndarray): 事件数据
         """
-        return (data >> shift) & mask
+        np.save(os.path.join(self.processed_folder, "%d.npy" % (data_idx,)), event_data)
+        return True
 
 
-    def load_data(self) -> np.ndarray:
-        """
-        加载数据集。
-        @return:
-            data_label: np.ndarray 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
+    def clear_processed(self, except_index: bool = False) -> None:
         """
-        return None
-    
+        清空processed文件夹中的内容。
+        Args:
+            except_index (bool): 是否要排除"__main__.csv"
+        """
+        if os.path.isdir(self.processed_folder):
+            shutil.rmtree(self.processed_folder)
+        self.clear_cache()
+
+
+    def create_cache(self) -> None:
+        """
+        创建缓存。
+        """
+        info_json = os.path.join(self.cached_folder, "__info__.json")
+        cache_info = {
+            "type": self.cache_tag,
+            "object_num": len(self.data_target),
+            "last_modified": time.time()
+        }
+
+        # 打开缓存文件夹，查看基本信息
+        if os.path.isdir(self.cached_folder) and os.path.isfile(info_json):   
+            with open(info_json, "r", encoding = "utf-8") as f:
+                old_cache_info = json.load(f)
+            cache_type = old_cache_info["type"]
+            cache_size = old_cache_info["object_num"]
+            cache_mtime = old_cache_info["last_modified"]
+            file_num = sum([1 if s.endswith(".pt") else 0 for s in os.listdir(self.cached_folder)])
+
+            # 如果类型对得上，且文件个数一致，就更新基本信息，使用原缓存
+            if cache_type == self.cache_tag and cache_size == len(self.data_target) and cache_size == file_num:
+                print("[green]Using cache file.[/green]")
+                with open(info_json, "w", encoding = "utf-8") as f:
+                    json.dump(cache_info, f)
+                return
+        
+        # 若打不开缓存文件夹或缓存文件夹不满足条件，清除原有的其它缓存，重建新的缓存
+        self.clear_cache()
+        os.makedirs(self.cached_folder, exist_ok = True)
+        print("[blue]Making cache, please wait ...[/blue]")
+
+        def create_cache_file(source: str, dest: str, convert: Callable, dtype: torch.dtype) -> None:
+            """
+            将数据从源地址加载出来后，经过转换，放入目标地址。
+            Args:
+                source (str): 源地址
+                dest (str): 目标地址
+                convert (Callable): 转换规则
+            """
+            if os.path.isfile(dest):
+                return
+            data = np.load(source)
+            data = convert(data)
+            data = data.to(dtype)
+            torch.save(data, dest)
+        
+        # 使用多线程进行转换。为保险起见，用最多2*CPU个worker，每次处理4*CPU个数据
+        workers_num = multiprocessing.cpu_count() * 2
+        batch_size = workers_num * 4
+        looping = ((len(self.data_target) - 1) // batch_size) + 1
+
+        # 循环处理每个数据，得到缓存
+        for i in track(range(looping), description = "Making cache"):
+            with ThreadPoolExecutor(max_workers = workers_num) as t:
+                # 执行线程
+                task_pool = []
+                for j in range(batch_size):
+                    idx = i * batch_size + j
+                    if idx >= len(self.data_target):
+                        break
+                    data_idx = self.data_target[idx][0]
+                    source_dir = os.path.join(self.processed_folder, "%d.npy" % (data_idx,))
+                    target_dir = os.path.join(self.cached_folder, "%d.pt" % (data_idx,))
+                    task_pool.append(t.submit(create_cache_file, source_dir, target_dir, self.event_data_to_tensor, self.cache_dtype))
+                wait(task_pool)
+
+                # 检查线程有无出错
+                for k in range(len(task_pool)):
+                    t = task_pool[k]
+                    if t.exception():
+                        print("[red bold]Error occured in thread %d:[/red bold]" % (idx,))
+                        raise RuntimeError(t.exception())
+        
+        # 写入基本信息
+        print("[green]Successfully made cache of %d data.[/green]" % (len(self.data_target,)))
+        with open(info_json, "w", encoding = "utf-8") as f:
+            json.dump(cache_info, f)
+
 
-    def save_event_data(self, data_idx: int, event_data: np.ndarray) -> bool:
+    def clear_cache(self) -> None:
         """
-        将预处理的数据存储至文件中。
-        @params:
-            data_idx: int 数据序号
-            event_data: np.ndarray 事件数据
+        清除缓存。
         """
-        event_data = self.compress_event_data(event_data)
-        np.save(os.path.join(self.processed_folder, "%d.npy" % (data_idx,)), event_data)
-        return True
-    
+        if os.path.isdir(self.cached_folder):
+            shutil.rmtree(self.cached_folder)
 
-    def pre_process(self) -> None:
+
+    def download(self) -> None:
         """
-        数据的预处理，可以自定义。
+        下载数据集。
         """
-        if not self.check_exists():
-            raise RuntimeError("Dataset not found. You can use download=True to download it")
-        self.data_target = self.load_data()
-        self.data_target = self.data_target[self.data_target[:, 2] == (1 if self.train else 0)][:, :2]
-        self.data_target = self.data_target.tolist()
-        random.shuffle(self.data_target)
-    
+        return
 
-    def compress_event_data(self, data: np.ndarray) -> np.ndarray:
+
+    def process(self) -> np.ndarray:
         """
-        压缩事件数据。
-        @params:
-            data: np.ndarray 未被压缩的数据
-        @return:
-            compressed_data: np.ndarray 已被压缩的数据
+        加载数据集。
+        Returns:
+            data_label (np.ndarray): 数据信息，包括3列：数据集、标签、其为训练集（1）还是测试集（0）。
         """
-        return data
+        return None
 
 
-    def decompress_event_data(self, data: np.ndarray) -> np.ndarray:
+    def pre_process(self) -> None:
         """
-        解压事件数据。
-        @params:
-            data: np.ndarray 未被解压的数据
-        @return:
-            decompressed_data: np.ndarray 已被解压的数据
+        数据的预处理，可以自定义。
         """
-        return data
+        if not self.check_exists():
+            raise RuntimeError("Dataset not found. You can use download=True to download it")
+        self.data_target = self.process()
+        if self.cached:
+            self.create_cache()
+        self.data_target = self.data_target[self.data_target[:, 2] == (1 if self.train else 0)][:, :2]
+        self.data_target = self.data_target.tolist()
 
 
-    def event_data_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def event_data_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将缓存的numpy矩阵转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量
+        Args:
+            data (np.ndarray): 数据
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量
         """
-        return torch.tensor(data, dtype = torch.float)
+        if self.transform is not None:
+            data = self.transform(data)
+        return data
 
 
     def __len__(self) -> int:
         """
         获取数据集长度。
-        @return:
-            len: int 数据集长度
+        Returns:
+            len (int): 数据集长度
         """
         return len(self.data_target)
     
     
     def __getitem__(self, index: int) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         获取数据集。
-        @params:
-            index: int 索引
-        @return:
-            x: torch.Tensor 数据
-            y: torch.Tensor 标签
+        Args:
+            index (int): 索引
+        Returns:
+            x (torch.Tensor): 数据
+            y (torch.Tensor): 标签
         """
         data_idx = self.data_target[index][0]
-        data = np.load(os.path.join(self.processed_folder, "%d.npy" % (data_idx,)))
-        data = self.decompress_event_data(data)
-        data = self.event_data_2_tensor(data)
+        if self.cached:
+            data = torch.load(os.path.join(self.cached_folder, "%d.pt" % (data_idx,)))
+            data = data.to(torch.float)
+        else:
+            source_dir = os.path.join(self.processed_folder, "%d.npy" % (data_idx,))
+            data = np.load(source_dir)
+            data = self.event_data_to_tensor(data)
         target = self.data_target[index][1]
-        if self.transform is not None:
-            data = self.transform(data)
         if self.target_transform is not None:
             target = self.target_transform(data)
         return data, target
 
 
 class EventDataset1d(EventDataset):
     original_size = (1, 2, 128)
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, t_size: int = 128, x_size: int = 128, polarity: bool = True, clipped: Optional[Union[Tuple, float]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, t_size: int = 128, x_size: int = 128, polarity: bool = True) -> None:
         """
         一维事件数据集框架
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            t_size: int 时间维度的大小
-            x_size: int 空间维度的大小
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            t_size (int): 时间维度的大小
+            x_size (int): 空间维度的大小
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
         """
         self.t_size = t_size
         self.p_size = 2 if polarity else 1
         self.x_size = x_size
-        if isinstance(clipped, Tuple):
-            assert clipped[1] > clipped[0], "Clip end must be larger than clip start."
-        self.clipped = clipped
+        self.shape = (self.t_size, self.p_size, self.x_size)
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count
         )
     
 
-    def tx_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def tx_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将t,x数组转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据，形状为[n, 2]
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量，形状为[T, L]
-        """
-        data = data.astype("float32")
-        res = torch.zeros(self.t_size, self.x_size, dtype = torch.float)
-        if not data.shape[0]:
-            return res
-        if self.clipped is not None:
-            if isinstance(self.clipped, int):
-                data = data[data[:, 0] < self.clipped]
-            elif isinstance(self.clipped, Tuple):
-                data = data[(data[:, 0] >= self.clipped[0]) & (data[:, 0] < self.clipped[1])]
-        data[:, 0] -= np.min(data[:, 0])
-        data[:, 0] = np.floor(data[:, 0] * self.t_size / max(np.max(data[:, 0]) + 1, self.original_size[0]))
-        data[:, 1] = np.floor(data[:, 1] * self.x_size / self.original_size[2])
-        data, counts = np.unique(data, axis = 0, return_counts = True)
-        t_filter = (data[:, 0] >= 0) & (data[:, 0] < self.t_size)
-        data = data[t_filter].astype("int32")
-        counts = counts[t_filter].astype("float32")
-        res[data.T] = torch.tensor(counts, dtype = torch.float) if self.count else 1
+        Args:
+            data (np.ndarray): 数据，形状为[n, 2]
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量，形状为[T, L]
+        """
+        res = DF.event_seq_to_spike_train(
+            event_seq = data,
+            shape = (self.t_size, self.x_size),
+            original_shape = (max(np.max(data[:, 0]) + 1, self.original_size[0]), self.original_size[2]),
+            count = self.count
+        )
         return res
     
 
-    def tpx_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def tpx_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将t,p,x数组转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据，形状为[n, 3]
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量，形状为[T, C(P), L]
-        """
-        data = data.astype("float32")
-        res = torch.zeros(self.t_size, self.p_size, self.x_size, dtype = torch.float)
-        if not data.shape[0]:
-            return res
-        if self.clipped is not None:
-            if isinstance(self.clipped, int):
-                data = data[data[:, 0] < self.clipped]
-            elif isinstance(self.clipped, Tuple):
-                data = data[(data[:, 0] >= self.clipped[0]) & (data[:, 0] < self.clipped[1])]
-        data[:, 0] -= np.min(data[:, 0])
-        data[:, 0] = np.floor(data[:, 0] * self.t_size / max(np.max(data[:, 0]) + 1, self.original_size[0]))
-        data[:, 1] = np.floor(data[:, 1] * self.p_size / self.original_size[1])
-        data[:, 2] = np.floor(data[:, 2] * self.x_size / self.original_size[2])
-        data, counts = np.unique(data, axis = 0, return_counts = True)
-        t_filter = (data[:, 0] >= 0) & (data[:, 0] < self.t_size)
-        data = data[t_filter].astype("int32")
-        counts = counts[t_filter].astype("float32")
-        res[data.T] = torch.tensor(counts, dtype = torch.float) if self.count else 1
+        Args:
+            data (np.ndarray): 数据，形状为[n, 3]
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量，形状为[T, C(P), L]
+        """
+        res = DF.event_seq_to_spike_train(
+            event_seq = data,
+            shape = (self.t_size, self.p_size, self.x_size),
+            original_shape = (max(np.max(data[:, 0]) + 1, self.original_size[0]), self.original_size[1], self.original_size[2]),
+            count = self.count
+        )
         return res
 
 
-    def event_data_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def event_data_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将缓存的numpy矩阵转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量
+        Args:
+            data (np.ndarray): 数据
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量
         """
+        data = super().event_data_to_tensor(data)
         if self.original_data_polarity_exists:
-            return self.tpx_2_tensor(data)
-        return self.tx_2_tensor(data)
+            return self.tpx_to_tensor(data)
+        return self.tx_to_tensor(data)
 
 
 class EventDataset2d(EventDataset):
     original_size = (1, 2, 128, 128)
 
 
-    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, sampling: int = 1, count: bool = False, t_size: int = 128, y_size: int = 128, x_size: int = 128, polarity: bool = True, clipped: Optional[Union[Tuple, float]] = None) -> None:
+    def __init__(self, root: str, train: bool = True, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None, download: bool = False, cached: bool = True, cache_dtype: torch.dtype = torch.uint8, count: bool = False, t_size: int = 128, y_size: int = 128, x_size: int = 128, polarity: bool = True) -> None:
         """
         二维事件数据集框架
-        @params:
-            root: str 数据集的存储位置
-            train: bool 是否为训练集
-            transform: Callable | None 数据如何变换
-            target_transform: Callable | None 标签如何变换
-            download: bool 如果数据集不存在，是否应该下载
-            sampling: int 是否进行采样（每隔n个事件采样一次），1为不采样（保存每个事件）
-            count: bool 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
-            t_size: int 时间维度的大小
-            y_size: int 第一个空间维度的大小
-            x_size: int 第二个空间维度的大小
-            polarity: bool 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
-            clipped: bool 要在t为什么范围内截取事件，接受None（不截取）、int（结尾）或tuple（开头与结尾）
+        Args:
+            root (str): 数据集的存储位置
+            train (bool): 是否为训练集
+            transform (Callable | None): 数据如何变换
+            target_transform (Callable | None): 标签如何变换
+            download (bool): 如果数据集不存在，是否应该下载
+            cached (bool): 是否为数据集作缓存。若为 False，则不作缓存，但是代价是运行速度变慢
+            cache_dtype (torch.dtype): 如果为数据集作缓存，缓存的数据类型。默认为8位整型数，若count=True，您可能需要更高的精度储存脉冲张量
+            count (bool): 是否采取脉冲计数，若为True则输出张量中各个点脉冲的个数，否则只输出是否有脉冲
+            t_size (int): 时间维度的大小
+            y_size (int): 第一个空间维度的大小
+            x_size (int): 第二个空间维度的大小
+            polarity (bool): 最终数据集是否采集极性信息，如果采集，通道数就是2，否则是1
         """
         self.t_size = t_size
         self.p_size = 2 if polarity else 1
         self.y_size = y_size
         self.x_size = x_size
-        if isinstance(clipped, Tuple):
-            assert clipped[1] > clipped[0], "Clip end must be larger than clip start."
-        self.clipped = clipped
+        self.shape = (self.t_size, self.p_size, self.y_size, self.x_size)
         super().__init__(
             root = root,
             train = train,
             transform = transform,
             target_transform = target_transform,
             download = download,
-            sampling = sampling,
+            cached = cached,
+            cache_dtype = cache_dtype,
             count = count
         )
 
 
-    def tyx_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def tyx_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将t,y,x数组转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据，形状为[n, 3]
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量，形状为[T, H, W]
-        """
-        data = data.astype("float32")
-        res = torch.zeros(self.t_size, self.y_size, self.x_size, dtype = torch.float)
-        if not data.shape[0]:
-            return res
-        if self.clipped is not None:
-            if isinstance(self.clipped, int):
-                data = data[data[:, 0] < self.clipped]
-            elif isinstance(self.clipped, Tuple):
-                data = data[(data[:, 0] >= self.clipped[0]) & (data[:, 0] < self.clipped[1])]
-        data[:, 0] -= np.min(data[:, 0])
-        data[:, 0] = np.floor(data[:, 0] * self.t_size / max(np.max(data[:, 0]) + 1, self.original_size[0]))
-        data[:, 1] = np.floor(data[:, 1] * self.y_size / self.original_size[2])
-        data[:, 2] = np.floor(data[:, 2] * self.x_size / self.original_size[3])
-        data, counts = np.unique(data, axis = 0, return_counts = True)
-        t_filter = (data[:, 0] >= 0) & (data[:, 0] < self.t_size)
-        data = data[t_filter].astype("int32")
-        counts = counts[t_filter].astype("float32")
-        res[data.T] = torch.tensor(counts, dtype = torch.float) if self.count else 1
+        Args:
+            data (np.ndarray): 数据，形状为[n, 3]
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量，形状为[T, H, W]
+        """
+        res = DF.event_seq_to_spike_train(
+            event_seq = data,
+            shape = (self.t_size, self.y_size, self.x_size),
+            original_shape = (max(np.max(data[:, 0]) + 1, self.original_size[0]), self.original_size[2], self.original_size[3]),
+            count = self.count
+        )
         return res
 
 
-    def tpyx_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def tpyx_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将t,p,y,x数组转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据，形状为[n, 4]
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量，形状为[T, C(P), H, W]
-        """
-        data = data.astype("float32")
-        res = torch.zeros(self.t_size, self.p_size, self.y_size, self.x_size, dtype = torch.float)
-        if not data.shape[0]:
-            return res
-        if self.clipped is not None:
-            if isinstance(self.clipped, int):
-                data = data[data[:, 0] < self.clipped]
-            elif isinstance(self.clipped, Tuple):
-                data = data[(data[:, 0] >= self.clipped[0]) & (data[:, 0] < self.clipped[1])]
-        data[:, 0] -= np.min(data[:, 0])
-        np.set_printoptions(threshold = np.inf)
-        data[:, 0] = np.floor(data[:, 0] * self.t_size / max(np.max(data[:, 0]) + 1, self.original_size[0]))
-        data[:, 1] = np.floor(data[:, 1] * self.p_size / self.original_size[1])
-        data[:, 2] = np.floor(data[:, 2] * self.y_size / self.original_size[2])
-        data[:, 3] = np.floor(data[:, 3] * self.x_size / self.original_size[3])
-        data, counts = np.unique(data, axis = 0, return_counts = True)
-        t_filter = (data[:, 0] >= 0) & (data[:, 0] < self.t_size)
-        data = data[t_filter].astype("int32")
-        counts = counts[t_filter].astype("float32")
-        res[data.T] = torch.tensor(counts, dtype = torch.float) if self.count else 1
+        Args:
+            data (np.ndarray): 数据，形状为[n, 4]
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量，形状为[T, C(P), H, W]
+        """
+        res = DF.event_seq_to_spike_train(
+            event_seq = data,
+            shape = (self.t_size, self.p_size, self.y_size, self.x_size),
+            original_shape = (max(np.max(data[:, 0]) + 1, self.original_size[0]), self.original_size[1], self.original_size[2], self.original_size[3]),
+            count = self.count
+        )
         return res
 
 
-    def event_data_2_tensor(self, data: np.ndarray) -> torch.Tensor:
+    def event_data_to_tensor(self, data: np.ndarray) -> torch.Tensor:
         """
         将缓存的numpy矩阵转为最后的PyTorch张量。
-        @params:
-            data: np.ndarray 数据
-        @return:
-            data_tensor: torch.Tensor 渲染成事件的张量
+        Args:
+            data (np.ndarray): 数据
+        Returns:
+            data_tensor (torch.Tensor): 渲染成事件的张量
         """
+        data = super().event_data_to_tensor(data)
         if self.original_data_polarity_exists:
-            return self.tpyx_2_tensor(data)
-        return self.tyx_2_tensor(data)
+            return self.tpyx_to_tensor(data)
+        return self.tyx_to_tensor(data)
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/sew.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/sew.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,114 +13,130 @@
 from typing import Tuple, Callable
 try:
     from rich import print
 except:
     pass
 
 
+from matterhorn_pytorch.snn.soma import LIF
+if torch.cuda.is_available():
+    try:
+        from matterhorn_pytorch.snn.soma_cuda import LIF
+    except:
+        try:
+            from matterhorn_pytorch.snn.soma_cpp import LIF
+        except:
+            pass
+else:
+    try:
+        from matterhorn_pytorch.snn.soma_cpp import LIF
+    except:
+        pass
+
+
 class ResADD(snn.Module):
     def __init__(self) -> None:
         super().__init__(
             multi_time_step = True
         )
 
 
     def forward(self, a: torch.Tensor, s: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数，ADD连接函数。
-        @params:
-            a: torch.Tensor 经过两层卷积处理后的脉冲张量
-            s: torch.Tensor 原始脉冲张量
-        @return:
-            o: torch.Tensor 输出脉冲张量
+        Args:
+            a (torch.Tensor): 经过两层卷积处理后的脉冲张量
+            s (torch.Tensor): 原始脉冲张量
+        Returns:
+            o (torch.Tensor): 输出脉冲张量
         """
         return a + s
 
 
 class ResAND(snn.Module):
     def __init__(self) -> None:
         super().__init__(
             multi_time_step = True
         )
 
 
     def forward(self, a: torch.Tensor, s: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数，AND连接函数。
-        @params:
-            a: torch.Tensor 经过两层卷积处理后的脉冲张量
-            s: torch.Tensor 原始脉冲张量
-        @return:
-            o: torch.Tensor 输出脉冲张量
+        Args:
+            a (torch.Tensor): 经过两层卷积处理后的脉冲张量
+            s (torch.Tensor): 原始脉冲张量
+        Returns:
+            o (torch.Tensor): 输出脉冲张量
         """
         return a * s
 
 
 class ResIAND(snn.Module):
     def __init__(self) -> None:
         super().__init__(
             multi_time_step = True
         )
 
 
     def forward(self, a: torch.Tensor, s: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数，IAND连接函数。
-        @params:
-            a: torch.Tensor 经过两层卷积处理后的脉冲张量
-            s: torch.Tensor 原始脉冲张量
-        @return:
-            o: torch.Tensor 输出脉冲张量
+        Args:
+            a (torch.Tensor): 经过两层卷积处理后的脉冲张量
+            s (torch.Tensor): 原始脉冲张量
+        Returns:
+            o (torch.Tensor): 输出脉冲张量
         """
         return (1.0 - a) * s
 
 
-def ConvLIF(in_channels: int, out_channels: int, kernel_size: int = 3, stride: int = 1, tau_m: float = 2.0, spiking_function: snn.Module = snn.Rectangular(), trainable: bool = False):
+def ConvLIF(in_channels: int, out_channels: int, kernel_size: int = 3, stride: int = 1, tau_m: float = 2.0, spiking_function: snn.Module = snn.Gaussian(), trainable: bool = False):
     """
     绑定卷积神经元（突触）和LIF神经元（胞体）
-    @params:
-        in_channels: int 输入脉冲通道数
-        out_channels: int 输出脉冲通道数
-        kernel_size: int 卷积核的大小
-        stride: int 卷积步长
-        tau_m: float 参数τ_{m}，神经元时间常数
-        spiking_function: snn.Module 脉冲函数
-        trainable: bool 参数是否可以训练
+    Args:
+        in_channels (int): 输入脉冲通道数
+        out_channels (int): 输出脉冲通道数
+        kernel_size (int): 卷积核的大小
+        stride (int): 卷积步长
+        tau_m (float): 参数τ_{m}，神经元时间常数
+        spiking_function (snn.Module): 脉冲函数
+        trainable (bool): 参数是否可以训练
     """
     return snn.Sequential(
         snn.Conv2d(
             in_channels = in_channels,
             out_channels = out_channels,
             kernel_size = kernel_size,
             stride = stride,
             padding = kernel_size // 2
         ),
         snn.BatchNorm2d(
             num_features = out_channels
         ),
-        snn.LIF(
+        LIF(
             tau_m = tau_m,
             spiking_function = spiking_function,
             trainable = trainable
         )
     )
 
 
 class SEWBlock(snn.Module):
-    def __init__(self, in_channels: int, out_channels: int, tau_m: float = 2.0, spiking_function: snn.Module = snn.Rectangular(), residual_connection: snn.Module = ResADD(), down_sampling: bool = False, trainable: bool = False) -> None:
+    def __init__(self, in_channels: int, out_channels: int, tau_m: float = 2.0, spiking_function: snn.Module = snn.Gaussian(), residual_connection: snn.Module = ResADD(), down_sampling: bool = False, trainable: bool = False) -> None:
         """
         Spiking Element-Wise Block， SEW ResNet的单元。
-        @params:
-            in_channels: int 输入脉冲通道数
-            out_channels: int 输出脉冲通道数
-            tau_m: float 参数τ_{m}，神经元时间常数
-            spiking_function: snn.Module 脉冲函数
-            residual_connection: snn.Module 脉冲连接方式
-            down_sampling: bool 是否进行下采样（出来的图像大小是原大小的一半）
-            trainable: bool 参数是否可以训练
+        Args:
+            in_channels (int): 输入脉冲通道数
+            out_channels (int): 输出脉冲通道数
+            tau_m (float): 参数τ_{m}，神经元时间常数
+            spiking_function (snn.Module): 脉冲函数
+            residual_connection (snn.Module): 脉冲连接方式
+            down_sampling (bool): 是否进行下采样（出来的图像大小是原大小的一半）
+            trainable (bool): 参数是否可以训练
         """
         super().__init__(
             multi_time_step = True
         )
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.conv1 = ConvLIF(
@@ -162,53 +178,42 @@
                 trainable = trainable
             )
         else:
             self.down_sampling_block = None
         self.residual_connection = residual_connection
     
 
-    def reset(self) -> None:
-        """
-        重置模型。
-        """
-        self.conv1.reset()
-        self.conv2.reset()
-        if self.down_sampling_block is not None:
-            self.down_sampling_block.reset()
-        self.residual_connection.reset()
-    
-
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 输入脉冲张量
-        @return:
-            o: torch.Tensor 输出脉冲张量
+        Args:
+            x (torch.Tensor): 输入脉冲张量
+        Returns:
+            o (torch.Tensor): 输出脉冲张量
         """
         a = self.conv2(self.conv1(x))
         if self.down_sampling_block is not None:
             s = self.down_sampling_block(x)
         else:
             s = x
         o = self.residual_connection(a, s)
         return o
 
 
 class SEWRes18(snn.Module):
-    def __init__(self, input_h_w: Tuple[int] = (128, 128), num_classes: int = 10, tau_m: float = 2.0, spiking_function: snn.Module = snn.Rectangular(), residual_connection: snn.Module = ResADD(), trainable: bool = False) -> None:
+    def __init__(self, input_h_w: Tuple[int] = (128, 128), num_classes: int = 10, tau_m: float = 2.0, spiking_function: snn.Module = snn.Gaussian(), residual_connection: snn.Module = ResADD(), trainable: bool = False) -> None:
         """
         Spiking Element-Wise Block， SEW ResNet的单元。
-        @params:
-            input_h_w: Tuple[int] 输出脉冲通道数
-            num_classes: int 输出类别数
-            tau_m: float 参数τ_{m}，神经元时间常数
-            spiking_function: snn.Module 脉冲函数
-            residual_connection: snn.Module 脉冲连接方式
-            trainable: bool 参数是否可以训练
+        Args:
+            input_h_w (int*): 输出脉冲通道数
+            num_classes (int): 输出类别数
+            tau_m (float): 参数τ_{m}，神经元时间常数
+            spiking_function (snn.Module): 脉冲函数
+            residual_connection (snn.Module): 脉冲连接方式
+            trainable (bool): 参数是否可以训练
         """
         super().__init__(
             multi_time_step = True
         )
         self.model = snn.Sequential(
             snn.DirectEncoder(),
             ConvLIF(
@@ -295,27 +300,21 @@
                 kernel_size = (input_h_w[0] >> 5, input_h_w[1] >> 5)
             ), # [512, 1, 1]
             nn.Flatten(), # [512]
             nn.Linear(
                 in_features = 512,
                 out_features = num_classes
             ), # [10]
+            nn.Softmax()
         )
-    
-
-    def reset(self) -> None:
-        """
-        重置模型。
-        """
-        self.model.reset()
 
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 输入脉冲张量
-        @return:
-            x: torch.Tensor 输出张量
+        Args:
+            x (torch.Tensor): 输入脉冲张量
+        Returns:
+            x (torch.Tensor): 输出张量
         """
         x = self.model(x)
         return x
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/model/ta.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/model/ta.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,83 +17,74 @@
     pass
 
 
 class TemporalWiseAttention(snn.Module):
     def __init__(self, time_steps: int, r: float, d_threshold: float) -> None:
         """
         Tempora-wise Attention连接层
-        @params:
-            time_steps: int 时间步长
-            r: float 用于控制权重矩阵的大小(T*(T/r)和(T/r)*T)
-            d_threshold: float 注意阈值，用于阶跃函数
+        Args:
+            time_steps (int): 时间步长
+            r (float): 用于控制权重矩阵的大小(T*(T/r)和(T/r)*T)
+            d_threshold (float): 注意阈值，用于阶跃函数
         """
         super().__init__(
             multi_time_step = True
         )
         self.time_steps = time_steps
         self.r = r
         self.d_threshold = d_threshold
 
         self.fc1 = snn.Linear(self.time_steps, math.floor(self.time_steps / self.r), bias = False)
         self.fc2 = snn.Linear(math.floor(self.time_steps / self.r), self.time_steps, bias = False)
         self.relu = nn.ReLU()
         self.sigmoid = nn.Sigmoid()
-        self.heaviside = snn.Rectangular()
-
-
-    def reset(self) -> None:
-        """
-        重置模型。
-        """
-        self.fc1.reset()
-        self.fc2.reset()
-        self.heaviside.reset()
+        self.heaviside = snn.Gaussian()
     
 
     def f_train(self, s: torch.Tensor) -> torch.Tensor:
         """
         训练模式下的前向传播，公式为$d^{n-1}=σ(W_{2}^{n}δ(W_{1}^{n}s^{n-1}]))$
-        @params:
-            s: torch.Tensor 统计向量$s^{n-1}$
-        @return:
-            d: torch.Tensor 分数向量$d^{n-1}$
+        Args:
+            s (torch.Tensor): 统计向量$s^{n-1}$
+        Returns:
+            d (torch.Tensor): 分数向量$d^{n-1}$
         """
         dim = len(s.shape)
         if dim > 1:
             s = s.permute(1, 0) # 将形状[T, B]翻转为[B, T]
         d = self.sigmoid(self.fc2(self.relu(self.fc1(s))))
         if dim > 1:
             d = d.permute(1, 0) # 将形状[B, T]翻转为[T, B]
         return d
 
 
     def f_inf(self, s: torch.Tensor) -> torch.Tensor:
         """
         推理模式下的前向传播，公式为$d^{n-1}=σ(W_{2}^{n}δ(W_{1}^{n}s^{n-1}]))$
-        @params:
-            s: torch.Tensor 统计向量$s^{n-1}$，形状为[B, T]
-        @return:
-            d: torch.Tensor 分数向量$d^{n-1}$，形状为[B, T]
+        Args:
+            s (torch.Tensor): 统计向量$s^{n-1}$，形状为[B, T]
+        Returns:
+            d (torch.Tensor): 分数向量$d^{n-1}$，形状为[B, T]
         """
         dim = len(s.shape)
         if dim > 1:
             s = s.permute(1, 0) # 将形状[T, B]翻转为[B, T]
         d = self.heaviside(self.sigmoid(self.fc2(self.relu(self.fc1(s)))) - self.d_threshold)
         if dim > 1:
             d = d.permute(1, 0) # 将形状[B, T]翻转为[T, B]
         return d
 
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数
-        @params:
-            x: torch.Tensor 原始脉冲张量
-        @return:
-            x: torch.Tensor 过滤后的脉冲张量
+        Args:
+            x (torch.Tensor): 原始脉冲张量
+        Returns:
+            x (torch.Tensor): 过滤后的脉冲张量
         """
         is_train = x.requires_grad
         dim = len(x.shape)
         s = x.clone().detach().requires_grad_(is_train)
         pre_permute = []
         post_permute = []
         # 获取统计向量$s^{n-1}$
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/__init__.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: UTF-8 -*-
 """
 此文件夹放置SNN的一些基本模块。
 """
 
 
+from . import functional
 from .container import Spatial, Temporal, Sequential
 from .decoder import SumSpike as SumSpikeDecoder, AverageSpike as AvgSpikeDecoder, MinTime as MinTimeDecoder, AverageTime as AvgTimeDecoder
 from .encoder import Direct as DirectEncoder, Poisson as PoissonEncoder, Temporal as TemporalEncoder
-from .layer import SRM0Linear, MaxPool1d, MaxPool2d, MaxPool3d, AvgPool1d, AvgPool2d, AvgPool3d, Flatten, Unflatten
+from .layer import STDPLinear, MaxPool1d, MaxPool2d, MaxPool3d, AvgPool1d, AvgPool2d, AvgPool3d, Flatten, Unflatten, Dropout, Dropout1d, Dropout2d, Dropout3d
 from .skeleton import Module
-from .soma import Soma, IF, LIF, QIF, EIF, Izhikevich, KLIF, LIAF
+from .soma import IF, LIF, QIF, ExpIF, Izhikevich, KLIF, LIAF
 from .surrogate import Rectangular, Polynomial, Sigmoid, Gaussian
-from .synapse import Linear, Conv1d, Conv2d, Conv3d, ConvTranspose1d, ConvTranspose2d, ConvTranspose3d, BatchNorm1d, BatchNorm2d, BatchNorm3d, LayerNorm
+from .synapse import Linear, Conv1d, Conv2d, Conv3d, ConvTranspose1d, ConvTranspose2d, ConvTranspose3d, BatchNorm1d, BatchNorm2d, BatchNorm3d, LayerNorm, Neurotransmitter
 try:
     from rich import print
 except:
     pass
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/encoder.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,36 +3,41 @@
 脉冲神经网络的编码机制。
 注意：此单元可能会改变张量形状。
 """
 
 
 import torch
 import torch.nn as nn
+import matterhorn_pytorch.snn.functional as SF
 from matterhorn_pytorch.snn.skeleton import Module
+from typing import Callable
 try:
     from rich import print
 except:
     pass
 
 
 class Encoder(Module):
-    def __init__(self) -> None:
+    def __init__(self, reset_after_process: bool = False) -> None:
         """
         编码器的基类。编码器是一个多时间步模型。
+        Args:
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
         """
         super().__init__(
-            multi_time_step = True
+            multi_time_step = True,
+            reset_after_process = reset_after_process
         )
 
 
     def supports_single_time_step(self) -> bool:
         """
         是否支持单个时间步。
-        @return:
-            if_support: bool 是否支持单个时间步
+        Returns:
+            if_support (bool): 是否支持单个时间步
         """
         return False
 
 
 class Direct(Encoder):
     def __init__(self) -> None:
         """
@@ -40,171 +45,167 @@
         """
         super().__init__()
     
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         直接编码的前向传播函数，直接将第二个维度作为时间维度，转置到首个维度上
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,T,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[T,B,...]
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,T,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[T,B,...]
         """
         idx = [i for i, j in enumerate(x.shape)]
-        assert len(idx) >= 2, "There is no time steps."
+        assert len(idx) >= 2, "There is no temporal dimension."
         idx[0], idx[1] = idx[1], idx[0]
         y = x.permute(*idx)
         return y
 
 
 class Poisson(Encoder):
-    def __init__(self, time_steps: int = 1, max_value: float = 1.0, min_value: float = 0.0) -> None:
+    def __init__(self, time_steps: int = 1) -> None:
         """
         泊松编码（速率编码），将值转化为脉冲发放率（多步）
-        @params:
-            time_steps: int 生成的时间步长
-            max_value: float 最大值
-            min_value: float 最小值
+        Args:
+            time_steps (int): 生成的时间步长
         """
         super().__init__()
-        assert max_value > min_value, "Max value is less than min value."
         self.time_steps = time_steps
-        self.max_value = max_value
-        self.min_value = min_value
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return "time_steps=%d, max=%.3f, min=%.3f" % (self.time_steps, self.max_value, self.min_value)
+        return "time_steps=%d" % (self.time_steps)
 
 
     def forward_single(self, x:torch.Tensor) -> torch.Tensor:
         """
         单步前向传播函数。
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[B,...]
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[B,...]
         """
         r = torch.rand_like(x)
-        y = r.le(x).to(x)
+        y = SF.le(r, x)
         return y
     
 
-    def forward_multiple(self, x: torch.Tensor, time_steps: int) -> torch.Tensor:
+    def forward_multiple(self, x: torch.Tensor) -> torch.Tensor:
         """
         多步前向传播函数。
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[T, B,...]
-        """
-        y_seq = []
-        for t in range(time_steps):
-            y_seq.append(self.forward_single(x))
-        y = torch.stack(y_seq)
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[T, B,...]
+        """
+        res_shape = [self.time_steps] + list(x.shape)
+        v = torch.ones(*res_shape).to(x) * x
+        y = self.forward_single(v)
         return y
 
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         泊松编码的前向传播函数，将值$V$转化为该时间步$t$内的脉冲$O^{0}(t)$
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[T,B,...]
-        """
-        x = (x - self.min_value) / (self.max_value - self.min_value)
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[T,B,...]
+        """
+        min_value = torch.min(x)
+        max_value = torch.max(x)
+        if max_value == min_value:
+            x = torch.full_like(x, 0.5)
+        else:
+            x = (x - min_value) / (max_value - min_value)
         if self.time_steps <= 1:
             y = self.forward_single(x)
         else:
-            y = self.forward_multiple(x, self.time_steps)
+            y = self.forward_multiple(x)
         return y
 
 
 class Temporal(Encoder):
-    def __init__(self, time_steps: int = 1, max_value: float = 1.0, min_value: float = 0.0, prob: float = 0.75, reset_after_process: bool = True) -> None:
+    def __init__(self, time_steps: int = 1, prob: float = 1.0, transform: Callable = lambda x: x, reset_after_process: bool = True) -> None:
         """
         时间编码，在某个时间之前不会产生脉冲，在某个时间之后随机产生脉冲
-        @params:
-            time_steps: int 生成的时间步长
-            max_value: float 最大值
-            min_value: float 最小值
-            prob: float 若达到了时间，以多大的概率发放脉冲，范围为[0, 1]
-            reset_after_process: bool 是否在执行完后自动重置，若为False则需要手动重置
+        Args:
+            time_steps (int): 生成的时间步长
+            prob (float): 若达到了时间，以多大的概率发放脉冲，范围为[0, 1]
+            transform (Callable): 将数据x如何变形
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
         """
-        super().__init__()
-        assert max_value > min_value, "Max value is less than min value."
+        super().__init__(
+            reset_after_process = reset_after_process
+        )
         self.time_steps = time_steps
-        self.max_value = max_value
-        self.min_value = min_value
         self.prob = prob
-        self.reset_after_process = reset_after_process
+        self.transform = transform
         self.reset()
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return "time_steps=%d, max=%.3f, min=%.3f, spike_freq=%.3f" % (self.time_steps, self.max_value, self.min_value, self.prob)
+        return "time_steps=%d, prob=%g, reset_after_process=%s" % (self.time_steps, self.prob, str(self.reset_after_process))
 
 
-    def reset(self) -> None:
+    def reset(self) -> Module:
         """
         重置编码器
         """
         self.current_time_step = 0
+        return super().reset()
 
 
-    def forward_single(self, x:torch.Tensor) -> torch.Tensor:
+    def forward_single(self, x: torch.Tensor) -> torch.Tensor:
         """
         单步前向传播函数。
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[B,...]
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[B,...]
         """
-        f = (self.current_time_step + 0.0 - x).ge(0.0).to(x)
-        r = torch.rand_like(x).le(self.prob).to(x)
+        f = SF.le(x, self.current_time_step)
+        r = SF.le(torch.rand_like(x), self.prob)
         y = f * r
         self.current_time_step += 1
         return y
     
 
     def forward_multiple(self, x: torch.Tensor, time_steps: int) -> torch.Tensor:
         """
         多步前向传播函数。
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[T, B,...]
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[T, B,...]
         """
         y_seq = []
         for t in range(time_steps):
             y_seq.append(self.forward_single(x))
         y = torch.stack(y_seq)
         return y
 
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
-        泊松编码的前向传播函数，将值$V$转化为该时间步$t$内的脉冲$O^{0}(t)$
-        @params:
-            x: torch.Tensor 输入张量，形状为[B,...]
-        @return:
-            y: torch.Tensor 输出张量，形状为[T,B,...]
+        时间编码的前向传播函数，将值$V$转化为该时间步$t$内的脉冲$O^{0}(t)$
+        Args:
+            x (torch.Tensor): 输入张量，形状为[B,...]
+        Returns:
+            y (torch.Tensor): 输出张量，形状为[T,B,...]
         """
-        x = (x - self.min_value) / (self.max_value - self.min_value) * self.time_steps
+        x = self.transform(x)
         if self.time_steps <= 1:
             y = self.forward_single(x)
         else:
             y = self.forward_multiple(x, self.time_steps)
-        if self.reset_after_process:
-            self.reset()
         return y
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/layer.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/layer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,298 +1,269 @@
 # -*- coding: UTF-8 -*-
 """
 脉冲神经网络的整个神经元层，输入为脉冲，输出为脉冲。
 由突触将来自上一层神经元的脉冲信号$O_{j}^{l-1}(t)$整合成为突触后电位$X_{i}^{l}(t)$后，在胞体中进行突触后电位的累积和发放。
 """
 
 
-import math
-from typing import Optional, Union
+from typing import Tuple, Callable, Optional, Union
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t, _size_any_t
 from torch.types import _size
+from matterhorn_pytorch.snn.container import Temporal
+import matterhorn_pytorch.snn.functional as SF
 from matterhorn_pytorch.snn.skeleton import Module
 from matterhorn_pytorch.snn import surrogate
+from matterhorn_pytorch.training.functional import stdp_online
 try:
     from rich import print
 except:
     pass
 
 
-class val_to_spike(torch.autograd.Function):
-    @staticmethod
-    def forward(ctx, x: torch.Tensor) -> torch.Tensor:
-        """
-        模拟值转脉冲的前向传播函数，以0.5为界
-        @params:
-            x: torch.Tensor 模拟值
-        @return:
-            o: torch.Tensor 脉冲值（0、1）
-        """
-        return x.ge(0.5).to(x)
-    
-
-    @staticmethod
-    def backward(ctx, grad_output: torch.Tensor) -> torch.Tensor:
-        """
-        模拟值转脉冲的反向传播函数
-        @params:
-            grad_output: torch.Tensor 输出梯度
-        @return:
-            grad_input: torch.Tensor 输入梯度
-        """
-        return grad_output
-
-
-class SRM0Linear(Module):
-    def __init__(self, in_features: int, out_features: int, tau_m: float = 2.0, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: nn.Module = surrogate.Rectangular(), trainable: bool = False, device = None, dtype = None) -> None:
-        """
-        SRM0神经元，突触响应的神经元
-        电位公式较为复杂：
-        $$U_{i}(t)=η_{i}(t-t_{i})+\sum_{j}{w_{ij}\sum_{t_{j}^{(f)}}{ε_{ij}(t_{i}-t_{j}^{(f)})}}$$
-        其中复位函数
-        $$η_{i}(u)=-Θe^{-u^{m}+n}G(u)$$
-        G(u)为矩形窗，当u∈[0,1)时为+∞，否则为1。
-        突触响应函数
-        $$ε_{ij}(s)=e^{-\frac{s}{τ_{m}}}H(s)$$
-        H(s)为阶跃函数，当s>0时为1，否则为0。
-        在此将其简化为多个突触反应与一个复位反应的叠加，即
-        $$U_{i}^{l}(t)=u_{rest}+\sum_{j}{w_{ij}U_{ij}^{l}(t)}+R_{i}^{l}(t)$$
-        @params:
-            in_features: int 输入长度，用法同nn.Linear
-            out_features: int 输出长度，用法同nn.Linear
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: nn.Module 计算脉冲时所使用的阶跃函数
-            trainable: bool 参数是否可以训练
-            device: Optional[torch.device, str] 所使用的设备
-            dtype: Optional[type] 数据类型
-        """
-        super().__init__()
-        self.in_features = in_features
-        self.out_features = out_features
-        self.weight = nn.Parameter(torch.empty((out_features, in_features), device = device, dtype = dtype))
-        nn.init.kaiming_uniform_(self.weight, a = math.sqrt(5))
-        self.tau_m = nn.Parameter(torch.tensor(tau_m), requires_grad = trainable)
-        self.u_threshold = u_threshold
-        self.u_rest = u_rest
-        self.spiking_function = spiking_function
-        self.reset()
-    
-
-    def extra_repr(self) -> str:
-        """
-        额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
-        """
-        return "multi_time_step=%s, in_features=%d, out_features=%d, tau_m=%.3f, u_th=%.3f, u_rest=%.3f" % ("True" if self.multi_time_step else "False", self.in_features, self.out_features, self.tau_m, self.u_threshold, self.u_rest)
-
-
-    def reset(self) -> None:
-        """
-        重置整个神经元
-        """
-        self.s = 0.0
-        self.r = 0.0
-
-
-    def init_tensor(self, u: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        校正整个电位形状
-        @params:
-            u: torch.Tensor 待校正的电位，可能是张量或浮点值
-            x: torch.Tensor 带有正确数据类型、所在设备和形状的张量
-        @return:
-            u: torch.Tensor 经过校正的电位张量
-        """
-        if isinstance(u, float):
-            u = u * torch.ones_like(x)
-        return u
-
-
-    def f_synapse_response(self, s: torch.Tensor, o: torch.Tensor) -> torch.Tensor:
-        """
-        根据上一时刻的历史反应$S_{ij}^{l}(t-1)$与输入脉冲$O_{j}^{l-1}(t)$计算当前反应$S_{ij}^{l}(t)$。
-        该部分可用如下公式概括：
-        $$S_{ij}^{l}(t)=\frac{1}{\tau_{m}}S_{ij}^{l}(t-1)+O_{j}^{l-1}(t)$$
-        @params:
-            s: torch.Tensor 上一时刻的历史反应$S_{ij}^{l}(t-1)$
-            o: torch.Tensor 输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            s: torch.Tensor 当前反应$S_{ij}^{l}(t)$
-        """
-        s = (1.0 / self.tau_m) * s + o
-        return s
-
-
-    def f_synapse_sum(self, w: torch.Tensor, s: torch.Tensor) -> torch.Tensor:
-        """
-        根据当前反应$S_{ij}^{l}(t)$与权重$W_{ij}$求和计算当前电位$U_{i}^{l}(t)$。
-        该部分可用如下公式概括：
-        $$X_{i}^{l}(t)=\sum_{j}{w_{ij}S_{ij}^{l}(t)}$$
-        @params:
-            w: torch.Tensor 权重矩阵$W_{ij}$
-            s: torch.Tensor 当前反应$S_{ij}^{l}(t)$
-        @return:
-            o: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        """
-        u = nn.functional.linear(s, w)
-        return u
-
-
-    def f_response(self, r: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        通过上一时刻的响应$R_{i}^{l}(t)$和当前时刻的输入电位$X_{i}^{l}(t)$计算当前电位$U_{i}^{l}(t)$。
-        该部分可用如下公式概括：
-        $$U_{i}^{l}(t)=X_{i}^{l}(t)*R_{i}^{l}(t)+u_{rest}$$
-        @params:
-            r: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        """
-        u = self.u_rest + (x * r)
-        return u
-    
-
-    def f_firing(self, u: torch.Tensor) -> torch.Tensor:
-        """
-        通过当前电位$U_{i}^{l}(t)$计算当前脉冲$O_{i}^{l}(t)$。
-        该部分可用如下公式概括：
-        $$U_{i}^{l}(t)=X_{i}^{l}(t)+R_{i}^{l}(t)+u_{rest}$$
-        $$O_{i}^{l}(t)=Heaviside(U_{i}^{l}(t)-u_{th})$$
-        @params:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        @return:
-            o: torch.Tensor 当前脉冲$O_{i}^{l}(t)$
-        """
-        return self.spiking_function(u - self.u_threshold)
-
-
-    def f_reset(self, u: torch.Tensor, o: torch.Tensor) -> torch.Tensor:
-        """
-        通过上一时刻的重置电位$R_{i}^{l}(t-1)$与当前脉冲$O_{i}^{l}(t-1)$得到当前重置电位$R_{i}^{l}(t)$。
-        该部分可用如下公式概括：
-        $$R_{i}^{l}(t)=\frac{1}{\tau_{r}}R_{i}^{l}(t-1)-m(u_{th}-u_{rest})O_{i}^{l}(t-1)$$
-        此处将其改为是否产生不应期，得到：
-        $$R_{i}^{l}(t)=-(u_{th}-u_{rest})O_{i}^{l}(t-1)$$
-        @params:
-            u: torch.Tensor 上一时刻的重置电位$R_{i}^{l}(t-1)$
-            o: torch.Tensor 当前脉冲$O_{i}^{l}(t-1)$
-        @return:
-            r: torch.Tensor 当前重置电位$R_{i}^{l}(t)$
-        """
-        r = 1.0 - o
-        return r
-
-
-    def forward(self, o: torch.Tensor) -> torch.Tensor:
-        """
-        前向传播函数。
-        @params:
-            o: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            o: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
-        """
-        # 突触函数
-        # [batch_size, input_shape] -> [batch_size, output_shape]
-        self.s = self.init_tensor(self.s, o)
-        self.s = self.f_synapse_response(self.s, o)
-        x = self.f_synapse_sum(self.weight, self.s)
-
-        # 胞体函数，仍旧遵循R-S-R三段式
-        # [batch_size, output_shape] -> [batch_size, output_shape]
-        self.r = self.init_tensor(self.r, x)
-        u = self.f_response(self.r, x)
-        o = self.f_firing(u)
-        self.r = self.f_reset(u, o)
-        return o
-
-
 class Layer(Module):
     def __init__(self, multi_time_step = False) -> None:
         """
         突触函数的骨架，定义突触最基本的函数。
-        @params:
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         super().__init__(
             multi_time_step = multi_time_step
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return "multi_time_step=%s, " % ("True" if self.multi_time_step else "False")
+        return "multi_time_step=%s" % (str(self.multi_time_step),)
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$，形状为[B, ...]
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$，形状为[B, ...]
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$，形状为[B, ...]
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$，形状为[B, ...]
         """
         y = x
         return y
 
 
     def forward_multi_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         多个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$，形状为[T, B, ...]
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$，形状为[T, B, ...]
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$，形状为[T, B, ...]
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$，形状为[T, B, ...]
         """
         time_steps = x.shape[0]
         batch_size = x.shape[1]
         x = x.flatten(0, 1)
         y = self.forward_single_time_step(x)
         output_shape = [time_steps, batch_size] + list(y.shape[1:])
         y = y.reshape(output_shape)
         return y
 
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         if self.multi_time_step:
             y = self.forward_multi_time_step(x)
         else:
             y = self.forward_single_time_step(x)
-        y = val_to_spike.apply(y)
+        y = SF.val_to_spike(y)
+        return y
+
+
+class f_stdp_linear(torch.autograd.Function):
+    @staticmethod
+    def forward(ctx: torch.Any, input: torch.Tensor, weight: torch.Tensor, input_trace: torch.Tensor, output_trace: torch.Tensor, soma: Module, a_pos: float = 0.015, tau_pos: float = 2.0, a_neg: float = 0.015, tau_neg: float = 2.0, training: bool = True, multi_time_step: bool = True) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        """
+        利用STDP进行学习的液体状态机的前向传播函数。
+        Args:
+            ctx (torch.Any): 上下文
+            input (torch.Tensor): 输入脉冲序列
+            weight (torch.Tensor): 权重矩阵
+            input_trace (torch.Tensor): 输入的迹，累积的输入效应
+            output_trace (torch.Tensor): 输出的迹，累积的输出效应
+            soma (snn.Module): 胞体
+            a_pos (float): STDP参数A+
+            tau_pos (float): STDP参数tau+
+            a_neg (float): STDP参数A-
+            tau_neg (float): STDP参数tau-
+            training (bool): 是否正在训练
+            multi_time_step (bool): 是否为多时间步模式
+        Returns:
+            output (torch.Tensor): 输出脉冲序列
+            input_trace (torch.Tensor): 输入的迹，累积的输入效应
+            output_trace (torch.Tensor): 输出的迹，累积的输出效应
+        """
+        if multi_time_step:
+            input_spike_train = input.clone()
+            time_steps = input.shape[0]
+            batch_size = input.shape[1]
+            flattened_input = input.flatten(0, 1)
+            psp = F.linear(flattened_input, weight, bias = None)
+            output_shape = [time_steps, batch_size] + list(psp.shape[1:])
+            psp = psp.reshape(output_shape)
+        else:
+            input_spike_train = input[None]
+            time_steps = 1
+            batch_size = input.shape[0]
+            psp = F.linear(input, weight, bias = None)
+        output = soma(psp)
+        if multi_time_step:
+            output_spike_train = output.clone()
+        else:
+            output_spike_train = output[None]
+        delta_weight = torch.zeros_like(weight)
+        if training:
+            for t in range(time_steps):
+                delta_weight, input_trace, output_trace = stdp_online(
+                    delta_weight = delta_weight,
+                    input_trace = input_trace,
+                    output_trace = output_trace,
+                    input_spike_train = input_spike_train[t],
+                    output_spike_train = output_spike_train[t],
+                    a_pos = a_pos,
+                    tau_pos = tau_pos,
+                    a_neg = a_neg,
+                    tau_neg = tau_neg
+                )
+        ctx.save_for_backward(delta_weight, input)
+        return output, input_trace, output_trace
+
+
+    @staticmethod
+    def backward(ctx: torch.Any, grad_output: torch.Tensor, grad_input_trace: torch.Tensor, grad_output_trace: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, None, None, None, None, None, None, None]:
+        """
+        利用STDP进行学习的液体状态机的反向传播函数。
+        Args:
+            ctx (torch.Any): 上下文
+            grad_output (torch.Tensor): 输出脉冲序列梯度
+            grad_input_trace (torch.Tensor): 输入的迹梯度
+            grad_output_trace (torch.Tensor): 输出的迹梯度
+        Returns:
+            grad_input (torch.Tensor): 输入脉冲序列梯度
+            grad_weight (torch.Tensor): 权重矩阵梯度
+            grad_input_trace (torch.Tensor): 输入的迹梯度
+            grad_output_trace (torch.Tensor): 输出的迹梯度
+            grad_soma (None): 胞体的梯度，为None
+            grad_a_pos (None): STDP参数A+的梯度，为None
+            grad_tau_pos (None): STDP参数tau+的梯度，为None
+            grad_a_neg (None): STDP参数A-的梯度，为None
+            grad_tau_neg (None): STDP参数tau-的梯度，为None
+            grad_training (None): 是否正在训练的梯度，为None
+            grad_multi_time_step (None): 是否为多时间步模式的梯度，为None
+        """
+        delta_weight, input = ctx.saved_tensors
+        delta_weight = -delta_weight
+        return torch.zeros_like(input), delta_weight, torch.zeros_like(grad_input_trace), torch.zeros_like(grad_output_trace), None, None, None, None, None, None, None
+
+
+class STDPLinear(Module):
+    def __init__(self, in_features: int, out_features: int, soma: Module, a_pos: float = 0.015, tau_pos: float = 2.0, a_neg: float = 0.015, tau_neg: float = 2.0, multi_time_step: bool = True, reset_after_process: bool = True, device: torch.device = None, dtype: torch.dtype = None) -> None:
+        """
+        使用STDP学习机制时的全连接层。
+        Args:
+            in_features (int): 输入长度，用法同nn.Linear
+            out_features (int): 输出长度，用法同nn.Linear
+            soma (nn.Module): 使用的脉冲神经元胞体，在matterhorn_pytorch.snn.soma中选择
+            a_pos (float): STDP参数A+
+            tau_pos (float): STDP参数tau+
+            a_neg (float): STDP参数A-
+            tau_neg (float): STDP参数tau-
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
+        """
+        self.input_trace = None
+        self.output_trace = None
+        super().__init__(
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process
+        )
+        self.in_features = in_features
+        self.out_features = out_features
+        self.weight = nn.Parameter(torch.empty((out_features, in_features), device = device, dtype = dtype))
+        nn.init.kaiming_uniform_(self.weight, a = 5.0 ** 0.5)
+        if self.multi_time_step:
+            if soma.supports_multi_time_step():
+                self.soma = soma.multi_time_step_(True)
+            elif not soma.multi_time_step:
+                self.soma = Temporal(soma, reset_after_process = False)
+        else:
+            if soma.supports_single_time_step():
+                self.soma = soma.multi_time_step_(False)
+            else:
+                self.soma = soma
+        self.a_pos = a_pos
+        self.tau_pos = tau_pos
+        self.a_neg = a_neg
+        self.tau_neg = tau_neg
+        self.reset()
+
+
+    def reset(self) -> nn.Module:
+        """
+        重置模型。
+        """
+        self.input_trace = SF.reset_tensor(self.input_trace, 0.0)
+        self.output_trace = SF.reset_tensor(self.output_trace, 0.0)
+        return super().reset()
+
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
+        """
+        if self.multi_time_step:
+            time_steps = x.shape[0]
+            batch_size = x.shape[1]
+        else:
+            time_steps = 1
+            batch_size = x.shape[0]
+        trace_shape = torch.zeros_like(self.weight)[None].repeat_interleave(batch_size, dim = 0)
+        self.input_trace = SF.init_tensor(self.input_trace, trace_shape)
+        self.output_trace = SF.init_tensor(self.output_trace, trace_shape)
+        y, self.input_trace, self.output_trace = f_stdp_linear.apply(x, self.weight, self.input_trace, self.output_trace, self.soma, self.a_pos, self.tau_pos, self.a_neg, self.tau_neg, self.training, self.multi_time_step)
         return y
 
 
 class MaxPool1d(Layer, nn.MaxPool1d):
-    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step: bool = False) -> None:
         """
         一维最大池化。
-        @params:
-            kernel_size: _size_any_t 池化核大小
-            stride: _size_any_t | None 池化步长
-            padding: _size_any_t 边界填充的长度
-            dilation: _size_any_t 输入侧的池化步长
-            return_indices: bool 是否返回带索引的内容
-            ceil_mode: bool 是否向上取整
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_any_t): 池化核大小
+            stride (_size_any_t | None): 池化步长
+            padding (_size_any_t): 边界填充的长度
+            dilation (_size_any_t): 输入侧的池化步长
+            return_indices (bool): 是否返回带索引的内容
+            ceil_mode (bool): 是否向上取整
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.MaxPool1d.__init__(
             self,
@@ -304,44 +275,44 @@
             ceil_mode = ceil_mode
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.MaxPool1d.extra_repr(self)
+        return ", ".join([nn.MaxPool1d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.MaxPool1d.forward(self, x)
         return y
 
 
 class MaxPool2d(Layer, nn.MaxPool2d):
-    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step: bool = False) -> None:
         """
         二维最大池化。
-        @params:
-            kernel_size: _size_any_t 池化核大小
-            stride: _size_any_t | None 池化步长
-            padding: _size_any_t 边界填充的长度
-            dilation: _size_any_t 输入侧的池化步长
-            return_indices: bool 是否返回带索引的内容
-            ceil_mode: bool 是否向上取整
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_any_t): 池化核大小
+            stride (_size_any_t | None): 池化步长
+            padding (_size_any_t): 边界填充的长度
+            dilation (_size_any_t): 输入侧的池化步长
+            return_indices (bool): 是否返回带索引的内容
+            ceil_mode (bool): 是否向上取整
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.MaxPool2d.__init__(
             self,
@@ -353,44 +324,44 @@
             ceil_mode = ceil_mode
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.MaxPool2d.extra_repr(self)
+        return ", ".join([nn.MaxPool2d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.MaxPool2d.forward(self, x)
         return y
 
 
 class MaxPool3d(Layer, nn.MaxPool3d):
-    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_any_t, stride: Optional[_size_any_t] = None, padding: _size_any_t = 0, dilation: _size_any_t = 1, return_indices: bool = False, ceil_mode: bool = False, multi_time_step: bool = False) -> None:
         """
         三维最大池化。
-        @params:
-            kernel_size: _size_any_t 池化核大小
-            stride: _size_any_t | None 池化步长
-            padding: _size_any_t 边界填充的长度
-            dilation: _size_any_t 输入侧的池化步长
-            return_indices: bool 是否返回带索引的内容
-            ceil_mode: bool 是否向上取整
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_any_t): 池化核大小
+            stride (_size_any_t | None): 池化步长
+            padding (_size_any_t): 边界填充的长度
+            dilation (_size_any_t): 输入侧的池化步长
+            return_indices (bool): 是否返回带索引的内容
+            ceil_mode (bool): 是否向上取整
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.MaxPool3d.__init__(
             self,
@@ -402,43 +373,43 @@
             ceil_mode = ceil_mode
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.MaxPool3d.extra_repr(self)
+        return ", ".join([nn.MaxPool3d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.MaxPool3d.forward(self, x)
         return y
 
 
 class AvgPool1d(Layer, nn.AvgPool1d):
-    def __init__(self, kernel_size: _size_1_t, stride: _size_1_t = None, padding: _size_1_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_1_t, stride: Optional[_size_1_t] = None, padding: _size_1_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, multi_time_step: bool = False) -> None:
         """
         一维平均池化。
-        @params:
-            kernel_size: _size_1_t 池化核大小
-            stride: _size_1_t 池化核步长
-            padding: _size_1_t 边界填充的长度
-            ceil_mode: bool 是否向上取整
-            count_include_pad: bool 是否连带边界一起计算
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_1_t): 池化核大小
+            stride (_size_1_t): 池化核步长
+            padding (_size_1_t): 边界填充的长度
+            ceil_mode (bool): 是否向上取整
+            count_include_pad (bool): 是否连带边界一起计算
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.AvgPool1d.__init__(
             self,
@@ -449,44 +420,44 @@
             count_include_pad = count_include_pad
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.AvgPool1d.extra_repr(self)
+        return ", ".join([nn.AvgPool1d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.AvgPool1d.forward(self, x)
         return y
 
 
 class AvgPool2d(Layer, nn.AvgPool2d):
-    def __init__(self, kernel_size: _size_2_t, stride: Optional[_size_2_t] = None, padding: _size_2_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, divisor_override: Optional[int] = None, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_2_t, stride: Optional[_size_2_t] = None, padding: _size_2_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, divisor_override: Optional[int] = None, multi_time_step: bool = False) -> None:
         """
         二维平均池化。
-        @params:
-            kernel_size: _size_2_t 池化核大小
-            stride: _size_2_t | None 池化核步长
-            padding: _size_2_t 边界填充的长度
-            ceil_mode: bool 是否向上取整
-            count_include_pad: bool 是否连带边界一起计算
-            divisor_override: int | None 是否用某个数取代总和作为除数
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_2_t): 池化核大小
+            stride (_size_2_t | None): 池化核步长
+            padding (_size_2_t): 边界填充的长度
+            ceil_mode (bool): 是否向上取整
+            count_include_pad (bool): 是否连带边界一起计算
+            divisor_override (int | None): 是否用某个数取代总和作为除数
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.AvgPool2d.__init__(
             self,
@@ -498,44 +469,44 @@
             divisor_override = divisor_override
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.AvgPool2d.extra_repr(self)
+        return ", ".join([nn.AvgPool2d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.AvgPool2d.forward(self, x)
         return y
 
 
 class AvgPool3d(Layer, nn.AvgPool3d):
-    def __init__(self, kernel_size: _size_3_t, stride: Optional[_size_3_t] = None, padding: _size_3_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, divisor_override: Optional[int] = None, multi_time_step = False) -> None:
+    def __init__(self, kernel_size: _size_3_t, stride: Optional[_size_3_t] = None, padding: _size_3_t = 0, ceil_mode: bool = False, count_include_pad: bool = True, divisor_override: Optional[int] = None, multi_time_step: bool = False) -> None:
         """
         三维平均池化。
-        @params:
-            kernel_size: _size_3_t 池化核大小
-            stride: _size_3_t | None 池化核步长
-            padding: _size_3_t 边界填充的长度
-            ceil_mode: bool 是否向上取整
-            count_include_pad: bool 是否连带边界一起计算
-            divisor_override: int | None 是否用某个数取代总和作为除数
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            kernel_size (_size_3_t): 池化核大小
+            stride (_size_3_t | None): 池化核步长
+            padding (_size_3_t): 边界填充的长度
+            ceil_mode (bool): 是否向上取整
+            count_include_pad (bool): 是否连带边界一起计算
+            divisor_override (int | None): 是否用某个数取代总和作为除数
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.AvgPool3d.__init__(
             self,
@@ -547,105 +518,233 @@
             divisor_override = divisor_override
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.AvgPool3d.extra_repr(self)
+        return ", ".join([nn.AvgPool3d.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.AvgPool3d.forward(self, x)
         return y
 
 
 class Flatten(Layer, nn.Flatten):
-    def __init__(self, start_dim: int = 1, end_dim: int = -1, multi_time_step = False) -> None:
+    def __init__(self, start_dim: int = 2, end_dim: int = -1, multi_time_step: bool = False) -> None:
         """
         展平层。
-        @params:
-            start_dim: int 起始维度
-            end_dim: int 终止维度
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            start_dim (int): 起始维度，默认为2（除去[T, B]之后的维度）
+            end_dim (int): 终止维度
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Flatten.__init__(
             self,
-            start_dim = start_dim,
-            end_dim = end_dim
+            start_dim = max(start_dim - 1, 0) if start_dim >= 0 else start_dim,
+            end_dim = max(end_dim - 1, 0) if end_dim >= 0 else end_dim
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.Flatten.extra_repr(self)
+        return ", ".join([nn.Flatten.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.Flatten.forward(self, x)
         return y
 
 
 class Unflatten(Layer, nn.Unflatten):
-    def __init__(self, dim: Union[int, str], unflattened_size: _size, multi_time_step = False) -> None:
+    def __init__(self, dim: Union[int, str], unflattened_size: _size, multi_time_step: bool = False) -> None:
         """
         反展开层。
-        @params:
-            dim: int | str 在哪个维度反展开
+        Args:
+            dim (int | str): 在哪个维度反展开
             unflattened_size: 这个维度上的张量要反展开成什么形状
-            multi_time_step: bool 是否调整为多个时间步模式
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         Layer.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Unflatten.__init__(
             self,
-            dim = dim,
+            dim = max(dim - 1, 0) if dim >= 0 else dim,
             unflattened_size = unflattened_size
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Layer.extra_repr(self) + nn.Unflatten.extra_repr(self)
+        return ", ".join([nn.Unflatten.extra_repr(self), Layer.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 上一层脉冲$O_{j}^{l-1}(t)$
-        @return:
-            y: torch.Tensor 当前层脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
         """
         y = nn.Unflatten.forward(self, x)
+        return y
+
+
+class Dropout(Layer, nn.Dropout):
+    def __init__(self, p: float = 0.5, inplace: bool = False, multi_time_step: bool = False) -> None:
+        """
+        遗忘层。
+        Args:
+            p (float): 遗忘概率
+            inplace (bool): 是否在原有张量上改动，若为True则直接改原张量，否则新建一个张量
+            multi_time_step (bool): 是否调整为多个时间步模式
+        """
+        Layer.__init__(
+            self,
+            multi_time_step = multi_time_step
+        )
+        nn.Dropout.__init__(
+            self,
+            p = p,
+            inplace = inplace
+        )
+
+
+    def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
+        """
+        y = nn.Dropout.forward(self, x)
+        return y
+
+
+class Dropout1d(Layer, nn.Dropout1d):
+    def __init__(self, p: float = 0.5, inplace: bool = False, multi_time_step: bool = False) -> None:
+        """
+        一维遗忘层。
+        Args:
+            p (float): 遗忘概率
+            inplace (bool): 是否在原有张量上改动，若为True则直接改原张量，否则新建一个张量
+            multi_time_step (bool): 是否调整为多个时间步模式
+        """
+        Layer.__init__(
+            self,
+            multi_time_step = multi_time_step
+        )
+        nn.Dropout1d.__init__(
+            self,
+            p = p,
+            inplace = inplace
+        )
+
+
+    def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
+        """
+        y = nn.Dropout1d.forward(self, x)
+        return y
+
+
+class Dropout2d(Layer, nn.Dropout2d):
+    def __init__(self, p: float = 0.5, inplace: bool = False, multi_time_step: bool = False) -> None:
+        """
+        二维遗忘层。
+        Args:
+            p (float): 遗忘概率
+            inplace (bool): 是否在原有张量上改动，若为True则直接改原张量，否则新建一个张量
+            multi_time_step (bool): 是否调整为多个时间步模式
+        """
+        Layer.__init__(
+            self,
+            multi_time_step = multi_time_step
+        )
+        nn.Dropout2d.__init__(
+            self,
+            p = p,
+            inplace = inplace
+        )
+
+
+    def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
+        """
+        y = nn.Dropout2d.forward(self, x)
+        return y
+
+
+class Dropout3d(Layer, nn.Dropout3d):
+    def __init__(self, p: float = 0.5, inplace: bool = False, multi_time_step: bool = False) -> None:
+        """
+        三维遗忘层。
+        Args:
+            p (float): 遗忘概率
+            inplace (bool): 是否在原有张量上改动，若为True则直接改原张量，否则新建一个张量
+            multi_time_step (bool): 是否调整为多个时间步模式
+        """
+        Layer.__init__(
+            self,
+            multi_time_step = multi_time_step
+        )
+        nn.Dropout3d.__init__(
+            self,
+            p = p,
+            inplace = inplace
+        )
+
+
+    def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 上一层脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            y (torch.Tensor): 当前层脉冲$O_{i}^{l}(t)$
+        """
+        y = nn.Dropout3d.forward(self, x)
         return y
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/soma.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/soma.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,609 +3,679 @@
 脉冲神经网络神经元的胞体，一层的后半段。输入为模拟电位值，输出为脉冲。
 由突触将来自上一层神经元的脉冲信号$O_{j}^{l-1}(t)$整合成为突触后电位$X_{i}^{l}(t)$后，在胞体中进行突触后电位的累积和发放。
 """
 
 
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
+import matterhorn_pytorch.snn.functional as SF
 from matterhorn_pytorch.snn.skeleton import Module
 from matterhorn_pytorch.snn import surrogate
 from typing import Callable, Iterable
 try:
     from rich import print
 except:
     pass
 
 
 class Soma(Module):
-    def __init__(self, tau_m: float = 1.0, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable: bool = False) -> None:
+    supported_surrogate_gradients = ("Rectangular", "Polynomial", "Sigmoid", "Gaussian")
+
+
+    def __init__(self, u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         Response-Firing-Reset三段式神经元胞体骨架，分别为：
         （1）通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$；
         （2）通过当前电位$U_{i}^{l}(t)$计算当前脉冲$O_{i}^{l}(t)$；
         （3）通过当前脉冲$O_{i}^{l}(t)$重置当前电位$U_{i}^{l}(t)$。
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
-        """
-        super().__init__()
-        self.tau_m = nn.Parameter(torch.tensor(tau_m), requires_grad = trainable)
-        self.u = 0.0
-        self.u_threshold = u_threshold
-        self.u_rest = u_rest
+        Args:
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
+        """
+        self.u = None
+        super().__init__(
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process
+        )
+        self.u_threshold = nn.Parameter(torch.tensor(u_threshold, device = device, dtype = dtype), requires_grad = False)
+        self.u_rest = nn.Parameter(torch.tensor(u_rest, device = device, dtype = dtype), requires_grad = False)
         self.spiking_function = spiking_function
+        self.surrogate_str = spiking_function.__class__.__name__
+        assert self.surrogate_str in self.supported_surrogate_gradients, "Unknown surrogate gradient."
+        self.spiking_function_prototype = self.supported_surrogate_gradients.index(self.surrogate_str)
         self.hard_reset = hard_reset
-        self.trainable = trainable
+        self.reset_function_prototype = 0 if self.hard_reset else 1
         self.reset()
 
 
-    def supports_multi_time_step(self) -> bool:
-        """
-        是否支持多个时间步。
-        @return:
-            if_support: bool 是否支持多个时间步
-        """
-        return False
-
-
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return "multi_time_step=%s, trainable=%s, reset=%s, " % ("True" if self.multi_time_step else "False", "True" if self.trainable else "False", "\"hard\"" if self.hard_reset else "\"soft\"")
-
-
-    def init_tensor(self, u: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        校正整个电位形状
-        @params:
-            u: torch.Tensor 待校正的电位，可能是张量或浮点值
-            x: torch.Tensor 带有正确数据类型、所在设备和形状的张量
-        @return:
-            u: torch.Tensor 经过校正的电位张量
-        """
-        if isinstance(u, float):
-            u = torch.full_like(x, u)
-            u = u.detach().requires_grad_(True)
-        return u
+        return "multi_time_step=%s, reset=%s" % (str(self.multi_time_step), "'hard'" if self.hard_reset else "'soft'")
 
 
     def reset(self) -> None:
         """
-        重置整个神经元
+        重置整个神经元。
         """
         self.detach()
-        self.u = self.u_rest
+        self.u = SF.reset_tensor(self.u, self.u_rest)
+        return super().reset()
 
     
-    def detach(self) -> None:
+    def detach(self) -> Module:
         """
         将历史电位从计算图中分离，以停止在时间上进行反向传播。
         """
         if isinstance(self.u, torch.Tensor):
-            self.u = self.u.detach().requires_grad_(True)
+            self.u = self.u.clone().detach().requires_grad_(True)
+        return super().detach()
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
-        du = (1.0 / self.tau_m) * (-(h - self.u_rest) + x)
+        du = x
         u = h + du
         return u
 
 
     def f_firing(self, u: torch.Tensor) -> torch.Tensor:
         """
         通过当前电位$U_{i}^{l}(t)$计算当前脉冲$O_{i}^{l}(t)$。
-        @params:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        @return:
-            o: torch.Tensor 当前脉冲$O_{i}^{l}(t)$
+        Args:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 当前脉冲$O_{i}^{l}(t)$
         """
         return self.spiking_function(u - self.u_threshold)
 
 
     def f_reset(self, u: torch.Tensor, o: torch.Tensor) -> torch.Tensor:
         """
         通过当前脉冲$O_{i}^{l}(t)$重置当前电位$U_{i}^{l}(t)$。
-        @params:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t-1)$
-            o: torch.Tensor 当前脉冲$O_{i}^{l}(t-1)$
-        @return:
-            h: torch.Tensor 经过重置之后的当前电位$U_{i}^{l}(t-1)$
+        Args:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t-1)$
+            o (torch.Tensor): 当前脉冲$O_{i}^{l}(t-1)$
+        Returns:
+            h (torch.Tensor): 经过重置之后的当前电位$U_{i}^{l}(t-1)$
         """
         if self.hard_reset:
             h = u * (1.0 - o) + self.u_rest * o
         else:
             h = u - (self.u_threshold - self.u_rest) * o
         return h
 
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
+    def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
-        前向传播函数。
-        @params:
-            x: torch.Tensor 来自突触的输入电位$X_{i}^{l}(t)$
-        @return:
-            o: torch.Tensor 胞体当前的输出脉冲$O_{i}^{l}(t)$
+        单个时间步的前向传播函数。
+        Args:
+            x (torch.Tensor): 来自突触的输入电位$X_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 胞体当前的输出脉冲$O_{i}^{l}(t)$
         """
-        self.u = self.init_tensor(self.u, x)
+        self.u = SF.init_tensor(self.u, x)
         self.u = self.f_response(self.u, x)
         o = self.f_firing(self.u)
         self.u = self.f_reset(self.u, o)
         return o
-    
+
+
+    def forward_multi_time_step(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        多个时间步的前向传播函数。
+        Args:
+            x (torch.Tensor): 来自突触的输入电位$X_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 胞体当前的输出脉冲$O_{i}^{l}(t)$
+        """
+        time_steps = x.shape[0]
+        o_seq = []
+        for t in range(time_steps):
+            o_seq.append(self.forward_single_time_step(x[t]))
+        o = torch.stack(o_seq)
+        return o
+
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        前向传播函数。
+        Args:
+            x (torch.Tensor): 来自突触的输入电位$X_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 胞体当前的输出脉冲$O_{i}^{l}(t)$
+        """
+        if self.multi_time_step:
+            o = self.forward_multi_time_step(x)
+        else:
+            o = self.forward_single_time_step(x)
+        return o
+
 
 class IF(Soma):
-    def __init__(self, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True) -> None:
+    def __init__(self, u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         Integrate-and-Fire(IF)神经元。
         无泄漏过程，一阶电位变换公式为：
         $$\frac{du}{dt}=RI$$
-        @params:
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
+        Args:
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = 1.0,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
-            hard_reset = hard_reset
+            hard_reset = hard_reset,
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
     
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "u_th=%.3f, u_rest=%.3f" % (self.u_threshold, self.u_rest)
+        return ", ".join(["u_threshold=%g, u_rest=%g" % (self.u_threshold, self.u_rest), super().extra_repr()])
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
         u = h + x
         return u
 
 
 class LIF(Soma):
-    def __init__(self, tau_m: float = 2.0, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable: bool = False) -> None:
+    def __init__(self, tau_m: float = 2.0, u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         Leaky-Integrate-and-Fire(LIF)神经元。
         一阶电位变换公式为：
         $$τ\frac{du}{dt}=-(u-u_{rest})+RI$$
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            tau_m (float): 膜时间常数$τ_{m}$
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = tau_m,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
+        self.tau_m = nn.Parameter(torch.tensor(tau_m, device = device, dtype = dtype), requires_grad = trainable)
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "tau_m=%.3f, u_th=%.3f, u_rest=%.3f" % (self.tau_m, self.u_threshold, self.u_rest)
+        return ", ".join(["tau_m=%g, u_threshold=%g, u_rest=%g" % (self.tau_m, self.u_threshold, self.u_rest), super().extra_repr()])
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
         du = (1.0 / self.tau_m) * (-(h - self.u_rest) + x)
         u = h + du
         return u
 
 
 class QIF(Soma):
-    def __init__(self, tau_m: float = 2.0, u_threshold: float = 1.0, u_rest: float = 0.0, u_c: float = 0.8, a_0: float = 1.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable: bool = False) -> None:
+    def __init__(self, tau_m: float = 2.0, u_threshold: float = -0.055, u_rest: float = -0.07, u_c: float = 1.0, a_0: float = 1.0, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         Quadratic Integrate-and-Fire(QIF)神经元。
         一阶电位变换公式为：
         $$τ\frac{du}{dt}=a_{0}(u-u_{rest})(u-u_{c})+RI$$
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            u_c: float 参数$u_{c}$
-            a_0: float 参数$a_{0}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            tau_m (float): 膜时间常数$τ_{m}$
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            u_c (float): 参数$u_{c}$
+            a_0 (float): 参数$a_{0}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = tau_m,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
-        self.a_0 = nn.Parameter(torch.tensor(a_0), requires_grad = trainable)
-        self.u_c = nn.Parameter(torch.tensor(u_c), requires_grad = trainable)
+        self.tau_m = nn.Parameter(torch.tensor(tau_m, device = device, dtype = dtype), requires_grad = trainable)
+        self.a_0 = nn.Parameter(torch.tensor(a_0, device = device, dtype = dtype), requires_grad = trainable)
+        self.u_c = nn.Parameter(torch.tensor(u_c, device = device, dtype = dtype), requires_grad = trainable)
     
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "tau_m=%.3f, u_th=%.3f, u_rest=%.3f, a_0=%.3f, u_C=%.3f" % (self.tau_m, self.u_threshold, self.u_rest, self.a_0, self.u_c)
+        return ", ".join(["tau_m=%g, u_threshold=%g, u_rest=%g, a_0=%g, u_C=%g" % (self.tau_m, self.u_threshold, self.u_rest, self.a_0, self.u_c), super().extra_repr()])
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
-        du = (1.0 / self.tau_m) * (-self.a_0 * (h - self.u_rest) * (h - self.u_c) + x)
+        du = (1.0 / self.tau_m) * (self.a_0 * (h - self.u_rest) * (h - self.u_c) + x)
         u = h + du
         return u
 
 
-class EIF(Soma):
-    def __init__(self, tau_m: float = 2.0, u_threshold: float = 1.0, u_rest: float = 0.0, u_t: float = 8.0, delta_t: float = 1.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable: bool = False) -> None:
+class ExpIF(Soma):
+    def __init__(self, tau_m: float = 2.0, u_threshold: float = -0.055, u_rest: float = -0.07, u_t: float = 0.0, delta_t: float = 0.001, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
-        Exponential Integrate-and-Fire(EIF)神经元。
+        Exponential Integrate-and-Fire(ExpIF)神经元。
         一阶电位变换公式为：
         $$τ\frac{du}{dt}=-(u-u_{rest})+Δ_{T}e^{\frac{u-u_{T}}{Δ_{T}}}+RI$$
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            u_t: float 参数$u_{T}$
-            delta_t: float 参数$Δ_{T}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            tau_m (float): 膜时间常数$τ_{m}$
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            u_t (float): 参数$u_{T}$
+            delta_t (float): 参数$Δ_{T}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = tau_m,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
-        self.delta_t = nn.Parameter(torch.tensor(delta_t), requires_grad = trainable)
-        self.u_t = nn.Parameter(torch.tensor(u_t), requires_grad = trainable)
+        self.tau_m = nn.Parameter(torch.tensor(tau_m, device = device, dtype = dtype), requires_grad = trainable)
+        self.delta_t = nn.Parameter(torch.tensor(delta_t, device = device, dtype = dtype), requires_grad = trainable)
+        self.u_t = nn.Parameter(torch.tensor(u_t, device = device, dtype = dtype), requires_grad = trainable)
     
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "tau_m=%.3f, u_th=%.3f, u_rest=%.3f, u_T=%.3f, delta_T=%.3f" % (self.tau_m, self.u_threshold, self.u_rest, self.u_t, self.delta_t)
+        return ", ".join(["tau_m=%g, u_threshold=%g, u_rest=%g, u_T=%g, delta_T=%g" % (self.tau_m, self.u_threshold, self.u_rest, self.u_t, self.delta_t), super().extra_repr()])
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
         du = (1.0 / self.tau_m) * (-(h - self.u_rest) + self.delta_t * torch.exp((h - self.u_t) / self.delta_t) + x)
         u = h + du
         return u
 
 
 class Izhikevich(Soma):
-    def __init__(self, a: float = 1.0, b: float = 1.0, u_threshold: float = 1.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable = False) -> None:
-        """
+    def __init__(self, u_threshold: float = -0.055, u_rest: float = -0.07, a: float = 1.0, b: float = 1.0, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
+        """, 
         Izhikevich神经元。
         一阶电位变换公式为：
         $$\frac{du}{dt}=0.04u^{2}+5u+140-w+I$$
         $$\frac{dw}{dt}=a(bu-w)$$
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            u_t: float 参数$u_{T}$
-            delta_t: float 参数$Δ_{T}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            u_t (float): 参数$u_{T}$
+            delta_t (float): 参数$Δ_{T}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
+        self.w = None
         super().__init__(
-            tau_m = 1.0,
             u_threshold = u_threshold,
-            u_rest = 0.0,
+            u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
-        self.w = 0.0
-        self.a = nn.Parameter(torch.tensor(a), requires_grad = trainable)
-        self.b = nn.Parameter(torch.tensor(b), requires_grad = trainable)
+        self.a = nn.Parameter(torch.tensor(a, device = device, dtype = dtype), requires_grad = trainable)
+        self.b = nn.Parameter(torch.tensor(b, device = device, dtype = dtype), requires_grad = trainable)
     
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "a=%.3f, b=%.3f, u_th=%.3f" % (self.a, self.b, self.u_threshold)
+        return ", ".join(["a=%g, b=%g, u_threshold=%g" % (self.a, self.b, self.u_threshold), super().extra_repr()])
 
 
     def reset(self) -> None:
         """
         重置整个神经元
         """
         self.detach()
-        self.u = 0.0
-        self.w = 0.0
+        self.u = SF.reset_tensor(self.u, self.u_rest)
+        self.w = SF.reset_tensor(self.w, 0.0)
+        return super().reset()
 
     
     def detach(self) -> None:
         """
         将历史电位与权重从计算图中分离，以停止在时间上进行反向传播。
         """
         if isinstance(self.u, torch.Tensor):
             self.u = self.u.detach().requires_grad_(True)
         if isinstance(self.w, torch.Tensor):
             self.w = self.w.detach().requires_grad_(True)
+        return super().detach()
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
-        self.w = self.init_tensor(self.w, h)
+        self.w = SF.init_tensor(self.w, h)
         dw = self.a * (self.b * h - self.w)
         self.w = self.w + dw
-        du = 0.04 * h * h + 5.0 * h + 140.0 - self.w + x
+        du = 0.00004 * h * h + 0.005 * h + 0.14 + self.u_rest - self.w + x
         u = h + du
         return u
 
 
+class KLIF(Soma):
+    def __init__(self, tau_m: float = 2.0, u_threshold: float = 1.0, u_rest: float = 0.0, k: float = 0.2, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
+        """
+        KLIF神经元
+        Args:
+            tau_m (float): 膜时间常数$τ_{m}$
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            k (float): 参数k
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
+        """
+        super().__init__(
+            u_threshold = u_threshold,
+            u_rest = u_rest,
+            spiking_function = spiking_function,
+            hard_reset = hard_reset,
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
+        )
+        self.tau_m = nn.Parameter(torch.tensor(tau_m, device = device, dtype = dtype), requires_grad = trainable)
+        self.k = nn.Parameter(torch.tensor(k, device = device, dtype = dtype), requires_grad = trainable)
+        
+
+    def extra_repr(self) -> str:
+        """
+        额外的表达式，把参数之类的放进来。
+        Returns:
+            repr_str (str): 参数表
+        """
+        return ", ".join(["tau_m=%g, u_threshold=%g, u_rest=%g" % (self.tau_m, self.u_threshold, self.u_rest), super().extra_repr()])
+
+
+    def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
+        """
+        通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
+        """
+        du = (1.0 / self.tau_m) * (-(h - self.u_rest) + x)
+        u = h + du
+        f = F.relu(self.k * (u - self.u_rest)) + self.u_rest
+        return f
+
+
 class Response(Soma):
-    def __init__(self, response_function: Callable, param_list: Iterable = [], u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), hard_reset: bool = True, trainable: bool = False) -> None:
+    def __init__(self, response_function: Callable, param_list: Iterable = [], u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         可以自定义反应函数的胞体。
-        @params:
-            response_function: Callable 自定义的反应函数，接受3个参数：历史电位$H^{l}(t)$、输入电位$X^{l}(t)$和模型的可训练参数列表
-            param_list: Iterable 可训练参数列表的初始化值，类型都是Number。固定参数请固定地写在反应函数中
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            response_function (Callable): 自定义的反应函数，接受3个参数：历史电位$H^{l}(t)$、输入电位$X^{l}(t)$和模型的可训练参数列表
+            param_list (Iterable): 可训练参数列表的初始化值，类型都是Number。固定参数请固定地写在反应函数中
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = 1.0,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
         self.response_function = response_function
-        self.param_list = [nn.Parameter(torch.tensor(x), requires_grad = trainable) for x in param_list]
+        self.param_list = [nn.Parameter(torch.tensor(x, device = device, dtype = dtype), requires_grad = trainable) for x in param_list]
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
         return self.response_function(h, x, self.param_list)
 
 
 class AnalogSoma(Soma):
-    def __init__(self, tau_m: float = 1.0, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), activation_function: nn.Module = nn.ReLU(), hard_reset: bool = True, trainable: bool = False) -> None:
+    def __init__(self, u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), activation_function: nn.Module = nn.ReLU(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         带有模拟输出的Response-Firing-Reset三段式神经元胞体骨架，分别为：
         （1）通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$；
         （2）通过当前电位$U_{i}^{l}(t)$计算当前脉冲$O_{i}^{l}(t)$；
         （3）通过当前电位$U_{i}^{l}(t)$计算当前模拟输出$Y_{i}^{l}(t)$；
         （4）通过当前脉冲$O_{i}^{l}(t)$重置当前电位$U_{i}^{l}(t)$。
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            activation_function: nn.Module 激活函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            activation_function (nn.Module): 激活函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = tau_m,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
         self.activation_function = activation_function
     
 
     def f_activation(self, u: torch.Tensor) -> torch.Tensor:
         """
         通过当前电位$U_{i}^{l}(t)$计算当前模拟输出$Y_{i}^{l}(t)$。
-        @params:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        @return:
-            y: torch.Tensor 当前模拟输出$Y_{i}^{l}(t)$
+        Args:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
+        Returns:
+            y (torch.Tensor): 当前模拟输出$Y_{i}^{l}(t)$
         """
         return self.activation_function(u - self.u_rest)
     
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            x: torch.Tensor 来自突触的输入电位$X_{i}^{l}(t)$
-        @return:
-            o: torch.Tensor 胞体当前的输出脉冲$O_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 来自突触的输入电位$X_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 胞体当前的输出脉冲$O_{i}^{l}(t)$
         """
-        self.u = self.init_tensor(self.u, x)
+        self.u = SF.init_tensor(self.u, x)
         self.u = self.f_response(self.u, x)
         o = self.f_firing(self.u)
         y = self.f_activation(self.u)
         self.u = self.f_reset(self.u, o)
         return y
 
 
-class KLIF(AnalogSoma):
-    def __init__(self, tau_m: float = 1, u_threshold: float = 1, u_rest: float = 0, k: float = 0.2, hard_reset: bool = True, trainable: bool = False) -> None:
-        """
-        KLIF神经元
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            k: float 参数k
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
-        """
-        super().__init__(
-            tau_m = tau_m,
-            u_threshold = u_threshold,
-            u_rest = u_rest,
-            spiking_function = self.f_kspiking,
-            activation_function = self.f_kspiking,
-            hard_reset = hard_reset,
-            trainable = trainable
-        )
-        self.k = nn.Parameter(torch.tensor(k), requires_grad = trainable)
-        
-
-    def extra_repr(self) -> str:
-        """
-        额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
-        """
-        return super().extra_repr() + "tau_m=%.3f, u_th=%.3f, u_rest=%.3f" % (self.tau_m, self.u_threshold, self.u_rest)
-
-
-    def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        """
-        du = (1.0 / self.tau_m) * (-(h - self.u_rest) + x)
-        u = h + du
-        return u
-
-
-    def f_kspiking(self, u: torch.Tensor) -> torch.Tensor:
-        """
-        通过当前电位$U_{i}^{l}(t)$计算当前脉冲$O_{i}^{l}(t)$。
-        @params:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
-        @return:
-            o: torch.Tensor 当前脉冲$O_{i}^{l}(t)$
-        """
-        return nn.functional.relu(self.k * u)
-
-
 class LIAF(AnalogSoma):
-    def __init__(self, tau_m: float = 1.0, u_threshold: float = 1.0, u_rest: float = 0.0, spiking_function: Module = surrogate.Rectangular(), activation_function: nn.Module = nn.ReLU(), hard_reset: bool = True, trainable: bool = False) -> None:
+    def __init__(self, tau_m: float = 2.0, u_threshold: float = -0.055, u_rest: float = -0.07, spiking_function: Module = surrogate.Gaussian(), activation_function: nn.Module = nn.ReLU(), hard_reset: bool = True, multi_time_step: bool = False, reset_after_process: bool = True, trainable: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         Leaky Integrate-and-Analog-Fire(LIAF)神经元
-        @params:
-            tau_m: float 膜时间常数$τ_{m}$
-            u_threshold: float 阈电位$u_{th}$
-            u_rest: float 静息电位$u_{rest}$
-            spiking_function: Module 计算脉冲时所使用的阶跃函数
-            activation_function: nn.Module 激活函数
-            hard_reset: bool 是否为硬重置
-            trainable: bool 参数是否可以训练
+        Args:
+            tau_m (float): 膜时间常数$τ_{m}$
+            u_threshold (float): 阈电位$u_{th}$
+            u_rest (float): 静息电位$u_{rest}$
+            spiking_function (Module): 计算脉冲时所使用的阶跃函数
+            activation_function (nn.Module): 激活函数
+            hard_reset (bool): 是否为硬重置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            reset_after_process (bool): 是否在执行完后自动重置，若为False则需要手动重置
+            trainable (bool): 参数是否可以训练
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         super().__init__(
-            tau_m = tau_m,
             u_threshold = u_threshold,
             u_rest = u_rest,
             spiking_function = spiking_function,
             activation_function = activation_function,
             hard_reset = hard_reset,
-            trainable = trainable
+            multi_time_step = multi_time_step,
+            reset_after_process = reset_after_process,
+            device = device,
+            dtype = dtype
         )
+        self.tau_m = nn.Parameter(torch.tensor(tau_m, device = device, dtype = dtype), requires_grad = trainable)
     
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return super().extra_repr() + "tau_m=%.3f, u_th=%.3f, u_rest=%.3f" % (self.tau_m, self.u_threshold, self.u_rest)
+        return ", ".join(["tau_m=%g, u_threshold=%g, u_rest=%g" % (self.tau_m, self.u_threshold, self.u_rest), super().extra_repr()])
 
 
     def f_response(self, h: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
         """
         通过上一时刻的电位$U_{i}^{l}(t-1)$和当前时刻的输入电位$X_{i}^{l}(t)$计算电位导数$dU/dt=U_{i}^{l}(t)-U_{i}^{l}(t-1)$，进而获得当前电位$U_{i}^{l}(t)$。
-        @params:
-            h: torch.Tensor 上一时刻的电位$U_{i}^{l}(t-1)$
-            x: torch.Tensor 输入电位$X_{i}^{l}(t)$
-        @return:
-            u: torch.Tensor 当前电位$U_{i}^{l}(t)$
+        Args:
+            h (torch.Tensor): 上一时刻的电位$U_{i}^{l}(t-1)$
+            x (torch.Tensor): 输入电位$X_{i}^{l}(t)$
+        Returns:
+            u (torch.Tensor): 当前电位$U_{i}^{l}(t)$
         """
         du = (1.0 / self.tau_m) * (-(h - self.u_rest) + x)
         u = h + du
         return u
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch/snn/synapse.py` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch/snn/synapse.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,86 +17,86 @@
     pass
 
 
 class Synapse(Module):
     def __init__(self, multi_time_step = False) -> None:
         """
         突触函数的骨架，定义突触最基本的函数。
-        @params:
-            multi_time_step: bool 是否调整为多个时间步模式
+        Args:
+            multi_time_step (bool): 是否调整为多个时间步模式
         """
         super().__init__(
             multi_time_step = multi_time_step
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return "multi_time_step=%s, " % ("True" if self.multi_time_step else "False")
+        return "multi_time_step=%s" % (str(self.multi_time_step),)
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$，形状为[B, ...]
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$，形状为[B, ...]
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$，形状为[B, ...]
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$，形状为[B, ...]
         """
         x = o
         return x
 
 
     def forward_multi_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         多个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$，形状为[T, B, ...]
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$，形状为[T, B, ...]
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$，形状为[T, B, ...]
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$，形状为[T, B, ...]
         """
         time_steps = o.shape[0]
         batch_size = o.shape[1]
         o = o.flatten(0, 1)
         x = self.forward_single_time_step(o)
         output_shape = [time_steps, batch_size] + list(x.shape[1:])
         x = x.reshape(output_shape)
         return x
 
 
     def forward(self, o: torch.Tensor) -> torch.Tensor:
         """
         前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         if self.multi_time_step:
             x = self.forward_multi_time_step(o)
         else:
             x = self.forward_single_time_step(o)
         return x
 
 
 class Linear(Synapse, nn.Linear):
-    def __init__(self, in_features: int, out_features: int, bias: bool = True, multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_features: int, out_features: int, bias: bool = True, multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         全连接操作，输入一个大小为[B, L_{in}]的张量，输出一个大小为[B, L_{out}]的张量。
-        @params:
+        Args:
             in_features: 输入的长度L_{in}
             out_features: 输出的长度L_{out}
-            bias: bool 是否要加入偏置
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+            bias (bool): 是否要加入偏置
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Linear.__init__(
             self,
@@ -107,49 +107,49 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.Linear.extra_repr(self)
+        return ", ".join([nn.Linear.extra_repr(self), Synapse.extra_repr(self)])
 
     
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.Linear.forward(self, o)
         return x
 
 
 class Conv1d(Synapse, nn.Conv1d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_1_t, stride: _size_1_t = 1, padding: Union[_size_1_t, str] = 0, dilation: _size_1_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_1_t, stride: _size_1_t = 1, padding: Union[_size_1_t, str] = 0, dilation: _size_1_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         一维卷积操作，输入一个大小为[B, C_{in}, L_{in}]的张量，输出一个大小为[B, C_{out}, L_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_1_t 卷积核的形状
-            stride: _size_1_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_1_t | str 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            dilation: _size_1_t 卷积的输入步长
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_1_t): 卷积核的形状
+            stride (_size_1_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_1_t | str): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            dilation (_size_1_t): 卷积的输入步长
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Conv1d.__init__(
             self,
@@ -166,49 +166,49 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.Conv1d.extra_repr(self)
+        return ", ".join([nn.Conv1d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.Conv1d.forward(self, o)
         return x
 
 
 class Conv2d(Synapse, nn.Conv2d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_2_t, stride: _size_2_t = 1, padding: Union[_size_2_t, str] = 0, dilation: _size_2_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_2_t, stride: _size_2_t = 1, padding: Union[_size_2_t, str] = 0, dilation: _size_2_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         二维卷积操作，输入一个大小为[B, C_{in}, H_{in}, W_{in}]的张量，输出一个大小为[B, C_{out}, H_{out}, W_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_2_t 卷积核的形状
-            stride: _size_2_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_2_t | str 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            dilation: _size_2_t 卷积的输入步长
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_2_t): 卷积核的形状
+            stride (_size_2_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_2_t | str): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            dilation (_size_2_t): 卷积的输入步长
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Conv2d.__init__(
             self,
@@ -225,49 +225,49 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.Conv2d.extra_repr(self)
+        return ", ".join([nn.Conv2d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.Conv2d.forward(self, o)
         return x
 
 
 class Conv3d(Synapse, nn.Conv3d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_3_t, stride: _size_3_t = 1, padding: Union[_size_3_t, str] = 0, dilation: _size_3_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_3_t, stride: _size_3_t = 1, padding: Union[_size_3_t, str] = 0, dilation: _size_3_t = 1, groups: int = 1, bias: bool = True, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         三维卷积操作，输入一个大小为[B, C_{in}, H_{in}, W_{in}, L_{in}]的张量，输出一个大小为[B, C_{out}, H_{out}, W_{out}, L_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_3_t 卷积核的形状
-            stride: _size_3_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_3_t | str 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            dilation: _size_3_t 卷积的输入步长
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_3_t): 卷积核的形状
+            stride (_size_3_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_3_t | str): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            dilation (_size_3_t): 卷积的输入步长
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.Conv3d.__init__(
             self,
@@ -284,50 +284,50 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.Conv3d.extra_repr(self)
+        return ", ".join([nn.Conv3d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.Conv3d.forward(self, o)
         return x
 
 
 class ConvTranspose1d(Synapse, nn.ConvTranspose1d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_1_t, stride: _size_1_t = 1, padding: _size_1_t = 0, output_padding: _size_1_t = 0, groups: int = 1, bias: bool = True, dilation: _size_1_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_1_t, stride: _size_1_t = 1, padding: _size_1_t = 0, output_padding: _size_1_t = 0, groups: int = 1, bias: bool = True, dilation: _size_1_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         一维逆卷积操作，输入一个大小为[B, C_{in}, L_{in}]的张量，输出一个大小为[B, C_{out}, L_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_1_t 卷积核的形状
-            stride: _size_1_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_1_t 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            output_padding: _size_1_t 在输出边缘填充的量
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            dilation: _size_1_t 卷积的输出步长
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_1_t): 卷积核的形状
+            stride (_size_1_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_1_t): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            output_padding (_size_1_t): 在输出边缘填充的量
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            dilation (_size_1_t): 卷积的输出步长
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.ConvTranspose1d.__init__(
             self,
@@ -345,50 +345,50 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.ConvTranspose1d.extra_repr(self)
+        return ", ".join([nn.ConvTranspose1d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.ConvTranspose1d.forward(self, o)
         return x
 
 
 class ConvTranspose2d(Synapse, nn.ConvTranspose2d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_2_t, stride: _size_2_t = 1, padding: _size_2_t = 0, output_padding: _size_2_t = 0, groups: int = 1, bias: bool = True, dilation: _size_2_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_2_t, stride: _size_2_t = 1, padding: _size_2_t = 0, output_padding: _size_2_t = 0, groups: int = 1, bias: bool = True, dilation: _size_2_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         二维逆卷积操作，输入一个大小为[B, C_{in}, H_{in}, W_{in}]的张量，输出一个大小为[B, C_{out}, H_{out}, W_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_2_t 卷积核的形状
-            stride: _size_2_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_2_t 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            output_padding: _size_2_t 在输出边缘填充的量
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            dilation: _size_2_t 卷积的输出步长
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_2_t): 卷积核的形状
+            stride (_size_2_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_2_t): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            output_padding (_size_2_t): 在输出边缘填充的量
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            dilation (_size_2_t): 卷积的输出步长
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.ConvTranspose2d.__init__(
             self,
@@ -406,50 +406,50 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.ConvTranspose2d.extra_repr(self)
+        return ", ".join([nn.ConvTranspose2d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.ConvTranspose2d.forward(self, o)
         return x
 
 
 class ConvTranspose3d(Synapse, nn.ConvTranspose3d):
-    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_3_t, stride: _size_3_t = 1, padding: _size_3_t = 0, output_padding: _size_3_t = 0, groups: int = 1, bias: bool = True, dilation: _size_3_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: _size_3_t, stride: _size_3_t = 1, padding: _size_3_t = 0, output_padding: _size_3_t = 0, groups: int = 1, bias: bool = True, dilation: _size_3_t = 1, padding_mode: str = "zeros", multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         三维逆卷积操作，输入一个大小为[B, C_{in}, H_{in}, W_{in}, L_{in}]的张量，输出一个大小为[B, C_{out}, H_{out}, W_{out}, L_{out}]的张量。
-        @params:
-            in_channels: int 输入的频道数C_{in}
-            out_channels: int 输出的频道C_{out}
-            kernel_size: _size_3_t 卷积核的形状
-            stride: _size_3_t 卷积的输出步长，决定卷积输出的形状
-            padding: _size_3_t 在边缘填充的量（一般为卷积核大小的一半，向下取整）
-            output_padding: _size_3_t 在输出边缘填充的量
-            groups: int 分组进行卷积操作的组数
-            bias: bool 是否要加入偏置
-            dilation: _size_3_t 卷积的输出步长
-            padding_mode: str 边缘填充的方式
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            in_channels (int): 输入的频道数C_{in}
+            out_channels (int): 输出的频道C_{out}
+            kernel_size (_size_3_t): 卷积核的形状
+            stride (_size_3_t): 卷积的输出步长，决定卷积输出的形状
+            padding (_size_3_t): 在边缘填充的量（一般为卷积核大小的一半，向下取整）
+            output_padding (_size_3_t): 在输出边缘填充的量
+            groups (int): 分组进行卷积操作的组数
+            bias (bool): 是否要加入偏置
+            dilation (_size_3_t): 卷积的输出步长
+            padding_mode (str): 边缘填充的方式
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.ConvTranspose3d.__init__(
             self,
@@ -467,45 +467,45 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.ConvTranspose3d.extra_repr(self)
+        return ", ".join([nn.ConvTranspose3d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            o: torch.Tensor 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            o (torch.Tensor): 来自上一层的输入脉冲$O_{j}^{l-1}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.ConvTranspose3d.forward(self, o)
         return x
 
 
 class BatchNorm1d(Synapse, nn.BatchNorm1d):
-    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         一维批归一化。
-        @params:
-            num_features: int 需要被归一化那一维度的长度
-            eps: float 参数epsilon
-            momentum: float 动量参数
-            affine: bool 是否启用参数gamma和beta，进行仿射变换
-            track_running_stats: bool 是否需要跟踪整个训练过程来进行批归一化的学习
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            num_features (int): 需要被归一化那一维度的长度
+            eps (float): 参数epsilon
+            momentum (float): 动量参数
+            affine (bool): 是否启用参数gamma和beta，进行仿射变换
+            track_running_stats (bool): 是否需要跟踪整个训练过程来进行批归一化的学习
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.BatchNorm1d.__init__(
             self,
@@ -518,45 +518,45 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.BatchNorm1d.extra_repr(self)
+        return ", ".join([nn.BatchNorm1d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.BatchNorm1d.forward(self, x)
         return x
 
 
 class BatchNorm2d(Synapse, nn.BatchNorm2d):
-    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         二维批归一化。
-        @params:
-            num_features: int 需要被归一化那一维度的长度
-            eps: float 参数epsilon
-            momentum: float 动量参数
-            affine: bool 是否启用参数gamma和beta，进行仿射变换
-            track_running_stats: bool 是否需要跟踪整个训练过程来进行批归一化的学习
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            num_features (int): 需要被归一化那一维度的长度
+            eps (float): 参数epsilon
+            momentum (float): 动量参数
+            affine (bool): 是否启用参数gamma和beta，进行仿射变换
+            track_running_stats (bool): 是否需要跟踪整个训练过程来进行批归一化的学习
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.BatchNorm2d.__init__(
             self,
@@ -569,45 +569,45 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.BatchNorm2d.extra_repr(self)
+        return ", ".join([nn.BatchNorm2d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.BatchNorm2d.forward(self, x)
         return x
 
 
 class BatchNorm3d(Synapse, nn.BatchNorm3d):
-    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, num_features: int, eps: float = 0.00001, momentum: float = 0.1, affine: bool = True, track_running_stats: bool = True, multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         三维批归一化。
-        @params:
-            num_features: int 需要被归一化那一维度的长度
-            eps: float 参数epsilon
-            momentum: float 动量参数
-            affine: bool 是否启用参数gamma和beta，进行仿射变换
-            track_running_stats: bool 是否需要跟踪整个训练过程来进行批归一化的学习
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            num_features (int): 需要被归一化那一维度的长度
+            eps (float): 参数epsilon
+            momentum (float): 动量参数
+            affine (bool): 是否启用参数gamma和beta，进行仿射变换
+            track_running_stats (bool): 是否需要跟踪整个训练过程来进行批归一化的学习
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.BatchNorm3d.__init__(
             self,
@@ -620,43 +620,43 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.BatchNorm3d.extra_repr(self)
+        return ", ".join([nn.BatchNorm3d.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.BatchNorm3d.forward(self, x)
         return x
 
 
 class LayerNorm(Synapse, nn.LayerNorm):
-    def __init__(self, normalized_shape: _shape_t, eps: float = 0.00001, elementwise_affine: bool = True, multi_time_step: bool = False, device = None, dtype = None) -> None:
+    def __init__(self, normalized_shape: _shape_t, eps: float = 0.00001, elementwise_affine: bool = True, multi_time_step: bool = False, device: torch.device = None, dtype: torch.dtype = None) -> None:
         """
         数据归一化。
-        @params:
-            normalized_shape: _shape_t 在什么数据尺度上进行归一化
-            eps: float 参数epsilon
-            elementwise_affine: bool 是否启用参数gamma和beta，进行仿射变换
-            multi_time_step: bool 是否调整为多个时间步模式
-            device: torch.device 所计算的设备
-            dtype: 所计算的数据类型
+        Args:
+            normalized_shape (_shape_t): 在什么数据尺度上进行归一化
+            eps (float): 参数epsilon
+            elementwise_affine (bool): 是否启用参数gamma和beta，进行仿射变换
+            multi_time_step (bool): 是否调整为多个时间步模式
+            device (torch.device): 所计算的设备
+            dtype (torch.dtype): 所计算的数据类型
         """
         Synapse.__init__(
             self,
             multi_time_step = multi_time_step
         )
         nn.LayerNorm.__init__(
             self,
@@ -667,23 +667,51 @@
             dtype = dtype
         )
 
 
     def extra_repr(self) -> str:
         """
         额外的表达式，把参数之类的放进来。
-        @return:
-            repr_str: str 参数表
+        Returns:
+            repr_str (str): 参数表
         """
-        return Synapse.extra_repr(self) + nn.LayerNorm.extra_repr(self)
+        return ", ".join([nn.LayerNorm.extra_repr(self), Synapse.extra_repr(self)])
 
 
     def forward_single_time_step(self, x: torch.Tensor) -> torch.Tensor:
         """
         单个时间步的前向传播函数。
-        @params:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
-        @return:
-            x: torch.Tensor 突触的突触后电位$X_{i}^{l}(t)$
+        Args:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
+        Returns:
+            x (torch.Tensor): 突触的突触后电位$X_{i}^{l}(t)$
         """
         x = nn.LayerNorm.forward(self, x)
-        return x
+        return x
+
+
+class Neurotransmitter(Synapse):
+    def __init__(self, mask: torch.Tensor, multi_time_step = False) -> None:
+        """
+        神经递质，分为兴奋性神经递质和抑制性神经递质，加在胞体后面。
+        Args:
+            mask (torch.Tensor): 一个布尔类型的张量，形状与单个时间步内的数据张量一致，元素为True代表兴奋性神经元，为False代表抑制性神经元
+            multi_time_step (bool): 是否调整为多个时间步模式
+        """
+        super().__init__(
+            multi_time_step = multi_time_step
+        )
+        self.mask = mask
+    
+
+    def forward_single_time_step(self, o: torch.Tensor) -> torch.Tensor:
+        """
+        单个时间步的前向传播函数。
+        Args:
+            o (torch.Tensor): 当前层的输出脉冲$O_{i}^{l}(t)$
+        Returns:
+            o (torch.Tensor): 当前层的输出脉冲$O_{i}^{l}(t)$
+        """
+        o = torch.abs(o)
+        mask = self.mask.to(torch.bool).to(o.device)
+        o = torch.where(mask, o, -o)
+        return o
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/PKG-INFO` & `matterhorn_pytorch-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,96 @@
 Metadata-Version: 2.1
-Name: matterhorn-pytorch
-Version: 1.0.1
-Summary: Matterhorn is a neo general SNN framework based on PyTorch.
-Home-page: https://github.com/AmperiaWang/Matterhorn
+Name: matterhorn_pytorch
+Version: 1.2.0
+Summary: Matterhorn is a novel general neuromorphic computing framework based on PyTorch.
+Home-page: https://github.com/xjtuiair-cag/Matterhorn
 Author: CAG, IAIR, XJTU, Xi'an, China
 Author-email: ericwang017@stu.xjtu.edu.cn
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: numba
 Requires-Dist: h5py
 Requires-Dist: tqdm
 Requires-Dist: rich
 Requires-Dist: torch
 Requires-Dist: torchvision
+Requires-Dist: pyecharts
 
 # Matterhorn
 
+[Technical Documentation](./docs/en_us/README.md)
+
+[English](./README.md)
+
+[中文](./README_zh_cn.md)
+
 ## 1 General Introduction
 
 ![logo](./assets/logo.png)
 
-Matterhorn is a neo general SNN framework based on PyTorch.
+Matterhorn is a novel general neuromorphic computing framework based on PyTorch.
 
 ## 2 Installation
 
+This is the brief one, for complete version you can refer to [the tutorial of Matterhorn's installation](./docs/en_us/1_install.md).
+
 ### Environment
 
-Python(>=3.7.0)
+Python (>= 3.7 and <= 3.9)
+
+CUDA (>= 11.3.0, with CUDNN, optional)
 
-CUDA(>=11.3.0, with CUDNN)
+PyTorch (>= 1.10.0 and <= 1.13.1)
 
-PyTorch(>=1.10.0 and <=1.13.1)
+TorchVision (>= 0.11.0 and <= 0.13.1)
 
-TorchVision(>=0.11.0 and <= 0.13.1)
+### Requirement Installation
 
-### Environment Installation
+For Windows version you may have to install GCC as well as G++ through Visual Studio (build tools) and [MinGW](./mingw-get-setup.exe).
 
-To install PyTorch you can find the command on [https://pytorch.org/get-started/previous-versions/](https://pytorch.org/get-started/previous-versions/).
+Then execute:
 
 ```sh
-pip install numpy matplotlib numba h5py tqdm rich torch torchvision
+git clone https://github.com/xjtuiair-cag/Matterhorn.git
+cd Matterhorn
+pip install -r requirements.txt
 ```
 
+Don't forget to add `sudo` prefix if you are not the root user.
+
 ### Install Matterhorn
 
 ```sh
-git clone https://github.com/AmperiaWang/Matterhorn.git
+git clone https://github.com/xjtuiair-cag/Matterhorn.git
 cd Matterhorn
-python3 setup.py install
+python3 setup.py develop
 ```
 
 Don't forget to add `sudo` if you are not the root user.
 
 ## 3 Module Explanation
 
-### Neurons in SNN
+For the references on specialized variables, functions or modules of SNNs, you can refer to [the detailed version of the document](./docs/en_us/snn/README.md).
+
+### Terms
+
+ANNs - Artificial Neural Networks
 
-As we're all known, the image below describes what an ANN looks like.
+SNNs - Spiking Neural Networks
 
-![ANN Structure](./assets/readme_1.png)
+### Neurons in SNNs
+
+As we're all known, the image below describes what ANNs look like.
+
+![ANNs' Structure](./assets/readme_1.png)
 
 **Operation 1** is **synapse function**, which uses weights and bias to calculate those values from previous layer to current layer. Commonly used synapse functions are including full connection layer `nn.Linear`, convolution layer `nn.Conv2D`, etc.
 
 We use an equation to describe the synapse function:
 
 $$Y^{l}=synapse(X^{l-1})$$
 
@@ -76,56 +98,56 @@
 
 **Operation 2** is **activation function**, which filters information from synapses and sends the filtered information to next layer. Commonly used activation functions are including `nn.ReLU`, `nn.Sigmoid`, etc.
 
 We use an equation to describe the activation function:
 
 $$X^{l}=activation(Y^{l})$$
 
-In conclusion, each of layers in ANN has 2 functions. We can build our ANN model in PyTorch by the code below:
+In conclusion, each of layers in ANNs has 2 functions. We can build our ANN model in PyTorch by the code below:
 
 ```python
 import torch.nn as nn
 
 model = nn.Sequential(
     nn.Linear(28 * 28, 10),
     nn.ReLU()
 )
 ```
 
-This is a 1-layer MLP. It can take an image with the size of 28x28 as input and classify it into 10 classes. In this example, two equations of ANN can be represented as below:
+This is a 1-layer MLP. It can take an image with the size of 28x28 as input and classify it into 10 classes. In this example, two equations of ANNs can be represented as below:
 
 $$Y^{l}=W^{l}X^{l-1}+\vec{b}$$
 
 $$X^{l}=ReLU(Y^{l})$$
 
-In SNN, the synapse equation is the same as that in ANN. However, functions in soma are no longer like what is in ANN. In the soma of SNN, there exists a loop in time. The image below describes what an SNN looks like.
+In SNNs, the synapse equation is the same as that in ANNs. However, functions in soma are no longer like what is in ANNs. In the soma of SNNs, there exists a loop in time. The image below describes what SNNs look like.
 
 ![SNN Structure](./assets/readme_2.png)
 
 **Operation 1**, the **synapse function**, calculates spikes from previous layer $O^{l-1}(t)$ thus generates the input potential $X^{l}(t)$.
 
 We use an equation to describe the synapse function:
 
 $$X^{l}(t)=synapse(O^{l-1}(t))$$
 
 By **operation 2**, the input potential, with the history potential, is calculated based on a 1-order differential equation, thus generating the soma potential $U^{l}(t)$. We name it **response function**.
 
 We use an equation to describe the response function:
 
-$$U^{l}(t)=response(H^{l}(t),X^{l}(t))$$
+$$U^{l}(t)=response(H^{l}(t-1),X^{l}(t))$$
 
 Each spiking neuron model has its unique response differential equation.
 
 For example, in a LIF neuron:
 
 $$\tau \frac{du}{dt}=-(u-u_{rest})+RI$$
 
 Discretizing it into a difference equation, we can get:
 
-$$U^{l}(t)=(1-\frac{1}{\tau})H^{l}(t)+\frac{1}{\tau}u_{rest}+X^{l}(t)$$
+$$U^{l}(t)-H^{l}(t-1)=\frac{1}{\tau}[-[H^{l}(t-1)-u_{rest}]+X^{l}(t)]$$
 
 **Operation 3** uses Heaviside step function and threshold potential $u_{th}$ to decide whether to generate spikes $O^{l}(t)$. We name it **firing function**.
 
 We use an equation to describe the firing function:
 
 $$O^{l}(t)=spiking(U^{l}(t))$$
 
@@ -135,43 +157,43 @@
 
 Where Heaviside step function returns 1 when input is greater than or equal to 0, returns 0 otherwise.
 
 The aim of **operation 4** is to set refractory time on neurons by output spikes $O^{l}(t)$. We name it **reset function**.
 
 We use an equation to describe reset function:
 
-$$H^{l}(t)=reset(U^{l}(t-1),O^{l}(t-1))$$
+$$H^{l}(t)=reset(U^{l}(t),O^{l}(t))$$
 
 Under most occasions we use equation below to reset potential:
 
-$$H^{l}(t)=U^{l}(t-1)[1-O^{l}(t-1)]+u_{rest}O^{l}(t-1)$$
+$$H^{l}(t)=U^{l}(t)[1-O^{l}(t)]+u_{rest}O^{l}(t)$$
 
-In brief, we use 4 equations to describe SNN neurons. This is what an SNN looks like. The shape of an SNN neuron is like a trumpet. Its synapses transform those spikes from last neuron and pass the input response to soma, in which there is a time loop awaits.
+In brief, we use 4 equations to describe spiking neurons. This is what SNN look like. The shape of a spiking neuron is like a trumpet. Its synapses transform those spikes from last neuron and pass the input response to soma, in which there is a time loop awaits.
 
-By unfolding SNN neurons on temporal dimension, we can get the spatial-temporal topology network of SNN.
+By unfolding spiking neurons on temporal dimension, we can get the spatio-temporal topology network of SNNs.
 
-![Spatial-temporal Topology Network of SNN](./assets/readme_3.png)
+![Spatial-temporal Topology Network of SNNs](./assets/readme_3.png)
 
-Like building ANN in PyTorch, we can build our SNN model in Matterhorn by the code below:
+Like building ANNs in PyTorch, we can build our SNN model in Matterhorn by the code below:
 
 ```python
 import torch
 import matterhorn_pytorch.snn as snn
 
 snn_model = snn.Temporal(
     snn.Spatial(
         snn.Linear(28 * 28, 10),
         snn.LIF()
     )
 )
 ```
 
-In the code, `Spatial` is one of Matterhorn's containers to represent sequential SNN layers on spatial dimension, and `Temporal` is another Matterhorn's container to repeat calculating potential and spikes on temporal dimension. By using `Spatial` and `Temporal`, an SNN spatial-temporal topology network is built and thus used for training and evaluating.
+In the code, `Spatial` is one of Matterhorn's containers to represent sequential SNN layers on spatial dimension, and `Temporal` is another Matterhorn's container to repeat calculating potential and spikes on temporal dimension. By using `Spatial` and `Temporal`, an spatio-temporal topology network is built and thus used for training and evaluating.
 
-The built network takes an $n+1$ dimensional `torch.Tensor` as input spike train. It will take the first dimension as time steps, thus calculating through each time step. after that, it will generate a `torch.Tensor` as output spike train, just like what an ANN takes and generates in PyTorch. The only difference, which is also a key point, is that we should encode our information into spike train and decode the output spike train.
+The built network takes an $n+1$ dimensional `torch.Tensor` as input spike train. It will take the first dimension as time steps, thus calculating through each time step. after that, it will generate a `torch.Tensor` as output spike train, just like what ANNs takes and generates in PyTorch. The only difference, which is also a key point, is that we should encode our information into spike train and decode the output spike train.
 
 ### Encoding and Decoding
 
 A spike train is a set of Dirac impulse functions on the axis of time.
 
 $$O(t)=\sum_{t_{i}}δ(t-t_{i})$$
 
@@ -222,17 +244,17 @@
 ```python
 import torch
 import matterhorn_pytorch.snn as snn
 
 decoder = snn.AvgSpikeDecoder()
 ```
 
-It will take first dimension as temporal dimension, and generate statistical results as output. The output can be transported into ANN for further processes.
+It will take first dimension as temporal dimension, and generate statistical results as output. The output can be transported into ANNs for further processes.
 
-Matterhorn provides a convenient container `matterhorn.snn.Sequential` to connect all your SNN and ANN models.
+Matterhorn provides a convenient container `matterhorn_pytorch.snn.Sequential` to connect all your SNN and ANN models.
 
 ```python
 import torch
 import matterhorn_pytorch.snn as snn
 
 model = snn.Sequential(
     snn.PoissonEncoder(
@@ -241,48 +263,19 @@
     snn.Flatten(),
     snn.Linear(28 * 28, 10, bias = False),
     snn.LIF(tau_m = tau, trainable = True),
     snn.AvgSpikeDecoder()
 )
 ```
 
-By now, you have experienced what an SNN looks like and how to build it by Matterhorn. For further experience, you can refer to [examples/2_layer_mlp.py](./examples/2_layer_mlp.py).
+By now, you have experienced what SNNs look like and how to build it by Matterhorn. For further experience, you can refer to [examples/1_starting.py](./examples/1_starting.py).
 
 ```sh
 cd Matterhorn
-python3 examples/2_layer_mlp.py
-```
-
-In most cases, neurons of SNNs can be divided into 1 synapse operation and 3 soma operations. However, there are always some special cases. SRM0 neuron model is one of them, whose response is calculated in each synapse. We can use 5 operations to represent SRM0 neurons, 2 for synapses and 3 for soma:
-
-**Operation 1**: **synapse response function**
-
-$$R_{j}^{l}(t)=(1-\frac{1}{\tau_{m}})R_{j}^{l}(t-1)+O_{j}^{l}(t)$$
-
-**Operation 2**: **synapse function**
-
-$$X_{i}^{l}(t)=\sum_{j}{w_{ij}R_{j}^{l}(t)}$$
-
-**Operation 3**: **response function**
-
-$$U_{i}^{l}(t)=X_{i}^{l}(t)H_{i}^{l}(t)$$
-
-**Operation 4**: **firing function**
-
-$$O_{i}^{l}(t)=Heaviside(U_{i}^{l}(t))$$
-
-**Operation 5**: **reset function**
-
-$$H_{i}^{l}(t)=1-O_{i}^{l}(t-1)$$
-
-With 5 operations resembled we can build a SRM0 neuron. For further experience, you can refer to [examples/2_layer_mlp_with_SRM0.py](./examples/2_layer_mlp_with_SRM0.py).
-
-```sh
-cd Matterhorn
-python3 examples/2_layer_mlp_with_SRM0.py
+python3 examples/1_starting.py
 ```
 
 ### Why Should We Need Surrogate Gradient
 
 In spiking neurons, we usually use Heaviside step function $u(t)$ to decide whether to generate a spike:
 
 $$O^{l}(t)=u(U^{l}(t)-u_{th})$$
@@ -295,73 +288,76 @@
 
 One of the most common surrogate gradients is rectangular function. It is a positive constant when absolute value of x is small enough, and 0 otherwise.
 
 ![Use rectangular function as surrogate gradient](./assets/readme_5.png)
 
 Also, functions suitable for surrogate gradient include the derivative of sigmoidal function, Gaussian function, etc.
 
-You can inspect all provided surrogate gradient functions in `matterhorn.snn.surrogate`.
+You can inspect all provided surrogate gradient functions in `matterhorn_pytorch.snn.surrogate`.
 
 ### Learning: BPTT Vs. STDP
 
-Training SNNs could be as easy as training ANNs after gradient problem of Heaviside step function is solved. After we unfold SNNs into a spatial-temporal network, backpropagation through time (BPTT) could be used in SNNs. On spatial dimension, gradients can be propagated through firing function and synapse function, thus neurons of previous layer would receive the gradient; On temporal dimension, the gradient of the next time step can be propagated through firing function and response function, thus soma of previous time would receive the gradient.
+Training SNNs could be as easy as training ANNs after gradient problem of Heaviside step function is solved. After we unfold SNNs into a spatio-temporal network, backpropagation through time (BPTT) could be used in SNNs. On spatial dimension, gradients can be propagated through firing function and synapse function, thus neurons of previous layer would receive the gradient; On temporal dimension, the gradient of the next time step can be propagated through firing function and response function, thus soma of previous time would receive the gradient.
 
 ![BPTT](./assets/readme_6.png)
 
 Besides BPTT, there is another simple way to train locally in each neuron without supervision, which we call spike-timing-dependent plasticity (STDP). STDP uses precise time differences between input and output spikes to calculate the weight increment.
 
 STDP follows equation below:
 
 $$Δw_{ij}=\sum_{t_{j}}{\sum_{t_{i}}W(t_{i}-t_{j})}$$
 
 where the weight function $W(x)$ is:
 
 $$
 W(x)=
-\left \{
 \begin{aligned}
 A_{+}e^{-\frac{x}{τ_{+}}},x>0 \\\\
 0,x=0 \\\\
 -A_{-}e^{\frac{x}{τ_{-}}},x<0
 \end{aligned}
-\right \}.
 $$
 
 ![STDP function](./assets/readme_7.png)
 
-By setting parameters $A_{+}$, $τ_{+}$, $A_{-}$ and $τ_{-}$, we can easily train SNNs unsupervised. For further experience, you can refer to [examples/2_layer_mlp_with_stdp.py](./examples/2_layer_mlp_with_stdp.py).
+By setting parameters $A_{+}$, $τ_{+}$, $A_{-}$ and $τ_{-}$, we can easily train SNNs unsupervised. For further experience, you can refer to [examples/2_using_stdp.py](./examples/2_using_stdp.py).
 
 ```sh
 cd Matterhorn
-python3 examples/2_layer_mlp_with_stdp.py
+python3 examples/2_using_stdp.py
 ```
 
 **Note:** Please make sure you have installed `matterhorn_cpp_extensions` (or `matterhorn_cuda_extensions` if you have CUDA), otherwise it will be extremely slow.
 
 ```sh
 cd matterhorn_cpp_extensions
-python3 setup.py install
+python3 setup.py develop
 ```
 
 if you have CUDA, you can install CUDA version:
 
 ```sh
 cd matterhorn_cuda_extensions
-python3 setup.py install
+python3 setup.py develop
 ```
 
 ### Neuromorphic Datasets
 
-Matterhorn provides several neuromorphic datasets for training spiking neural networks.
+Matterhorn provides several neuromorphic datasets for training SNNs. You can experience provided neuromorphic dataset in Matterhorn by example [examples/3_convolution_and_event_datasets.py](./examples/3_convolution_and_event_datasets.py).
+
+```sh
+cd Matterhorn
+python3 examples/3_convolution_and_event_datasets.py
+```
 
 #### NMNIST
 
-We know MNIST. MNIST dataset is for training image classification, consisting of a set of 28x28 pixel grayscale images of handwritten digits (0-9). NMNIST is like MNIST, which is different is that it distorts images and record them into events. The shape of events in NMNIST Dataset is Tx2x34x34.
+We know MNIST. MNIST dataset is for training image classification, consisting of a set of 28x28 pixel grayscale images of handwritten digits (0-9). NMNIST is like MNIST, which is different is that it distorts images and record them into events. The shape of events in NMNIST Dataset is `[T, 2, 34, 34]`.
 
-![NMNIST Dataset](./assets/readme_8.png)
+![NMNIST Dataset](./assets/docs/data/readme_4.png)
 
 You can use NMNIST dataset in Matterhorn by the code below:
 
 ```python
 from matterhorn_pytorch.data import NMNIST
 
 time_steps = 128
@@ -378,17 +374,17 @@
     download = True,
     time_steps = time_steps
 )
 ```
 
 #### CIFAR10-DVS
 
-CIFAR10-DVS dataset records distorted CIFAR-10 image by a DVS camera. The shape of events in CIFAR10-DVS Dataset is Tx2x128x128.
+CIFAR10-DVS dataset records distorted CIFAR-10 image by a DVS camera. The shape of events in CIFAR10-DVS Dataset is `[T, 2, 128, 128]` .
 
-![CIFAR10-DVS Dataset](./assets/readme_9.png)
+![CIFAR10-DVS Dataset](./assets/docs/data/readme_1.png)
 
 You can use CIFAR10-DVS Dataset in Matterhorn by the code below:
 
 ```python
 from matterhorn_pytorch.data import CIFAR10DVS
 
 time_steps = 128
@@ -405,17 +401,17 @@
     download = True,
     time_steps = time_steps
 )
 ```
 
 #### DVS128 Gesture
 
-DVS128 Gesture dataset records gestures from 29 different people under 3 different illuminating conditions by DVS camera. The shape of events in DVS128 Gesture dataset is Tx2x128x128.
+DVS128 Gesture dataset records gestures from 29 different people under 3 different illuminating conditions by DVS camera. The shape of events in DVS128 Gesture dataset is `[T, 2, 128, 128]` .
 
-![DVS128 Gesture Dataset](./assets/readme_10.png)
+![DVS128 Gesture Dataset](./assets/docs/data/readme_2.png)
 
 You can use DVS128 Gesture dataset in Matterhorn by the code below:
 
 ```python
 from matterhorn_pytorch.data import DVS128Gesture
 
 time_steps = 128
@@ -430,33 +426,19 @@
     root = "your/data/path",
     train = False,
     download = True,
     time_steps = time_steps
 )
 ```
 
-**Warning:** You may have to set parameter `sampling` to save the disk space in your device.
-
-```python
-train_dataset = DVS128Gesture(
-    root = "your/data/path",
-    train = True,
-    download = True,
-    sampling = 600,
-    time_steps = time_steps
-)
-```
-
-Recommended sampling ratio is more than 100 (which means choose one from `sampling` events).
-
 #### Spiking Heidelberg Digits (SHD)
 
-SHD dataset records vocal number from 1 to 10 in both English and German and turns them into events. The shape of events in SHD dataset is Tx700.
+SHD dataset records vocal number from 1 to 10 in both English and German and turns them into events. The shape of events in SHD dataset is `[T, 700]`.
 
-![SHD Dataset](./assets/readme_11.png)
+![SHD Dataset](./assets/docs/data/readme_3.png)
 
 You can use SHD dataset in Matterhorn by the code below:
 
 ```python
 from matterhorn_pytorch.data import SpikingHeidelbergDigits
 
 time_steps = 128
@@ -473,22 +455,16 @@
     download = True,
     time_steps = time_steps
 )
 ```
 
 ## 4 Neuromorphic Hardware Support
 
-Will come out soon, but not today.
+Will come out soon, but not today. Sorry.
 
-## References
+## References (and Special Thanks to)
 
-[1] Wei Fang, Yanqi Chen, Jianhao Ding, Zhaofei Yu, Huihui Zhou, Timothée Masquelier, Yonghong Tian, et al. Spikingjelly. [https://github.com/fangwei123456/spikingjelly](https://github.com/fangwei123456/spikingjelly).
+[1] Fang W, Chen Y, Ding J, et al. SpikingJelly: An open-source machine learning infrastructure platform for spike-based intelligence[J]. Science Advances, 2023, 9(40): eadi1480.
 
-```
-@misc{SpikingJelly,
-	title = {SpikingJelly},
-	author = {Fang, Wei and Chen, Yanqi and Ding, Jianhao and Chen, Ding and Yu, Zhaofei and Zhou, Huihui and Timothée Masquelier and Tian, Yonghong and other contributors},
-	year = {2020},
-	howpublished = {\url{https://github.com/fangwei123456/spikingjelly}},
-	note = {Accessed: 2023-08-01},
-}
-```
+[2] Fang W, Yu Z, Chen Y, et al. Deep residual learning in spiking neural networks[J]. Advances in Neural Information Processing Systems, 2021, 34: 21056-21069.
+
+[3] Yao M, Gao H, Zhao G, et al. Temporal-wise attention spiking neural networks for event streams classification[C]//Proceedings of the IEEE/CVF International Conference on Computer Vision. 2021: 10221-10230.
```

### Comparing `matterhorn_pytorch-1.0.1/matterhorn_pytorch.egg-info/SOURCES.txt` & `matterhorn_pytorch-1.2.0/matterhorn_pytorch.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,47 +11,59 @@
 matterhorn_cpp_extensions/api.cpp
 matterhorn_cpp_extensions/base.cpp
 matterhorn_cpp_extensions/base.h
 matterhorn_cpp_extensions/soma.cpp
 matterhorn_cpp_extensions/soma.h
 matterhorn_cpp_extensions/stdp.cpp
 matterhorn_cpp_extensions/stdp.h
-matterhorn_cuda_extensions/__init__.py
 matterhorn_cuda_extensions/api.cpp
 matterhorn_cuda_extensions/base.cu
 matterhorn_cuda_extensions/base.h
-matterhorn_cuda_extensions/cuda_utils.h
 matterhorn_cuda_extensions/setup.py
 matterhorn_cuda_extensions/soma.cpp
 matterhorn_cuda_extensions/soma.h
 matterhorn_cuda_extensions/soma_cuda.cu
 matterhorn_cuda_extensions/stdp.cpp
 matterhorn_cuda_extensions/stdp.h
 matterhorn_cuda_extensions/stdp_cuda.cu
+matterhorn_pytorch/__func__.py
 matterhorn_pytorch/__init__.py
 matterhorn_pytorch.egg-info/PKG-INFO
 matterhorn_pytorch.egg-info/SOURCES.txt
 matterhorn_pytorch.egg-info/dependency_links.txt
 matterhorn_pytorch.egg-info/requires.txt
 matterhorn_pytorch.egg-info/top_level.txt
 matterhorn_pytorch/data/__init__.py
 matterhorn_pytorch/data/aedat.py
+matterhorn_pytorch/data/functional.py
 matterhorn_pytorch/data/hdf5.py
 matterhorn_pytorch/data/nmnist.py
 matterhorn_pytorch/data/skeleton.py
+matterhorn_pytorch/data/transforms.py
+matterhorn_pytorch/lsm/__init__.py
+matterhorn_pytorch/lsm/functional.py
+matterhorn_pytorch/lsm/io.py
+matterhorn_pytorch/lsm/layer.py
 matterhorn_pytorch/model/__init__.py
 matterhorn_pytorch/model/sew.py
 matterhorn_pytorch/model/ta.py
 matterhorn_pytorch/snn/__init__.py
 matterhorn_pytorch/snn/container.py
 matterhorn_pytorch/snn/decoder.py
 matterhorn_pytorch/snn/encoder.py
+matterhorn_pytorch/snn/functional.py
 matterhorn_pytorch/snn/layer.py
-matterhorn_pytorch/snn/learning.py
 matterhorn_pytorch/snn/skeleton.py
 matterhorn_pytorch/snn/soma.py
 matterhorn_pytorch/snn/soma_cpp.py
 matterhorn_pytorch/snn/soma_cuda.py
 matterhorn_pytorch/snn/surrogate.py
 matterhorn_pytorch/snn/synapse.py
+matterhorn_pytorch/tnn/__init__.py
+matterhorn_pytorch/tnn/column.py
+matterhorn_pytorch/tnn/component.py
+matterhorn_pytorch/tnn/functional.py
+matterhorn_pytorch/training/__init__.py
+matterhorn_pytorch/training/functional.py
 matterhorn_pytorch/util/__init__.py
+matterhorn_pytorch/util/interpreter.py
 matterhorn_pytorch/util/plotter.py
```

### Comparing `matterhorn_pytorch-1.0.1/setup.py` & `matterhorn_pytorch-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,97 @@
 from setuptools import find_packages
 from setuptools import setup
-import torch.cuda as cuda
-from torch.utils.cpp_extension import BuildExtension
 import os
-from typing import List
+# import platform
+# from typing import List
 
 
-def get_cpp_files(root_path: str, exceptions: List[str]) -> List[str]:
-    full_list = os.listdir(root_path)
-    res_list = []
-    for filename in full_list:
-        if (filename.endswith(".cpp") or filename.endswith(".cu")) and not (filename in exceptions):
-            res_list.append(os.path.join(root_path, filename))
-    return res_list
+# def get_cpp_files(root_path: str, exceptions: List[str]) -> List[str]:
+#     full_list = os.listdir(root_path)
+#     res_list = []
+#     for filename in full_list:
+#         if (filename.endswith(".cpp") or filename.endswith(".cu")) and not (filename in exceptions):
+#             res_list.append(os.path.join(root_path, filename))
+#     return res_list
 
 
 requirements = ["torch"]
+# try:
+#     ext_modules = []
+#     from torch.cuda import is_available
+#     cuda_available = is_available()
+#     if cuda_available:
+#         print("\033[92mCUDA found on this device, installing Matterhorn CUDA extensions.\033[0m")
+#         from torch.utils.cpp_extension import CUDAExtension
+#         files = get_cpp_files(os.path.join(os.path.abspath("."), "matterhorn_cuda_extensions"), ["base.cpp", "base.cu"])
+#         print("Will compile " + ", ".join(files))
+#         ext_modules.append(CUDAExtension(
+#             "matterhorn_cuda_extensions",
+#             files,
+#             extra_compile_args = {
+#                 "cxx": ["-g", "-w"],
+#                 "nvcc": ["-O2"]
+#             }
+#         ))
+#     else:
+#         print("\033[93mCUDA not found on this device. If you have NVIDIA's GPU, please install CUDA and try again later, or manually install Matterhorn CUDA extensions.\033[0m")
+#     cpp_available = not os.system("g++ --version")
+#     if cpp_available:
+#         print("\033[92mG++ found on this device, installing Matterhorn CPP extensions.\033[0m")
+#         from torch.utils.cpp_extension import CppExtension
+#         files = get_cpp_files(os.path.join(os.path.abspath("."), "matterhorn_cpp_extensions"), ["base.cpp"])
+#         print("Will compile " + ", ".join(files))
+#         ext_modules.append(CppExtension(
+#             "matterhorn_cpp_extensions",
+#             files,
+#             extra_compile_args = {
+#                 "cxx": ["-g", "-w"]
+#             }
+#         ))
+#     else:
+#         print("\033[93mG++ not found on this device. Please install G++ and try again later, or manually install Matterhorn CPP extensions.\033[0m")
+#         if platform.system() == "Windows":
+#             print("\033[93mIf you're Windows user, please download and install G++ from https://github.com/xjtuiair-cag/Matterhorn/blob/main/mingw-get-setup.exe .\033[0m")
+            
+#     cmdclass = {}
+#     if cuda_available or cpp_available:
+#         print("\033[92mTrying to build Matterhorn extensions.\033[0m")
+#         if platform.system() == "Windows":
+#             print("\033[93mIf you're Windows user and errors occur, please follow Microsoft's instruction and install VS generation tools for C++, then retry.\033[0m")
+#         from torch.utils.cpp_extension import BuildExtension
+#         cmdclass = {
+#             "build_ext": BuildExtension
+#         }
+# except:
+#     print("\033[93mFailed to build Matterhorn extensions. You can manually build Matterhorn extensions later.\033[0m")
+#     ext_modules = []
+#     cmdclass = {}
 
-ext_modules = []
-cuda_available = cuda.is_available()
-if cuda_available:
-    print("\033[92mCUDA found on this device, installing matterhorn CUDA extensions.\033[0m")
-    from torch.utils.cpp_extension import CUDAExtension
-    files = get_cpp_files(os.path.join(os.path.abspath("."), "matterhorn_cuda_extensions"), ["base.cpp", "base.cu"])
-    print("Will compile " + ", ".join(files))
-    ext_modules.append(CUDAExtension(
-        "matterhorn_cuda_extensions",
-        files,
-        extra_compile_args = {
-            "cxx": ["-g", "-w"],
-            "nvcc": ["-O2"]
-        }
-    ))
-else:
-    print("\033[91mCUDA not found on this device. If you have NVIDIA's GPU, please install CUDA and try again later, or manually install Matterhorn CUDA extensions.\033[0m")
-cpp_available = not os.system("g++ --version")
-if cpp_available:
-    print("\033[92mg++ found on this device, installing matterhorn CPP extensions.\033[0m")
-    from torch.utils.cpp_extension import CppExtension
-    files = get_cpp_files(os.path.join(os.path.abspath("."), "matterhorn_cpp_extensions"), ["base.cpp"])
-    print("Will compile " + ", ".join(files))
-    ext_modules.append(CppExtension(
-        "matterhorn_cpp_extensions",
-        files,
-        extra_compile_args = {
-            "cxx": ["-g", "-w"]
-        }
-    ))
-else:
-    print("\033[91mg++ not found on this device. Please install g++ and try again later, or manually install Matterhorn CPP extensions.\033[0m")
-cmdclass = None
-if cuda_available or cpp_available:
-    cmdclass = {
-        "build_ext": BuildExtension
-    }
 
 with open(os.path.join(os.path.abspath("."), "requirements.txt"), "r", encoding="utf-8") as fh:
     install_requires = fh.read()
 
 
 with open(os.path.join(os.path.abspath("."), "README.md"), "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     install_requires = install_requires,
     name = "matterhorn_pytorch",
-    version = "1.0.1",
+    version = "1.2.0",
     author = "CAG, IAIR, XJTU, Xi'an, China",
     author_email = "ericwang017@stu.xjtu.edu.cn",
-    description = "Matterhorn is a neo general SNN framework based on PyTorch.",
+    description = "Matterhorn is a novel general neuromorphic computing framework based on PyTorch.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/AmperiaWang/Matterhorn",
+    url = "https://github.com/xjtuiair-cag/Matterhorn",
     packages = find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires = '>=3.7',
-    ext_modules = ext_modules,
-    cmdclass = cmdclass
+    # ext_modules = ext_modules,
+    # cmdclass = cmdclass
 )
```

