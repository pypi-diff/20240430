# Comparing `tmp/cfr-2024.4.30.tar.gz` & `tmp/cfr-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2024.4.30.tar", last modified: Tue Apr 30 16:56:17 2024, max compression
+gzip compressed data, was "cfr-2024.4.4.tar", last modified: Fri Apr  5 00:39:53 2024, max compression
```

## Comparing `cfr-2024.4.30.tar` & `cfr-2024.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-30 16:56:17.123007 cfr-2024.4.30/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-2024.4.30/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3207 2024-04-30 16:56:17.122425 cfr-2024.4.30/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1902 2024-04-30 08:43:27.000000 cfr-2024.4.30/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-30 16:56:17.105522 cfr-2024.4.30/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5134 2023-07-10 00:08:10.000000 cfr-2024.4.30/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-30 16:56:17.112971 cfr-2024.4.30/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      732 2023-07-10 00:08:10.000000 cfr-2024.4.30/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    27513 2024-04-06 05:42:18.000000 cfr-2024.4.30/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-30 16:56:17.119346 cfr-2024.4.30/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-2024.4.30/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2024-04-06 07:19:03.000000 cfr-2024.4.30/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-2024.4.30/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-2024.4.30/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    81217 2024-04-06 07:14:16.000000 cfr-2024.4.30/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49870 2024-04-04 23:42:37.000000 cfr-2024.4.30/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    61031 2024-04-30 16:54:27.000000 cfr-2024.4.30/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6083 2024-03-13 16:55:21.000000 cfr-2024.4.30/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    19837 2023-07-10 00:08:11.000000 cfr-2024.4.30/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    25886 2024-04-03 20:09:47.000000 cfr-2024.4.30/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    62648 2024-04-05 15:23:37.000000 cfr-2024.4.30/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-30 16:56:17.120599 cfr-2024.4.30/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3207 2024-04-30 16:56:14.000000 cfr-2024.4.30/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2024-04-30 16:56:15.000000 cfr-2024.4.30/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-30 16:56:14.000000 cfr-2024.4.30/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-2024.4.30/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      212 2024-04-30 16:56:14.000000 cfr-2024.4.30/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2024-04-30 16:56:14.000000 cfr-2024.4.30/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-30 16:56:17.123091 cfr-2024.4.30/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1480 2024-04-30 16:54:46.000000 cfr-2024.4.30/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.146807 cfr-2024.4.4/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-2024.4.4/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-05 00:39:53.145863 cfr-2024.4.4/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1421 2024-03-13 16:55:21.000000 cfr-2024.4.4/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.088819 cfr-2024.4.4/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5134 2023-07-10 00:08:10.000000 cfr-2024.4.4/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.127561 cfr-2024.4.4/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      732 2023-07-10 00:08:10.000000 cfr-2024.4.4/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    27431 2024-04-03 20:06:27.000000 cfr-2024.4.4/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.141879 cfr-2024.4.4/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-2024.4.4/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-2024.4.4/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-2024.4.4/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-2024.4.4/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    81175 2024-04-04 23:19:07.000000 cfr-2024.4.4/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49870 2024-04-04 23:42:37.000000 cfr-2024.4.4/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60527 2024-03-13 16:55:21.000000 cfr-2024.4.4/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6083 2024-03-13 16:55:21.000000 cfr-2024.4.4/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    19837 2023-07-10 00:08:11.000000 cfr-2024.4.4/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    25886 2024-04-03 20:09:47.000000 cfr-2024.4.4/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    62601 2024-04-04 21:58:32.000000 cfr-2024.4.4/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.143906 cfr-2024.4.4/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-2024.4.4/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      201 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-05 00:39:53.146914 cfr-2024.4.4/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1453 2024-04-05 00:39:18.000000 cfr-2024.4.4/setup.py
```

### Comparing `cfr-2024.4.30/LICENSE` & `cfr-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/PKG-INFO` & `cfr-2024.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.4.30
+Version: 2024.4.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
@@ -25,15 +25,14 @@
 Requires-Dist: eofs
 Requires-Dist: plotly
 Requires-Dist: pyresample
 Provides-Extra: psm
 Requires-Dist: pathos; extra == "psm"
 Requires-Dist: fbm; extra == "psm"
 Requires-Dist: pyvsl; extra == "psm"
-Requires-Dist: pybaywatch; extra == "psm"
 Provides-Extra: ml
 Requires-Dist: scikit-learn; extra == "ml"
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Provides-Extra: graphem
 Requires-Dist: cython; extra == "graphem"
 Requires-Dist: scikit-learn; extra == "graphem"
@@ -42,17 +41,14 @@
 [![PyPI version](https://badge.fury.io/py/cfr.svg)](https://badge.fury.io/py/cfr)
 [![PyPI](https://img.shields.io/badge/python-3.11-blue.svg)]()
 [![license](https://img.shields.io/github/license/fzhu2e/cfr.svg)]()
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
 
 # `cfr`: a Python package for Climate Field Reconstruction
 
-> [!NOTE]
-> Zhu, F., Emile-Geay, J., Hakim, G. J., Guillot, D., Khider, D., Tardif, R., & Perkins, W. A. (2024). cfr (v2024.1.26): a Python package for climate field reconstruction. Geoscientific Model Development, 17(8), 3409–3431. https://doi.org/10.5194/gmd-17-3409-2024
-
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
 + the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
 + the calibration and running of the proxy system models (PSMs, [Evans et al., 2013](https://doi.org/10.1016/j.quascirev.2013.05.024)),
 + the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR ([Hakim et al., 2016](https://doi.org/10.1002/2016JD024751); [Tardif et al., 2019](https://doi.org/https://doi.org/10.5194/cp-15-1251-2019)) and GraphEM ([Guillot et al., 2015](https://doi.org/10.1214/14-AOAS794)), and
 + the validation of the reconstructions, etc.
@@ -60,11 +56,10 @@
 For more details, please refer to the documentation linked below.
 
 ## Documentation
 
 + Homepage: https://fzhu2e.github.io/cfr
 + Installation: https://fzhu2e.github.io/cfr/ug-installation.html
 
-## How to cite
+## How to cite this repo
 
-If you find this package useful, please cite:
-+ Zhu, F., Emile-Geay, J., Hakim, G. J., Guillot, D., Khider, D., Tardif, R., & Perkins, W. A. (2024). cfr (v2024.1.26): a Python package for climate field reconstruction. Geoscientific Model Development, 17(8), 3409–3431. https://doi.org/10.5194/gmd-17-3409-2024
+This repo can be cited with DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cfr-2024.4.30/bin/cfr` & `cfr-2024.4.4/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/__init__.py` & `cfr-2024.4.4/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/climate.py` & `cfr-2024.4.4/cfr/climate.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,18 +537,15 @@
         if hasattr(self, 'plot_kwargs'):
             _kwargs.update(self.plot_kwargs)
 
         if 'title' not in kwargs and 'title' not in _kwargs:
             if len(self.da.dims) == 3:
                 t_value = self.da.time.values[0]
             elif len(self.da.dims) == 2:
-                try:
-                    t_value = self.da.time.values
-                except:
-                    t_value = ''
+                t_value = self.da.time.values
 
             try:
                 date_str = '-'.join(str(t_value).split('-')[:2])
             except:
                 date_str = str(t_value)
 
             kwargs['title'] = f'{self.da.name}, {date_str}'
```

### Comparing `cfr-2024.4.30/cfr/da/enkf.py` & `cfr-2024.4.4/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/gcm.py` & `cfr-2024.4.4/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/ml.py` & `cfr-2024.4.4/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/proxy.py` & `cfr-2024.4.4/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,14 @@
             elif noise == 'colored':
                 colored_noise_kws = {} if colored_noise_kws is None else colored_noise_kws
                 _colored_noise_kws = {'seed': seed, 'alpha': 1, 't': self.pseudo.time}
                 _colored_noise_kws.update(colored_noise_kws)
                 noise = utils.colored_noise(**_colored_noise_kws)
 
             self.pseudo.value += noise / np.std(noise) * sigma
-            self.pseudo.R = np.var(noise)
             if verbose: utils.p_success(f'>>> ProxyRecord.pseudo added with {noise} noise (SNR={SNR}).')
 
         if match_var or match_mean:
             proxy_time_min = np.min(self.time)
             proxy_time_max = np.max(self.time)
             pseudo_time_min = np.min(self.pseudo.time)
             pseudo_time_max = np.max(self.pseudo.time)
```

### Comparing `cfr-2024.4.30/cfr/psm.py` & `cfr-2024.4.4/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/reconjob.py` & `cfr-2024.4.4/cfr/reconjob.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,14 @@
             calib_period (tuple or list): the time period for calibration.
             use_predefined_R (bool): use the predefined observation error covariance instead of by calibration.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
         ptype_psm_dict_default = {ptype: 'Linear' for ptype in set(self.proxydb.type_list)}
         ptype_season_dict_default = {ptype: list(range(1, 13)) for ptype in set(self.proxydb.type_list)}
         ptype_clim_dict_default = {ptype: ['tas'] for ptype in set(self.proxydb.type_list)}
-
         if ptype_psm_dict is not None: ptype_psm_dict_default.update(ptype_psm_dict)
         if ptype_season_dict is not None: ptype_season_dict_default.update(ptype_season_dict)
         if ptype_clim_dict is not None: ptype_clim_dict_default.update(ptype_clim_dict)
 
         ptype_psm_dict = self.io_cfg(
             'ptype_psm_dict', ptype_psm_dict_default,
             verbose=verbose)
@@ -473,37 +472,28 @@
                 self.proxydb.records[pid].tags.add('calibrated')
                 if not use_predefined_R:
                     self.proxydb.records[pid].R = pobj.psm.calib_details['PSMmse']  # assign obs err variance
 
         if verbose:
             p_success(f'>>> {self.proxydb.nrec_tags("calibrated")} records tagged "calibrated" with ProxyRecord.psm created')
 
-    def forward_psms(self, verbose=False, ptype_forward_dict=None):
+    def forward_psms(self, verbose=False, **kwargs):
         ''' Forward the PSMs.
 
         Args:
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
-        ptype_forward_dict_default = {}
-        if ptype_forward_dict is not None: ptype_forward_dict_default.update(ptype_forward_dict)
-        ptype_forward_dict = self.io_cfg(
-            'ptype_forward_dict', ptype_forward_dict_default,
-            verbose=verbose)
-
         pdb_calib = self.proxydb.filter(by='tag', keys={'calibrated'})
             
         for pid, pobj in tqdm(pdb_calib.records.items(), total=pdb_calib.nrec, desc='Forwarding the PSMs'):
             for vn in pobj.psm.climate_required:
                 if 'clim' not in pobj.__dict__ or f'model.{vn}' not in pobj.clim:
                     pobj.get_clim(self.prior[vn], tag='model')
 
-            if pobj.ptype in ptype_forward_dict:
-                pobj.pseudo = pobj.psm.forward(**ptype_forward_dict[pobj.ptype])
-            else:
-                pobj.pseudo = pobj.psm.forward()
+            pobj.pseudo = pobj.psm.forward(**kwargs)
 
         if verbose:
             p_success(f'>>> ProxyRecord.pseudo created for {pdb_calib.nrec} records')
 
     def run_da(self, recon_period=None, recon_loc_rad=None, recon_timescale=None,
                recon_sampling_mode=None, recon_sampling_dist=None, recon_vars=None,
                normal_sampling_sigma=None, normal_sampling_cutoff_factor=None,
@@ -846,16 +836,15 @@
         self.load_clim(tag='prior', path_dict=self.configs['prior_path'],
                        anom_period=self.configs[f'prior_anom_period'],
                        rename_dict=prior_rename_dict, verbose=verbose)
         self.load_clim(tag='obs', path_dict=self.configs['obs_path'],
                        anom_period=self.configs[f'obs_anom_period'],
                        rename_dict=obs_rename_dict, verbose=verbose)
         self.calib_psms(ptype_psm_dict=self.configs['ptype_psm_dict'],
-                        ptype_season_dict=self.configs['ptype_season_dict'],
-                        ptype_clim_dict=self.configs['ptype_clim_dict'], verbose=verbose)
+                        ptype_season_dict=self.configs['ptype_season_dict'], verbose=verbose)
         self.forward_psms(verbose=verbose)
 
         if 'prior_annualize_months' in self.configs:
             self.annualize_clim(tag='prior', months=self.configs['prior_annualize_months'], verbose=verbose)
 
         if 'prior_regrid_nlat' in self.configs:
             self.regrid_clim(tag='prior', nlat=self.configs['prior_regrid_nlat'],
```

### Comparing `cfr-2024.4.30/cfr/reconres.py` & `cfr-2024.4.4/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/ts.py` & `cfr-2024.4.4/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/utils.py` & `cfr-2024.4.4/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.30/cfr/visual.py` & `cfr-2024.4.4/cfr/visual.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     label_legend.remove()
     ax.add_artist(label_legend)
     line.remove()
 
 def plot_field_map(field_var, lat, lon, levels=50, add_cyclic_point=True,
                    title=None, title_size=20, title_weight='normal', figsize=[10, 8],
                    plot_proxydb=False, proxydb=None, plot_proxydb_lgd=False, proxydb_lgd_kws=None,
-                   proxy_marker=None, proxy_color=None, modern_topo=True,
+                   proxy_marker=None, proxy_color=None,
                    site_lats=None, site_lons=None, site_marker='o',
                    site_markersize=50, site_color=sns.xkcd_rgb['amber'],
                    projection='Robinson', transform=ccrs.PlateCarree(),
                    proj_args=None, latlon_range=None, central_longitude=180,
                    lon_ticks=[0, 60, 120, 180, 240, 300], lat_ticks=[-90, 45, 0, 45, 90],
                    land_color=sns.xkcd_rgb['light grey'], ocean_color=sns.xkcd_rgb['light grey'],
                    land_zorder=None, ocean_zorder=None, signif_values=None, signif_range=[0.05, 9999], hatch='..',
@@ -404,18 +404,16 @@
             ax.xaxis.set_major_formatter(lon_formatter)
             ax.yaxis.set_major_formatter(lat_formatter)
             ax.set_xticks(lon_ticks[mask_lon], crs=ccrs.PlateCarree())
             ax.set_yticks(lat_ticks[mask_lat], crs=ccrs.PlateCarree())
     else:
         ax.set_global()
 
-    if modern_topo:
-        ax.add_feature(cfeature.LAND, facecolor=land_color, edgecolor=land_color, zorder=land_zorder)
-        ax.add_feature(cfeature.OCEAN, facecolor=ocean_color, edgecolor=ocean_color, zorder=ocean_zorder)
-
+    ax.add_feature(cfeature.LAND, facecolor=land_color, edgecolor=land_color, zorder=land_zorder)
+    ax.add_feature(cfeature.OCEAN, facecolor=ocean_color, edgecolor=ocean_color, zorder=ocean_zorder)
     if add_coastlines:
         ax.coastlines(zorder=99)
 
     if add_gridlines:
         ax.gridlines(edgecolor='gray', linestyle=':', crs=transform)
 
     if cmap is not None:
```

### Comparing `cfr-2024.4.30/cfr.egg-info/PKG-INFO` & `cfr-2024.4.4/cfr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.4.30
+Version: 2024.4.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
@@ -25,15 +25,14 @@
 Requires-Dist: eofs
 Requires-Dist: plotly
 Requires-Dist: pyresample
 Provides-Extra: psm
 Requires-Dist: pathos; extra == "psm"
 Requires-Dist: fbm; extra == "psm"
 Requires-Dist: pyvsl; extra == "psm"
-Requires-Dist: pybaywatch; extra == "psm"
 Provides-Extra: ml
 Requires-Dist: scikit-learn; extra == "ml"
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Provides-Extra: graphem
 Requires-Dist: cython; extra == "graphem"
 Requires-Dist: scikit-learn; extra == "graphem"
@@ -42,17 +41,14 @@
 [![PyPI version](https://badge.fury.io/py/cfr.svg)](https://badge.fury.io/py/cfr)
 [![PyPI](https://img.shields.io/badge/python-3.11-blue.svg)]()
 [![license](https://img.shields.io/github/license/fzhu2e/cfr.svg)]()
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
 
 # `cfr`: a Python package for Climate Field Reconstruction
 
-> [!NOTE]
-> Zhu, F., Emile-Geay, J., Hakim, G. J., Guillot, D., Khider, D., Tardif, R., & Perkins, W. A. (2024). cfr (v2024.1.26): a Python package for climate field reconstruction. Geoscientific Model Development, 17(8), 3409–3431. https://doi.org/10.5194/gmd-17-3409-2024
-
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
 + the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
 + the calibration and running of the proxy system models (PSMs, [Evans et al., 2013](https://doi.org/10.1016/j.quascirev.2013.05.024)),
 + the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR ([Hakim et al., 2016](https://doi.org/10.1002/2016JD024751); [Tardif et al., 2019](https://doi.org/https://doi.org/10.5194/cp-15-1251-2019)) and GraphEM ([Guillot et al., 2015](https://doi.org/10.1214/14-AOAS794)), and
 + the validation of the reconstructions, etc.
@@ -60,11 +56,10 @@
 For more details, please refer to the documentation linked below.
 
 ## Documentation
 
 + Homepage: https://fzhu2e.github.io/cfr
 + Installation: https://fzhu2e.github.io/cfr/ug-installation.html
 
-## How to cite
+## How to cite this repo
 
-If you find this package useful, please cite:
-+ Zhu, F., Emile-Geay, J., Hakim, G. J., Guillot, D., Khider, D., Tardif, R., & Perkins, W. A. (2024). cfr (v2024.1.26): a Python package for climate field reconstruction. Geoscientific Model Development, 17(8), 3409–3431. https://doi.org/10.5194/gmd-17-3409-2024
+This repo can be cited with DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cfr-2024.4.30/setup.py` & `cfr-2024.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2024.4.30',
+    version='2024.4.4',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
@@ -39,15 +39,14 @@
         'pyresample',
     ],
     extras_require={
         'psm': [
             'pathos',
             'fbm',
             'pyvsl',
-            'pybaywatch',
         ],
         'ml': [
             'scikit-learn',
             'torch',
             'torchvision',
         ],
         'graphem': [
```

