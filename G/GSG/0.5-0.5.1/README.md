# Comparing `tmp/GSG-0.5.tar.gz` & `tmp/GSG-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.5.tar", last modified: Thu Apr 18 09:17:27 2024, max compression
+gzip compressed data, was "dist/GSG-0.5.1.tar", last modified: Tue Apr 30 02:31:21 2024, max compression
```

## Comparing `GSG-0.5.tar` & `GSG-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 09:17:27.000000 GSG-0.5/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 09:17:27.000000 GSG-0.5/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       68 2024-04-18 09:17:26.000000 GSG-0.5/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-18 09:17:26.000000 GSG-0.5/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-18 09:17:26.000000 GSG-0.5/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-04-18 09:17:26.000000 GSG-0.5/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-18 09:17:26.000000 GSG-0.5/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    40597 2024-04-18 05:21:38.000000 GSG-0.5/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       68 2024-04-18 09:17:27.000000 GSG-0.5/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2854 2023-06-08 05:59:08.000000 GSG-0.5/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 09:17:27.000000 GSG-0.5/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 09:17:27.000000 GSG-0.5/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-18 09:17:27.000000 GSG-0.5/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      589 2024-04-18 09:17:22.000000 GSG-0.5/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-18 09:17:27.000000 GSG-0.5/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:31:21.000000 GSG-0.5.1/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2732 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-30 02:31:21.000000 GSG-0.5.1/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40597 2024-04-18 05:21:38.000000 GSG-0.5.1/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2732 2024-04-30 02:31:21.000000 GSG-0.5.1/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2555 2024-04-30 02:29:01.000000 GSG-0.5.1/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:31:21.000000 GSG-0.5.1/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.1/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.1/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:31:21.000000 GSG-0.5.1/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.1/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.1/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.1/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.1/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.1/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.1/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.1/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-30 02:31:21.000000 GSG-0.5.1/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-04-30 02:26:39.000000 GSG-0.5.1/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:31:21.000000 GSG-0.5.1/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.1/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.1/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.1/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.1/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.1/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.1/tools/utils.py
```

### Comparing `GSG-0.5/GSG.py` & `GSG-0.5.1/GSG.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/README.md` & `GSG-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,44 +5,31 @@
 <br>
 ## Overview
 
 GSG takes ST data as input and outputs,its spatially coherent graph representation learning. The ST data contain two components: gene expression and spatial location information. The gene expression of a spot is initially reduced by principal component analysis (PCA) or  initial extraction of highly variable genes (HVGs) as the initial spot features, which are used as nodes in the graph. Then, an adjacency of the graph is constructed based on the location  information. Specifically, the location information is used to calculate the relative distance matrix among the spots. According to the biological assumption that cells influence their neighbours according to the diffusion principle, we choose a certain distance threshold to generate a 0-1 adjacency matrix for the graph. To calculate the representation learning of the graph, we introduced a self-supervised masked graph autoencoder. GSG selects a random number of nodes and masks their initial node features using a mask token [MASK]. Then, a GNN encoder is used to obtain the corrupted graph embedding. The selected nodes are remasked with another token (DMASK) in the extracted embedding and passed through a decoder composed of GNNs to reproduce the initial features. The decoder output is used to reconstruct the node feature of the masked node, using the scaled cosine error as the loss function. By using MASK, GSG enhances the utilization of features of neighbouring nodes for better representation of ST data. With generative self-supervised graph learning, GSG learns to encode a spot/cell node embedding that contains gene expression information, which is further used to visualize the data with a UMAP plot and for other downstream analyses34.
 
 ## Requirements
 You'll need to install the following packages in order to run the codes.
-* python==3.7.12
+* python==3.8
 * torch==1.8.0
 * cudnn==8.4
-* numpy==1.21.6
+* numpy==1.22.0
 * scanpy==1.8.2
 * anndata==0.8.0
 * dgl==0.9.0
 * pandas==1.2.4
 * scipy==1.7.3
 * scikit-learn==1.0.1 
 * tqdm==4.64.1
 * matplotlib==3.5.3
 * tensorboardX==2.5.1
+* pyyaml==6.0.1
+* ploty==5.21.0
+* kaleido==0.2.1
+* igraph==0.11.4
 
-## Installation
-
-### From source
-Start by grabbing this source codes:
-```sh
-git clone https://github.com/keaml-Guan/GSG.git
-cd GSG
-```
-### Use python virutal environment with conda
-```sh
-conda creat -n gsg python=3.7
-conda activate gsg
-pip install -r requirements.txt
-```
-## Quick Start
-```sh
-python GSG_cluster.py --device 0 --cluster_label layer_guess_reordered_short
-```
+## Citation
 
 
 <!--
 ## Citation
 -->
```

### Comparing `GSG-0.5/datasets/data_util.py` & `GSG-0.5.1/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/__init__.py` & `GSG-0.5.1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/dot_gat.py` & `GSG-0.5.1/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/edcoder.py` & `GSG-0.5.1/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/gat.py` & `GSG-0.5.1/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/gcn.py` & `GSG-0.5.1/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/gin.py` & `GSG-0.5.1/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/models/loss_func.py` & `GSG-0.5.1/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/tools/batch_remove.py` & `GSG-0.5.1/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/tools/evaluation.py` & `GSG-0.5.1/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/tools/parameters_dict.py` & `GSG-0.5.1/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/tools/test.py` & `GSG-0.5.1/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5/tools/utils.py` & `GSG-0.5.1/tools/utils.py`

 * *Files identical despite different names*

