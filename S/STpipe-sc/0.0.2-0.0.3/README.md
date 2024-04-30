# Comparing `tmp/STpipe-sc-0.0.2.tar.gz` & `tmp/STpipe-sc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STpipe-sc-0.0.2.tar", last modified: Fri Apr  5 15:10:31 2024, max compression
+gzip compressed data, was "STpipe-sc-0.0.3.tar", last modified: Tue Apr 30 12:15:45 2024, max compression
```

## Comparing `STpipe-sc-0.0.2.tar` & `STpipe-sc-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:10:31.039553 STpipe-sc-0.0.2/
--rw-rw-rw-   0        0        0      945 2024-04-05 15:10:31.038596 STpipe-sc-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 15:10:30.984085 STpipe-sc-0.0.2/STpipe_sc.egg-info/
--rw-rw-rw-   0        0        0      945 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:10:31.039553 STpipe-sc-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1101 2024-04-05 15:10:12.000000 STpipe-sc-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:10:31.028570 STpipe-sc-0.0.2/stpipe/
--rw-rw-rw-   0        0        0     3748 2024-03-26 18:54:55.000000 STpipe-sc-0.0.2/stpipe/Findmarkers.py
--rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.2/stpipe/QC.py
--rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.2/stpipe/__init__.py
--rw-rw-rw-   0        0        0     1674 2024-04-01 16:57:25.000000 STpipe-sc-0.0.2/stpipe/cluster.py
--rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.2/stpipe/format.py
--rw-rw-rw-   0        0        0    21984 2024-04-03 00:48:54.000000 STpipe-sc-0.0.2/stpipe/function.py
--rw-rw-rw-   0        0        0     2507 2024-03-25 17:08:16.000000 STpipe-sc-0.0.2/stpipe/labeltransfer.py
--rw-rw-rw-   0        0        0    37008 2024-04-02 17:59:02.000000 STpipe-sc-0.0.2/stpipe/plot.py
--rw-rw-rw-   0        0        0     5567 2024-04-03 16:18:46.000000 STpipe-sc-0.0.2/stpipe/spatial_metacell.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.495255 STpipe-sc-0.0.3/
+-rw-rw-rw-   0        0        0      942 2024-04-30 12:15:45.491203 STpipe-sc-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.414989 STpipe-sc-0.0.3/STpipe_sc.egg-info/
+-rw-rw-rw-   0        0        0      942 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2024-04-30 12:15:45.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.386979 STpipe-sc-0.0.3/git/
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.387978 STpipe-sc-0.0.3/git/STpipe/
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.450966 STpipe-sc-0.0.3/git/STpipe/stpipe/
+-rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/Findmarkers.py
+-rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/QC.py
+-rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/__init__.py
+-rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/cluster.py
+-rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/format.py
+-rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/function.py
+-rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/labeltransfer.py
+-rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/plot.py
+-rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/spatial_metacell.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 12:15:45.495255 STpipe-sc-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2024-04-30 12:15:14.000000 STpipe-sc-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.486143 STpipe-sc-0.0.3/stpipe/
+-rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/Findmarkers.py
+-rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.3/stpipe/QC.py
+-rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.3/stpipe/__init__.py
+-rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/cluster.py
+-rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.3/stpipe/format.py
+-rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.3/stpipe/function.py
+-rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/labeltransfer.py
+-rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.3/stpipe/plot.py
+-rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.3/stpipe/spatial_metacell.py
```

### Comparing `STpipe-sc-0.0.2/PKG-INFO` & `STpipe-sc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.2
+Version: 0.0.3
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
-Requires-Python: ==3.8.18
-Requires-Dist: rpy2==3.5.15
+Requires-Python: ==3.8
+Requires-Dist: rpy2==3.5.16
 Requires-Dist: anndata2ri==1.3.1
-Requires-Dist: numpy==1.24.4
+Requires-Dist: numpy==1.21.6
 Requires-Dist: diffxpy==0.7.4
 Requires-Dist: scipy==1.10.1
 Requires-Dist: pandas==2.0.3
 Requires-Dist: anndata==0.9.2
-Requires-Dist: shapely==2.0.3
+Requires-Dist: shapely==2.0.4
 Requires-Dist: dask==2023.5.0
-Requires-Dist: numba==0.58.1
+Requires-Dist: numba==0.58.0
 Requires-Dist: pca==2.0.5
 Requires-Dist: openTSNE==1.0.1
 Requires-Dist: igraph==0.11.4
 Requires-Dist: sinfonia==0.0.3
 Requires-Dist: tangram-sc==1.0.4
 Requires-Dist: scanorama==1.7.4
-Requires-Dist: matplotlib==3.7.4
+Requires-Dist: matplotlib==3.7.5
 Requires-Dist: seaborn==0.13.2
 Requires-Dist: adjustText==1.1.1
 Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scikit-misc==0.2.0
+Requires-Dist: scikit-misc==0.1.4
 Requires-Dist: scikit-image==0.21.0
```

### Comparing `STpipe-sc-0.0.2/STpipe_sc.egg-info/PKG-INFO` & `STpipe-sc-0.0.3/STpipe_sc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.2
+Version: 0.0.3
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
-Requires-Python: ==3.8.18
-Requires-Dist: rpy2==3.5.15
+Requires-Python: ==3.8
+Requires-Dist: rpy2==3.5.16
 Requires-Dist: anndata2ri==1.3.1
-Requires-Dist: numpy==1.24.4
+Requires-Dist: numpy==1.21.6
 Requires-Dist: diffxpy==0.7.4
 Requires-Dist: scipy==1.10.1
 Requires-Dist: pandas==2.0.3
 Requires-Dist: anndata==0.9.2
-Requires-Dist: shapely==2.0.3
+Requires-Dist: shapely==2.0.4
 Requires-Dist: dask==2023.5.0
-Requires-Dist: numba==0.58.1
+Requires-Dist: numba==0.58.0
 Requires-Dist: pca==2.0.5
 Requires-Dist: openTSNE==1.0.1
 Requires-Dist: igraph==0.11.4
 Requires-Dist: sinfonia==0.0.3
 Requires-Dist: tangram-sc==1.0.4
 Requires-Dist: scanorama==1.7.4
-Requires-Dist: matplotlib==3.7.4
+Requires-Dist: matplotlib==3.7.5
 Requires-Dist: seaborn==0.13.2
 Requires-Dist: adjustText==1.1.1
 Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scikit-misc==0.2.0
+Requires-Dist: scikit-misc==0.1.4
 Requires-Dist: scikit-image==0.21.0
```

### Comparing `STpipe-sc-0.0.2/setup.py` & `STpipe-sc-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='STpipe-sc',
-    version='0.0.2',
+    version='0.0.3',
     description=('STpipe is designed to analyze spatial transcriptomic data.'),
     author='Mao Guangyao',
     license='MIT License',
     url='https://github.com/mgy520/STpipe',
     packages=find_namespace_packages(),
-    python_requires='==3.8.18',
+    python_requires='==3.8',
     install_requires=[
-            'rpy2==3.5.15',
+            'rpy2==3.5.16',
             'anndata2ri==1.3.1',
-            'numpy==1.24.4',
+            'numpy==1.21.6',
             'diffxpy==0.7.4',
             'scipy==1.10.1',
             'pandas==2.0.3',
             'anndata==0.9.2',
-            'shapely==2.0.3',
+            'shapely==2.0.4',
             'dask==2023.5.0',
-            'numba==0.58.1',
+            'numba==0.58.0',
             'pca==2.0.5',
             'openTSNE==1.0.1',
             'igraph==0.11.4',
             'sinfonia==0.0.3',
             'tangram-sc==1.0.4',
             'scanorama==1.7.4',
-            'matplotlib==3.7.4',
+            'matplotlib==3.7.5',
             'seaborn==0.13.2',
             'adjustText==1.1.1',
             'scikit-learn==1.3.2',
-            'scikit-misc==0.2.0',
+            'scikit-misc==0.1.4',
             'scikit-image==0.21.0'
     ]
 )
```

### Comparing `STpipe-sc-0.0.2/stpipe/Findmarkers.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/Findmarkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from sklearn.utils.sparsefuncs import mean_variance_axis
 from scipy.sparse import issparse
 
 
 def findallmarkers(cdata, cluster_key, min_pct=0.1, only_pos=True):
     """
-        Find marker genes for each cluster in cdata.
+        Find marker genes for each cluster in Spatial transcriptomics data.
 
         Parameters:
             cdata (Anndata): An Anndata object.
             cluster_key (str): The key representing the cell cluster annotations in the observation metadata of the Anndata object.
             min_pct (float, optional): The minimum percentage threshold for filtering sparse genes. Defaults to 0.1.
             only_pos (bool, optional): Whether to consider only genes with positive log2 fold change. Defaults to True.
```

### Comparing `STpipe-sc-0.0.2/stpipe/QC.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/QC.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.2/stpipe/cluster.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/cluster.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from rpy2.robjects import r
 import numpy as np
 
 anndata2ri.activate()
 
 def cluster(cdata, K_set, neighborhood_size, n_PCs):
     """
-        Stereo-seq data spatial clustering.
+        Spatial transcriptomics data spatial clustering.
 
         Parameters:
-            cdata (Anndata): Anndata object containing the single-cell data.
+            cdata (Anndata): Anndata object for Spatial transcriptomics data.
             K_set (list): List of integers specifying the range of cluster numbers to consider.for example:np.arange(10,30)
             neighborhood_size (int): Size of the neighborhood for computing adjacency matrix.
             n_PCs (int): Number of principal components to use.
 
         Returns:
             cdata (Anndata): An Anndata object with cluster labels assigned to observations.
         """
```

### Comparing `STpipe-sc-0.0.2/stpipe/format.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/format.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.2/stpipe/function.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     adata.uns['pca']['variance_ratio'] = results['variance_ratio']
     adata.uns['pca']['explained_var'] = results['explained_var']
     print('[pca] >done.')
     return adata
 
 def tsne(adata, input=15, perplexity=30, learning_rate='auto', random_seed=42,early_exaggeration=12, metric='euclidean',n_jobs=1,**kwargs):
     """
-        Perform t-distributed Stochastic Neighbor Embedding (t-SNE) dimensionality reduction on single-cell RNA-seq data.
+        Perform t-distributed Stochastic Neighbor Embedding (t-SNE) dimensionality reduction on Spatial transcriptomics data.
 
         Parameters:
             adata (AnnData): An anndata object.
             input (int or str, optional): (default: 15).
                 If an integer, it specifies the number of principal components from PCA to use as input for t-SNE.
                 If a string, it can be the name of an existing 'obsm' field in the AnnData object to use as input.
                 If the string does not correspond to an existing field, the function falls back to using the adata.X.
@@ -403,28 +403,29 @@
 
     return adata
 
 
 ##adata,bdata both lognormalized
 def falsepositive(ad_sp, ad_sc, train_gene=[], device='cuda:0', density_prior='rna_count_based', celltype=None):
     """
-        Identify false-positive genes between Stereo-seq data and scRNA-seq data.
+        Identify false-positive genes between Spatial transcriptomics data and scRNA-seq data.
 
         Parameters:
-            ad_sp (anndata.AnnData): Anndata object containing Stereo-seq data.
+            ad_sp (anndata.AnnData): Anndata object containing Spatial transcriptomics data.
             ad_sc (anndata.AnnData): Anndata object containing scRNA-seq data.
             train_gene (list): List of genes to use for training. Default is an empty list.
             density_prior (str, ndarray or None): Spatial density of spots, when is a string, value can be 'rna_count_based' or 'uniform', when is a ndarray, shape = (number_spots,). This array should satisfy the constraints sum() == 1. If None, the density term is ignored. Default value is 'rna_count_based'.
             device (str, optional): Device to use for computation. Default is 'cuda:0'.
             celltype (str or None, optional): Cell type key in ad_sp.obs. If provided, the cell types in the scRNA-seq will be mapped to the spatial transcriptomic data. Default value is None.
 
         Returns:
-            moran_ad_sp (pandas.Series): Pandas series containing Moran's I statistic for Stereo-seq data.\n
+            moran_ad_sp (pandas.Series): Pandas series containing Moran's I statistic for Spatial transcriptomics data.\n
             moran_ad_sc (pandas.Series): Pandas series containing Moran's I statistic for scRNA-seq data.\n
-            ad_ge (anndata.AnnData): AnnData object represents the scRNA-seq data mapping to the Stereo-seq space.
+            ad_ge (anndata.AnnData): AnnData object represents the scRNA-seq data mapping to the Spatial transcriptomics space.
+            as_sp (anndata.AnnData): ad_sp with celltype
         """
     if 'moranI' not in ad_sp.var:
         ad_sp = sinfonia.spatially_variable_genes(ad_sp, mode='moran', coordinate_key='spatial')
     tg.pp_adatas(ad_sc, ad_sp, genes=train_gene)
     ad_map = tg.map_cells_to_space(adata_sc=ad_sc, adata_sp=ad_sp, density_prior=density_prior, device=device,
                                    verbose=False)
     if celltype is not None:
```

### Comparing `STpipe-sc-0.0.2/stpipe/labeltransfer.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/labeltransfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,44 +13,44 @@
     class_prob = (class_prob.T - class_prob.min(1)) / class_prob.ptp(1)
     return class_prob
 
 
 #adata bdata should be lognormalized,both genes are recommended to be highly variable
 def labeltransfer(adata,bdata,celltype='celltype'):
     """
-        Transfer cell type labels from scRNA-seq to Stereo-seq using Scanorama.
+        Transfer cell type labels from scRNA-seq to Spatial transcriptomics data using Scanorama.
 
         It performs batch correction using Scanorama on the combined datasets and computes the label transfer based on cosine distances between the corrected embeddings.
 
         Parameters:
-            adata (anndata.AnnData): AnnData object representing Stereo-seq.
+            adata (anndata.AnnData): AnnData object representing Spatial transcriptomics data.
             bdata (anndata.AnnData): AnnData object representing scRNA-seq.
             celltype (str): The key in the observation metadata of 'bdata' containing cell type labels. Default is 'celltype'.
 
         Returns:
             adata_transfer (anndata.AnnData): AnnData object with transferred cell type labels.
                 The transferred labels are stored in the observation metadata under the key 'labeltransfer_celltype'.
                 Additionally, the maximum confidence score are stored in the observation metadata under the keys 'max_score'.
         """
     bdata.obs[celltype] = bdata.obs[celltype].astype('category')
     adatas = [bdata, adata]
     adatas2 = scanorama.correct_scanpy(adatas, return_dimred=True)
     cdata = anndata.concat(
         adatas2,
         label="dataset",
-        keys=["scRNA-seq", "Stereo-seq"],
+        keys=["scRNA-seq", "St"],
         join="outer",
         uns_merge="first",
     )
 
     distances = 1 - cosine_distances(
         cdata[cdata.obs.dataset == "scRNA-seq"].obsm[
             "X_scanorama"
         ],
-        cdata[cdata.obs.dataset == "Stereo-seq"].obsm[
+        cdata[cdata.obs.dataset == "St"].obsm[
             "X_scanorama"
         ],
     )
     class_prob = _label_transfer(distances, bdata.obs.celltype)
     df = pd.DataFrame(
         class_prob,
         columns=sorted(bdata.obs[celltype].cat.categories),
```

### Comparing `STpipe-sc-0.0.2/stpipe/plot.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,17 +437,17 @@
     plt.tight_layout()
     plt.show()
 
 
 def plot_spatial(adata, by=None, s=5, cmap=None, savefig=None, dpi=360, figsize=(6, 6),
                  tiff=None, coord='spatial', title=None, legend=False, categorical=False, legend_title=True):
     """
-        Plot spatial information from Stereo-seq data.
+        Plot spatial information from Spatial transcriptomics data.
 
-        This function visualizes spatial information from Stereo-seq data. It can display cell
+        This function visualizes spatial information for Spatial transcriptomics data. It can display cell
         coordinates on an image, with the option to color cells based on a specified category or gene expression level.
 
         Parameters:
             adata (anndata.AnnData): An AnnData object containing the spatial data.
             by (str or None): Name of the category column in adata.obs to group cells by, or name of the gene for coloring
                               cells based on gene expression. Defaults to None.
             s (float): Size of the markers representing cells. Defaults to 5.
@@ -586,15 +586,15 @@
     plt.xticks(rotation=xrotation,ha=xha)
     if save:
         plt.savefig(save, bbox_inches='tight', dpi=300)
     plt.show()
 
 
 def plot_cellcount_between_ref_query(adata_query, adata_ref ,key1='labeltransfer_celltype', key2='celltype', figsize=(12, 5),
-                                     xrotation=45, xha='right', save=None, title1='scRNA-seq', title2='Stereo-seq',dpi=360):
+                                     xrotation=45, xha='right', save=None, title1='scRNA-seq', title2='St',dpi=360):
     """
         Plot cell count comparison between reference and query datasets.
 
         This function plots a bar chart comparing the cell counts of different cell types between a reference dataset
         and a query dataset.
 
         Parameters:
@@ -603,15 +603,15 @@
             key1 (str): Key in adata_query.obs representing the cell type information. Defaults to 'labeltransfer_celltype'.
             key2 (str): Key in adata_ref.obs representing the cell type information. Defaults to 'celltype'.
             figsize (tuple): Size of the figure in inches (width, height). Defaults to (12, 5).
             xrotation (int): Rotation angle for x-axis tick labels. Defaults to 45.
             xha (str): Horizontal alignment of x-axis tick labels. Defaults to 'right'.
             save (str or None): File path to save the plot. If None, the plot is not saved. Defaults to None.
             title1 (str): Title for the query dataset plot. Defaults to 'scRNA-seq'.
-            title2 (str): Title for the reference dataset plot. Defaults to 'Stereo-seq'.
+            title2 (str): Title for the reference dataset plot. Defaults to 'St'.
             dpi (int): Dots per inch for the saved figure. Defaults to 360.
         """
     adata_celltype_counts = adata_query.obs[key1].value_counts()
     bdata_celltype_counts = adata_ref.obs[key2].value_counts()
     all_celltypes = set(adata_celltype_counts.index) | set(bdata_celltype_counts.index)
     all_celltypes = sorted(all_celltypes)
```

### Comparing `STpipe-sc-0.0.2/stpipe/spatial_metacell.py` & `STpipe-sc-0.0.3/git/STpipe/stpipe/spatial_metacell.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def spatial_bigcells(adata, method='walktrap', n_pca=30, n_neighbors=200, n_jobs=4, distance_threshold=50, p=5,
                      resolution=1,celltypes='celltype',nb_trials=1,
                      weights=None, const=1, a=50, sigma=10, b=10, node_weight=None):
     """
         Detect spatial metacell using network-based clustering algorithms.
 
         Parameters:
-            adata (anndata.AnnData): An AnnData object representing the Stereo-seq data.
+            adata (anndata.AnnData): An AnnData object representing the Spatial transcriptomics data.
             method (str, optional): The clustering method to use. Options are 'walktrap', 'edge_betweenness', 'leiden', 'multilevel', and 'infomap'.
             n_pca (int, optional): Number of principal components to use for dimensionality reduction.
             n_neighbors (int, optional): Number of neighbors to consider for constructing the k-nearest neighbor graph.
             n_jobs (int, optional): Number of parallel jobs to run for k-nearest neighbor search.
             distance_threshold (int or None, optional): Threshold distance for filtering out distant neighbors.
             p (int, optional): For method is walktrap or edge_betweenness. The desired number of cells per metacell.
             nb_trials (int): For method is infomap.The number of attempts to partition the network (can be any integer value equal or larger than 1).
```

