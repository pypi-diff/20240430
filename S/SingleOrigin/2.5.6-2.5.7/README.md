# Comparing `tmp/SingleOrigin-2.5.6.tar.gz` & `tmp/singleorigin-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SingleOrigin-2.5.6.tar", last modified: Mon Apr  1 17:24:55 2024, max compression
+gzip compressed data, was "singleorigin-2.5.7.tar", last modified: Mon Apr 29 22:10:43 2024, max compression
```

## Comparing `SingleOrigin-2.5.6.tar` & `singleorigin-2.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.179841 SingleOrigin-2.5.6/
--rw-r--r--   0 funni      (501) staff       (20)    32452 2022-01-20 18:33:29.000000 SingleOrigin-2.5.6/LICENSE.txt
--rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-01 17:24:55.179622 SingleOrigin-2.5.6/PKG-INFO
--rw-r--r--   0 funni      (501) staff       (20)     2151 2024-01-29 15:54:52.000000 SingleOrigin-2.5.6/README.md
--rw-r--r--   0 funni      (501) staff       (20)     1182 2024-04-01 17:24:00.000000 SingleOrigin-2.5.6/pyproject.toml
--rw-r--r--   0 funni      (501) staff       (20)       38 2024-04-01 17:24:55.179888 SingleOrigin-2.5.6/setup.cfg
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.173117 SingleOrigin-2.5.6/src/
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.176072 SingleOrigin-2.5.6/src/SingleOrigin/
--rw-r--r--   0 funni      (501) staff       (20)     1753 2022-02-04 19:39:13.000000 SingleOrigin-2.5.6/src/SingleOrigin/Element_table.txt
--rw-r--r--   0 funni      (501) staff       (20)     2277 2024-04-01 17:24:32.000000 SingleOrigin-2.5.6/src/SingleOrigin/__init__.py
--rw-r--r--   0 funni      (501) staff       (20)    33831 2024-01-29 18:22:49.000000 SingleOrigin-2.5.6/src/SingleOrigin/cell_transform.py
--rw-r--r--   0 funni      (501) staff       (20)   141016 2024-01-29 19:51:17.000000 SingleOrigin-2.5.6/src/SingleOrigin/find_atom_columns.py
--rw-r--r--   0 funni      (501) staff       (20)    64684 2024-03-29 21:44:25.000000 SingleOrigin-2.5.6/src/SingleOrigin/measure_lattice.py
--rw-r--r--   0 funni      (501) staff       (20)   116689 2024-03-11 19:35:52.000000 SingleOrigin-2.5.6/src/SingleOrigin/utils.py
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.179377 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/
--rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/PKG-INFO
--rw-r--r--   0 funni      (501) staff       (20)      434 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/SOURCES.txt
--rw-r--r--   0 funni      (501) staff       (20)        1 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/dependency_links.txt
--rw-r--r--   0 funni      (501) staff       (20)      162 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/requires.txt
--rw-r--r--   0 funni      (501) staff       (20)       13 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/top_level.txt
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-29 22:10:43.669286 singleorigin-2.5.7/
+-rw-r--r--   0 funni      (501) staff       (20)    32452 2022-01-20 18:33:29.000000 singleorigin-2.5.7/LICENSE.txt
+-rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-29 22:10:43.669084 singleorigin-2.5.7/PKG-INFO
+-rw-r--r--   0 funni      (501) staff       (20)     2151 2024-01-29 15:54:52.000000 singleorigin-2.5.7/README.md
+-rw-r--r--   0 funni      (501) staff       (20)     1182 2024-04-29 22:04:29.000000 singleorigin-2.5.7/pyproject.toml
+-rw-r--r--   0 funni      (501) staff       (20)       38 2024-04-29 22:10:43.669337 singleorigin-2.5.7/setup.cfg
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-29 22:10:43.666057 singleorigin-2.5.7/src/
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-29 22:10:43.667976 singleorigin-2.5.7/src/SingleOrigin/
+-rw-r--r--   0 funni      (501) staff       (20)     1753 2022-02-04 19:39:13.000000 singleorigin-2.5.7/src/SingleOrigin/Element_table.txt
+-rw-r--r--   0 funni      (501) staff       (20)     2297 2024-04-29 22:04:00.000000 singleorigin-2.5.7/src/SingleOrigin/__init__.py
+-rw-r--r--   0 funni      (501) staff       (20)    33831 2024-01-29 18:22:49.000000 singleorigin-2.5.7/src/SingleOrigin/cell_transform.py
+-rw-r--r--   0 funni      (501) staff       (20)   140550 2024-04-29 20:56:43.000000 singleorigin-2.5.7/src/SingleOrigin/find_atom_columns.py
+-rw-r--r--   0 funni      (501) staff       (20)    67958 2024-04-26 22:01:05.000000 singleorigin-2.5.7/src/SingleOrigin/measure_lattice.py
+-rw-r--r--   0 funni      (501) staff       (20)   113123 2024-04-29 21:54:33.000000 singleorigin-2.5.7/src/SingleOrigin/utils.py
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-29 22:10:43.668852 singleorigin-2.5.7/src/SingleOrigin.egg-info/
+-rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-29 22:10:43.000000 singleorigin-2.5.7/src/SingleOrigin.egg-info/PKG-INFO
+-rw-r--r--   0 funni      (501) staff       (20)      434 2024-04-29 22:10:43.000000 singleorigin-2.5.7/src/SingleOrigin.egg-info/SOURCES.txt
+-rw-r--r--   0 funni      (501) staff       (20)        1 2024-04-29 22:10:43.000000 singleorigin-2.5.7/src/SingleOrigin.egg-info/dependency_links.txt
+-rw-r--r--   0 funni      (501) staff       (20)      162 2024-04-29 22:10:43.000000 singleorigin-2.5.7/src/SingleOrigin.egg-info/requires.txt
+-rw-r--r--   0 funni      (501) staff       (20)       13 2024-04-29 22:10:43.000000 singleorigin-2.5.7/src/SingleOrigin.egg-info/top_level.txt
```

### Comparing `SingleOrigin-2.5.6/LICENSE.txt` & `singleorigin-2.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.6/PKG-INFO` & `singleorigin-2.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleOrigin
-Version: 2.5.6
+Version: 2.5.7
 Summary: Crystallographic analysis for STEM data
 Author-email: Stephen Funni <sdf68@cornell.edu>
 Project-URL: homepage, https://github.com/sdfunni/SingleOrigin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `SingleOrigin-2.5.6/README.md` & `singleorigin-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.6/pyproject.toml` & `singleorigin-2.5.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SingleOrigin"
-version = "2.5.6"
+version = "2.5.7"
 authors = [{name = "Stephen Funni", email = "sdf68@cornell.edu"}]
 description = "Crystallographic analysis for STEM data"
 readme = "README.md"
 license = { file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/Element_table.txt` & `singleorigin-2.5.7/src/SingleOrigin/Element_table.txt`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/__init__.py` & `singleorigin-2.5.7/src/SingleOrigin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SingleOrigin is a module for atomic column position finding intended for 
     high resolution scanning transmission electron microscope images.
-    Copyright (C) 2023  Stephen D. Funni
+    Copyright (C) 2024  Stephen D. Funni
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -12,15 +12,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see https://www.gnu.org/licenses"""
 
 
-__version__ = "2.5.6"
+__version__ = "2.5.7"
 
 from SingleOrigin.utils import (
     metric_tensor,
     bond_length,
     bond_angle,
     absolute_angle_bt_vectors,
     rotation_angle_bt_vectors,
@@ -31,37 +31,36 @@
     elec_wavelength,
     select_folder,
     select_file,
     load_image,
     image_norm,
     write_image_array_to_tif,
     band_pass_filter,
+    linearKDE_2D,
+    nearestKDE_2D,
     fast_rotate_90deg,
     rotation_matrix,
     rotate_xy,
     rotate_image_kde,
+    get_circular_kernel,
     std_local,
     binary_find_largest_rectangle,
     binary_find_smallest_rectangle,
     plane_2d,
-    plane_ss,
     plane_fit,
     fft_square,
     hann_2d,
     get_fft_pixel_size,
     get_feature_size,
     detect_peaks,
     watershed_segment,
     img_equ_ellip,
     img_ellip_param,
     gaussian_2d,
-    gaussian_ellip_ss,
-    gaussian_circ_ss,
-    fit_gaussian_ellip,
-    fit_gaussian_circ,
+    fit_gaussians,
     pack_data_prefit,
     fit_gaussian_group,
     cft,
     find_ewpc_peak,
     get_ewpc,
     get_ewic,
     center_image_point,
@@ -73,14 +72,16 @@
     pick_points,
     register_lattice_to_peaks,
     plot_basis,
     disp_vect_sum_squares,
     fit_lattice,
     fft_amplitude_area,
     quickplot,
+    gaussian_circ_ss,
+    gaussian_ellip_ss,
 )
 
 from SingleOrigin.cell_transform import UnitCell
 
 from SingleOrigin.find_atom_columns import (
     HRImage,
     AtomicColumnLattice,
```

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/cell_transform.py` & `singleorigin-2.5.7/src/SingleOrigin/cell_transform.py`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/find_atom_columns.py` & `singleorigin-2.5.7/src/SingleOrigin/find_atom_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,19 +62,20 @@
 from skimage.morphology import erosion
 
 from SingleOrigin.utils import (
     image_norm,
     linearKDE_2D,
     img_ellip_param,
     gaussian_2d,
-    fit_gaussian_ellip,
     pack_data_prefit,
+    fit_gaussians,
     fit_gaussian_group,
     detect_peaks,
     watershed_segment,
+    get_circular_kernel,
     std_local,
     fft_square,
     get_vpcf,
     fit_lattice,
     get_feature_size,
     rotation_matrix,
     rotate_xy,
@@ -324,15 +325,14 @@
                 np.array([[lattice_rot.x0, lattice_rot.y0]]),
                 angle,
                 rotation_origin
             ) + origin_shift).squeeze()
 
             '''Transform data'''
             tmat = rotation_matrix(angle, rotation_origin)
-            print(tmat)
 
             lattice_rot.dir_struct_matrix = (
                 lattice_rot.dir_struct_matrix
                 @ tmat[0:2, 0:2].T
             )
 
             lattice_rot.a1 = lattice_rot.dir_struct_matrix[0, :]
@@ -767,15 +767,14 @@
 
         if n_plots % ncols == 0:
             ncols_ = ncols + 1
             width_ratios += [0.4]
         else:
             ncols_ = ncols
 
-        # print(nrows, ncols_)
         gs = fig.add_gridspec(
             nrows=nrows,
             ncols=ncols_,
             width_ratios=width_ratios,
             height_ratios=[1 for _ in range(nrows)],
             wspace=0.05
         )
@@ -1068,15 +1067,15 @@
         LoG_sigma=None
         ):
         Registers a reference lattice to the image.
 
     fit_atom_columns(
         self,
         buffer=0,
-        local_thresh_factor=1,
+        bkgd_thresh_factor=1,
         peak_sharpening_filter='auto',
         peak_grouping_filter='auto',
         filter_by='elem',
         sites_to_fit='all',
         watershed_line=True,
         use_LoG_fitting=False
         ):
@@ -1375,15 +1374,15 @@
         # Downsample for speed
         if np.max([self.h, self.w]) > 2000:
             fft_der_ds = downscale_local_mean(fft_der, (2, 2))
         else:
             fft_der_ds = fft_der
         masks, num_masks, _, spots = watershed_segment(
             fft_der_ds,
-            local_thresh_factor=0,
+            bkgd_thresh_factor=0,
             buffer=2*sigma
         )
 
         # Resample
         if np.max([self.h, self.w]) > 2000:
             masks = rescale(masks, (2, 2), order=0)
             spots.loc[:, 'x':'y'] *= 2
@@ -1500,28 +1499,31 @@
         -------
         None.
 
         """
 
         if self.sigma is None:
             self.sigma = get_feature_size(self.image)
-            sigma = self.sigma
+            # sigma = self.sigma
 
         image_std = image_norm(gaussian_filter(
             std_local(self.image, r),
-            sigma=sigma)
+            sigma=self.sigma)
         )
         new_mask = np.where(image_std > thresh, 1, 0)
         if fill_holes:
             new_mask = binary_fill_holes(new_mask)
         if buffer:
-            new_mask = erosion(
-                new_mask,
-                footprint=np.ones((3, 3))
-            )
+            footprint = get_circular_kernel(1)
+
+            for _ in range(buffer):
+                new_mask = erosion(
+                    new_mask,
+                    footprint=footprint
+                )
 
         self.roi_mask *= new_mask
 
         if show_mask:
             self.show_roi_mask()
 
     def get_roi_mask_polygon(
@@ -2092,17 +2094,14 @@
         )]
 
         t = [time.time()]
 
         for i, mult in enumerate([1, 3, 9]):
             lim = mult * init_inc
 
-            # print(f'Refinement iteration {i+1}')
-
-            # if lim > init_inc:
             at_cols_orig_type[['x_ref', 'y_ref']] = (
                 at_cols_orig_type.loc[:, 'u':'v'].to_numpy(dtype=float)
                 @ self.dir_struct_matrix
                 + np.array([self.x0, self.y0])
             )
 
             filtered = at_cols_orig_type[
@@ -2144,16 +2143,14 @@
 
             self.dir_struct_matrix = params[:4].reshape((2, 2))
 
             self.x0 = params[4]
             self.y0 = params[5]
 
             t += [time.time()]
-            # print(f'{int((t[-1]-t[-2]) // 60)} min '
-            #       + f'{(t[-1]-t[-2]) % 60 :.{2}f} sec')
 
         at_cols[['x_ref', 'y_ref']] = (
             at_cols.loc[:, 'u':'v'].to_numpy(dtype=float)
             @ self.dir_struct_matrix
             + np.array([self.x0, self.y0])
         )
 
@@ -2237,25 +2234,24 @@
                 head_width=arrow_scale * 3,
                 head_length=arrow_scale * 5
             )
 
     def fit_atom_columns(
             self,
             buffer=0,
-            local_thresh_factor=0.95,
+            bkgd_thresh_factor=0.95,
             pos_toler=None,
             peak_sharpening_filter='auto',
             peak_grouping_filter='auto',
             select_sites_by='elem',
             sites_to_fit='all',
             watershed_line=True,
             parallelize=True,
             use_circ_gauss=False,
             use_bounds=False,
-            use_background_param=True,
             pos_bound_dist=None
     ):
         """Algorithm for fitting 2D Gaussians to HR STEM image.
 
         1) Laplacian of Gaussian filter applied to image to isolate individual
         atom column areas. Watershed method used to generate individual mask
         regions.
@@ -2279,19 +2275,19 @@
 
         Parameters
         ----------
         buffer : int
             Distance defining the image border used to ignore atom columns
             whose fits my be questionable.
 
-        local_thresh_factor : scalar
+        bkgd_thresh_factor : scalar
             Removes background from each segmented region by thresholding.
             Threshold value determined by finding the maximum value of edge
             pixels in the segmented region and multipling this value by the
-            local_thresh_factor value. The LoG-filtered image (with
+            bkgd_thresh_factor value. The LoG-filtered image (with
             sigma=peak_sharpening_filter) is used for this calculation.
             Default: 0.95.
 
         pos_toler : scalar or None
             The maximum allowed distance between the registered refernce
             lattice and a detected peak, in Angstroms. If greater than this
             distance, the reference lattice position will be used for the
@@ -2357,20 +2353,14 @@
             Whether to apply bounds to minimization algorithm. This may be
             needed if unphysical results are obtained (e.g. negative
             background, negative amplitude, highly elliptical fits, etc.).
             The bounded version of the minimization is slower than the
             unbounded.
             Default: False
 
-        use_background_param : bool
-            Whether to use the background parameter when fitting each atom
-            column or group of columns. If False, background value is forced
-            to be 0.
-            Default: True
-
         pos_bound_dist : 'auto' or scalar or None
             The +/- distance in Angstroms used to bound the x, y position of
             each atom column fit from its initial guess location. If 'auto',
             half the minimum seperation between atom columns in the reference
             lattice is used. If 'None', position bounds are not used.
             Argument is only functional when 'use_bounds' is set to True.
             Default: None
@@ -2383,16 +2373,14 @@
 
         print('Preparing to fit atom columns...')
 
         """Handle various settings configurations, prepare for masking
         process, and check for exceptions"""
         t = [time.time()]
         self.buffer = buffer
-        if not use_background_param:
-            use_bounds = True
 
         if self.at_cols_uncropped.shape[0] == 0:
             raise Exception(
                 "Must define lattice before running fitting routine"
             )
 
         if self.at_cols.shape[0] == 0:
@@ -2467,18 +2455,18 @@
                     "Filtering by 'sites_to_fit' resulted in no atom " +
                     "columns remaining. Check arguments."
                 )
 
         """Find minimum distance (in pixels) between atom columns for peak
         detection neighborhood"""
 
-        min_dist = self.get_min_atom_col_dist()
+        self.min_dist = self.get_min_atom_col_dist()
 
         if pos_bound_dist == 'auto':
-            pos_bound_dist = min_dist/2
+            pos_bound_dist = self.min_dist/2
         elif pos_bound_dist is None:
             pos_bound_dist = np.inf
         elif (np.isin(type(pos_bound_dist), [float, int]).item() &
               (pos_bound_dist > 0)):
             pos_bound_dist = pos_bound_dist / self.pixel_size_est
         else:
             raise Exception(
@@ -2488,30 +2476,30 @@
         t += [time.time()]
         print(f'Step 1 (Initial checks): {(t[-1]-t[-2]) :.{2}f} sec')
 
         """Use Watershed segmentation with LoG filtering to generate fitting
         masks"""
         peak_masks, num_peak_masks, slices_LoG, xy_peak = watershed_segment(
             img_LoG,
-            local_thresh_factor=local_thresh_factor,
+            bkgd_thresh_factor=bkgd_thresh_factor,
             watershed_line=watershed_line,
-            min_dist=min_dist * 0.75
+            min_dist=self.min_dist * 0.75
         )
 
         t += [time.time()]
         print(f'Step 2 (fitting masks): {(t[-1]-t[-2]) :.{2}f} sec')
 
         """Use Watershed segmentation with Gaussian blur to group columns for
         simultaneous fitting"""
         if peak_grouping_filter is not None:
             group_masks, _, _, _ = watershed_segment(
                 img_gauss,
-                local_thresh_factor=0,
+                bkgd_thresh_factor=0,
                 watershed_line=watershed_line,
-                min_dist=min_dist
+                min_dist=self.min_dist
             )
 
             t += [time.time()]
             print(f'Step 3 (grouping masks): {(t[-1]-t[-2]) :.{2}f} sec')
 
         else:
             group_masks = peak_masks
@@ -2524,14 +2512,16 @@
         xy_ref = at_cols.loc[:, 'x_ref':'y_ref'].to_numpy(dtype=float)
         inds = np.array(
             [np.argmin(norm(xy_peak - xy, axis=1)) for xy in xy_ref]
         )
         xy_peak = np.array([xy_peak[ind, :] for ind in inds])
         slices_LoG = [slices_LoG[ind] for ind in inds]
 
+        self.slices_LoG = slices_LoG
+
         """If the difference between detected peak position and reference
         position is greater than the position tolerance, the reference is taken
         as the initial guess."""
 
         """*** OR now we will just throw them out???"""
         if pos_toler is None:
             pos_toler = peak_sharpening_filter
@@ -2614,28 +2604,28 @@
         ]
 
         group_slices = [np.s_[
             np.min(group[0]): np.max(group[1]),
             np.min(group[2]): np.max(group[3])]
             for group in group_fit_slices
         ]
+        self.group_slices = group_slices
 
         """Pack image slices and metadata together for the fitting routine"""
 
         args_packed = pack_data_prefit(
             data=self.image,
             slices=group_slices,
             masks=peak_masks,
             xy_peaks=xy_peak,
             peak_mask_index=peak_masks_to_peaks,
             peak_groups=peak_groups,
             pos_bound_dist=pos_bound_dist,
             use_circ_gauss=use_circ_gauss,
             use_bounds=use_bounds,
-            use_background_param=use_background_param,
         )
 
         self.args_packed = args_packed
 
         at_cols_inds = at_cols.index.to_numpy(dtype=float)
         self.at_cols_inds = at_cols_inds
 
@@ -3424,15 +3414,15 @@
             else:
                 pcf_sm = copy.deepcopy(vpcf)
                 sigma = 2
 
             masks_indiv, n_peaks, _, peaks = watershed_segment(
                 pcf_sm,
                 min_dist=sigma,
-                local_thresh_factor=0,
+                bkgd_thresh_factor=0,
                 sigma=None,
                 buffer=buffer,
                 watershed_line=False,
             )
 
             peaks['peak_max'] = vpcf[
                 peaks.loc[:, 'y'].to_numpy(dtype=int),
@@ -3457,15 +3447,15 @@
                     sigma=sigma_group,
                     truncate=3
                 )
 
                 group_masks, _, _, _ = watershed_segment(
                     pcf_sm,
                     min_dist=sigma_group,
-                    local_thresh_factor=0,
+                    bkgd_thresh_factor=0,
                     sigma=None,
                     buffer=0,
                     watershed_line=True
                 )
 
                 group_masks_to_peaks = map_coordinates(
                     group_masks,
@@ -3548,20 +3538,20 @@
                                    (None, None),
                                    (0, None),
                                    ]
 
                     p0 = np.array(p0 + [0])
                     bounds += [(0, 0)]
 
-                    params = fit_gaussian_ellip(
+                    params = fit_gaussians(
                         pcf_masked,
                         p0,
-                        masks=None,
                         method='L-BFGS-B',
-                        bounds=bounds
+                        bounds=bounds,
+                        shape='ellip'
                     )
 
                     params = params[:, :-1]
                     params[:, 3] = params[:, 2] / params[:, 3]
                     params[:, 4] = np.degrees(params[:, 4])
                     params[:, -1] = np.sqrt(1 - params[:, 3]**2
                                             / params[:, 2]**2)
@@ -3978,16 +3968,14 @@
 
         vects, str1, str2 = self.get_vector_from_vpcf(
             vpcf,
             number_of_peaks_to_pick=number_of_peaks_to_pick,
             plot_equ_ellip=plot_equ_ellip,
         )
 
-        # print(vects)
-
         if dist_along_vector is not None:
             dist_along_vector = dist_along_vector.reshape(-1, 2)
             if dist_along_vector.shape[0] != number_of_peaks_to_pick:
                 raise Exception(
                     'argument "dist_along_vector" must a vector for each peak '
                     + 'that will be picked. That is, if '
                     + 'number_of_peaks_to_pick=n, "dist_along_vector" must '
```

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/measure_lattice.py` & `singleorigin-2.5.7/src/SingleOrigin/measure_lattice.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,20 @@
     solve,
 )
 
 import pandas as pd
 
 from scipy.ndimage import center_of_mass, gaussian_filter
 
-from sklearn.cluster import MiniBatchKMeans
-from skimage.morphology import erosion
+from sklearn.cluster import KMeans
+from skimage.morphology import erosion, dilation
 
 from matplotlib import pyplot as plt
 from matplotlib.patches import Rectangle, Circle
+from matplotlib.colors import LogNorm, PowerNorm
 
 from SingleOrigin.utils import (
     image_norm,
     detect_peaks,
     get_feature_size,
     pick_points,
     register_lattice_to_peaks,
@@ -57,15 +58,17 @@
     hann_2d,
     fit_lattice,
     metric_tensor,
     get_astar_2d_matrix,
     rotation_angle_bt_vectors,
     absolute_angle_bt_vectors,
     watershed_segment,
-    fft_square
+    fft_square,
+    plane_fit,
+    plane_2d,
 )
 
 from SingleOrigin.cell_transform import UnitCell
 
 
 class ReciprocalLattice:
 
@@ -197,27 +200,27 @@
                 self.data,
                 upsample_factor=upsample_factor)
 
             self.ewpc_mean = np.mean(
                 self.ewpc,
                 axis=(0, 1),
             )
-            display_image = self.ewpc_mean
+            im_display = self.ewpc_mean
 
         else:
-            display_image = self.data_mean
+            im_display = self.data_mean
 
         if upsample_factor is not None:
             self.origin_shift = self.scan_w * (upsample_factor - 1) / 2
             self.dp_h *= upsample_factor
             self.dp_w *= upsample_factor
 
         if show_mean_image:
             fig, ax = plt.subplots(1)
-            ax.imshow(np.log(display_image), cmap='gray')
+            ax.imshow(im_display, cmap='gray', norm=LogNorm())
             if self.origin is not None:
                 ax.scatter(*self.origin, c='red', marker='+')
 
     def kmeans_segmentation_ewpc(self, n_clusters, window=4):
         """
         Segment scan using kmeans over the ewpc patterns.
 
@@ -244,15 +247,15 @@
         ewpc[:, :, 64-window:64+window+1, 64-window:64+window+1] = 0
 
         # Prepare kmeans analysis
         X_train = ewpc.reshape((-1, 128*128))**0.5
         X_train -= np.min(X_train)
         X_train /= np.max(X_train)
 
-        kmeans = MiniBatchKMeans(n_clusters=n_clusters)
+        kmeans = KMeans(n_clusters=n_clusters)
         kmeans.fit(X_train)
         self.kmeans_labels = kmeans.labels_.reshape((self.scan_h, self.scan_w))
         plt.imshow(self.kmeans_labels)
 
     def initalize_ewpc_analysis(
         self,
         pick_basis_order=(1, 1),
@@ -1240,22 +1243,24 @@
 
         return beta
 
     def initalize_bragg_lattice(
         self,
         a1_order=1,
         a2_order=1,
-        sigma=3,
+        sigma=None,
         buffer=5,
-        thresh_factor_std=1,
         detection_thresh='auto',
-        peak_max_thresh_factor=0.1,
+        peak_bkgd_thresh_factor=0.1,
+        fit_bkgd=False,
         max_order=5,
-        verbose=True,
         show_fit=True,
+        verbose=True,
+        logscale=True,
+        pwrscale=None,
     ):
         """Find peaks in a reciprocal lattice image (i.e. FFT or diffraction
         pattern) and get the reciprocal lattice parameters.
 
         Peaks locations are determined by center-of-mass applied to the
         surrounding region as found using the watershed method. A best-fit
         lattice is then registered to the set of located peaks. This procedure
@@ -1265,43 +1270,38 @@
         Parameters
         ----------
         a1_order, a2_order : ints
             The order of the first peak along the a1* and a2* directions.
             (e.g.: if the first spot corresponds to an (002) reflection, then
              set equal to 2.)
 
-        sigma : int or float
+        sigma : scalar or 'auto'
             The Laplacian of Gaussian sigma value to use for sharpening of the
-            peaks for the peak finding algorithm. Usually a value between 2
+            peaks for the peak finding algorithm. If None, automatic feature
+            size detection will be used.
+            Usually a value between 2
             and 10 will work well.
 
         buffer : scalar
             Distance defining the edge border outside which peaks will be
             ignored.
 
-        thresh_factor_std : scalar
-            Relative adjustment of the threshold level for detecting peaks.
-            Greater values will detect fewer peaks; smaller values, more.
-            The thresholding is done based on the standard deviation of the
-            peak and its surrounding area with the assumption that : dim or
-            noise peaks will have low standard deviations.
-            Default: 1.
-
         detection_thresh : scalar or str
-            The threshold (in % max image intensity) of peak amplitude to
+            The threshold (in % max data intensity) of peak maxima to
             consider as a possible reciprocal lattice spot. Used to remove
-            noise peaks with high local standard devaition from being detected
-            as Bragg peaks. If 'auto' is passed, determined as 2 * the image
-            mean.
-
-        peak_max_thresh_factor : scalar
-            Thresholding factor applied to the watershed region of each peak.
-            Threshold value for each peak determined as:
-                peak_max_thresh_factor * (peak_max - edge_max) + edge_max.
-            Where edge_max is the maximum value of the edge pixels of the
+            low intensity peaks. If 'auto' is passed, determined as the mean
+            intensity of the data.
+            Default: 'auto'
+
+        peak_bkgd_thresh_factor : scalar
+            Thresholding factor applied to remove background pixels from the
+            watershed region of each peak. Threshold value for each peak
+            determined as:
+                peak_bkgd_thresh_factor * (peak_max - edge_max) + edge_max.
+            Where edge_max is the maximum value of the edge pixels in the
             watershed region and peak_max is the maximum of the region. This
             This value should be [0 : ~0.8]. The method ensures that the
             threshold is above the local background and prevents an asymmetric
             region being used for center-of-mass determination.
             Default: 0.1.
 
         max_order : int
@@ -1312,122 +1312,174 @@
             Whether to show the fitted Bragg lattice.
             Default: True
 
         verbose : bool
             Whether to print lattice fitting information to the console.
             Default: True
 
+        logscale : bool
+            Whether to log scale the displayed pattern intensities for
+            diffraction patterns. No effect on measurements.
+            Default: True.
+
+        pwrscale : scalar or None
+            If a scalar and logscale is False, will apply a power scaling
+            (e.g. 0.5) to the displayed pattern intensity for diffraction
+            patterns. No effect on measurements. If None, no scaling.
+            Default: None.
+
         Returns
         -------
         ...
 
         """
 
         if self.datatype == 'image':
             # pwr_factor = 0.2
             n_picks = 2
             fix_origin = True
             log_fft = np.log(fft_square(self.data_mean))
-            # display_im = image_norm(gaussian_filter(log_fft, sigma))
-            display_im = image_norm(log_fft)
-            U = display_im.shape[0] // 2
+            im_meas = im_display = image_norm(log_fft + 1e-6)
+            U = im_display.shape[0] // 2
             origin = np.array([U, U])
+            imnorm = None
 
         elif self.datatype == 'dp':
             n_picks = 3
             fix_origin = False
-            # pwr_factor = 0.2
-            display_im = image_norm(self.data_mean)
+            im_meas = self.data_mean
+            if logscale:
+                imnorm = LogNorm()
+            elif pwrscale is not None:
+                imnorm = PowerNorm(pwrscale)
+            else:
+                imnorm = None
         else:
             raise Exception(
                 "'datatype' must be 'image' or 'dp'."
             )
 
         if detection_thresh == 'auto':
-            detection_thresh = np.mean(display_im)
+            detection_thresh = np.mean(im_meas)
 
-        h, w = display_im.shape
+        h, w = im_meas.shape
 
-        if sigma is None:
+        if sigma == 'auto':
             peak_map = detect_peaks(
-                copy.deepcopy(display_im),
+                im_meas,
                 min_dist=4,
                 thresh=0
             )
 
             # Find the max of the 2nd highest peak (ignores the central peak)
-            vmax = np.unique(peak_map*display_im)[-2]
+            vmax = np.unique(peak_map*im_meas)[-2]
 
             # Get feature size after applying vmax as a maximum threshold.
             # This prevents the central peak from dominating the size
             # determination vmax will also be used as the upper limit of the
             # imshow cmap.
 
             image_thresh = np.where(
-                display_im > vmax,
-                0,
-                display_im
+                im_meas > vmax,
+                vmax,
+                im_meas
             )
 
-            min_dist = get_feature_size(image_thresh)
-            if min_dist < 3:
-                min_dist = 3
-            sigma = min_dist
-            self.sigma = min_dist
+            self.sigma = get_feature_size(image_thresh)
+            if self.sigma < 1:
+                self.sigma = 1
 
         else:
-            min_dist = sigma
             self.sigma = sigma
 
+        im_filt = gaussian_filter(im_meas, self.sigma)
+
         masks, num_masks, _, peaks = watershed_segment(
-            display_im,
-            local_thresh_factor=0,
-            peak_max_thresh_factor=peak_max_thresh_factor,
+            im_filt,
+            sigma=None,
+            bkgd_thresh_factor=0,
+            peak_bkgd_thresh_factor=peak_bkgd_thresh_factor,
             buffer=buffer,
-            min_dist=min_dist
+            min_dist=self.sigma,
+            min_pixels=self.sigma * 2,
         )
-        peaks = peaks[peaks.loc[:, 'max'] > detection_thresh]
 
         # Remove edge pixels:
         if buffer > 0:
             peaks = peaks[
                 ((peaks.x >= buffer) &
                  (peaks.x <= self.dp_w - buffer) &
                  (peaks.y >= buffer) &
                  (peaks.y <= self.dp_h - buffer))
             ].reset_index(drop=True)
 
-        peaks['stdev'] = [
-            np.std(display_im[
-                int(np.max([y-sigma, 0])):int(np.min([y+sigma+1, self.dp_h])),
-                int(np.max([x-sigma, 0])):int(np.min([x+sigma+1, self.dp_w]))
-            ])
-            for [x, y]
-            in np.around(peaks.loc[:, 'x':'y']).to_numpy(dtype=int)
-        ]
+        # # Update peaks DataFrame with unfiltered data values (std, max, min)
+        self.all_peaks = copy.deepcopy(peaks)
+        for i, peak in peaks.iterrows():
+            mask = np.where(masks == peak.label, 1, 0)
+            peak_masked = mask * im_meas
+
+            peaks.at[i, 'stdev'] = np.std(peak_masked[peak_masked > 0]
+                                          ).astype(float)
+            peaks.at[i, 'max'] = np.max(peak_masked[peak_masked > 0]
+                                        ).astype(float)
+            peaks.at[i, 'mean'] = np.mean(peak_masked[peak_masked > 0]
+                                          ).astype(float)
+
+            mask_bkgd = dilation(mask, footprint=np.ones((3, 3))) - mask
+            bkgd_masked = im_meas * mask_bkgd
+            peaks.at[i, 'min'] = np.mean(bkgd_masked[bkgd_masked > 0]
+                                         ).astype(float)
 
-        thresh = 0.003 * thresh_factor_std
-
-        if thresh > 0:
-            peaks = peaks[
-                (peaks.loc[:, 'stdev'] > thresh) &
-                (peaks.loc[:, 'max'] > detection_thresh)
-            ].reset_index(drop=True)
+        peaks = peaks[peaks.loc[:, 'max'] > detection_thresh
+                      ].reset_index(drop=True)
 
         xy = peaks.loc[:, 'x':'y'].to_numpy(dtype=float)
+        xy.shape
+
+        y, x = np.indices(im_meas.shape)
+
         for i, xy_ in enumerate(xy):
             mask_num = masks[int(xy_[1]), int(xy_[0])]
             mask = np.where(masks == mask_num, 1, 0)
-            com = np.flip(center_of_mass(display_im*mask))
-            peaks.loc[i, ['x_com', 'y_com']] = com
+            masked_peak = im_meas*mask
+            if fit_bkgd:
+                bkgd_mask = dilation(mask) - mask
+                bkgd_int = bkgd_mask * im_meas
+
+                params = plane_fit(
+                    bkgd_int,
+                    p0=[0, 0, np.mean(bkgd_int)]
+                )
+                bkgd = plane_2d(x, y, *params)
+                masked_peak = np.where(mask > 0, masked_peak - bkgd, 0)
 
-        xy = peaks.loc[:, 'x':'y'].to_numpy(dtype=float)
+                # Make sure no (-) numbers and residual background removed
+                min_ = np.min(masked_peak[masked_peak != 0])
+                masked_peak = (masked_peak - min_) * mask
+
+            else:
+                min_ = np.min(masked_peak[masked_peak > 0])
+                masked_peak = (masked_peak - min_) * mask
+
+            masked_peak[masked_peak < 0] = 0
+
+            if np.sum(masked_peak) > 0:
+                com = np.flip(center_of_mass(masked_peak))
+                peaks.loc[i, ['x_com', 'y_com']] = com
+
+        peaks = peaks.dropna()
+
+        xy = peaks.loc[:, 'x_com':'y_com'].to_numpy(dtype=float)
+
+        self.all_peaks = copy.copy(peaks)
+        self.masks = masks
 
         fig, ax = plt.subplots(figsize=(10, 10))
-        ax.imshow((display_im)**(0.5), cmap='gray')
+        ax.imshow(im_meas, cmap='gray', norm=imnorm)
         ax.scatter(xy[:, 0], xy[:, 1], c='red', marker='+')
         if self.datatype == 'fft':
             ax.scatter(origin[0], origin[1], c='white', marker='+')
             fig.suptitle(
                 'Pick peaks for the a1* and a2* reciprocal basis vectors' +
                 ' \n in that order).',
                 fontsize=12,
@@ -1483,36 +1535,53 @@
         inds = np.argmin(norm(vects, axis=2), axis=1)
 
         self.recip_latt = pd.DataFrame({
             'h': recip_latt_indices[:, 0],
             'k': recip_latt_indices[:, 1],
             'x_ref': xy_ref[:, 0],
             'y_ref': xy_ref[:, 1],
-            'x_max': [xy[ind, 0] for ind in inds],
-            'y_max': [xy[ind, 1] for ind in inds],
+            'x_com': [xy[ind, 0] for ind in inds],
+            'y_com': [xy[ind, 1] for ind in inds],
+            'stdev': [peaks.loc[:, 'stdev'].to_numpy()[ind] for ind in inds],
+            'max': [peaks.loc[:, 'max'].to_numpy()[ind] for ind in inds],
             'mask_ind': inds
         })
 
         # Remove peaks that are too far from initial reciprocal lattice
-        self.recip_latt = self.recip_latt[norm(
-            self.recip_latt.loc[:, 'x_max':'y_max'].to_numpy(dtype=float)
-            - self.recip_latt.loc[:, 'x_ref':'y_ref'].to_numpy(dtype=float),
-            axis=1
-        ) < np.max([0.1*np.max(norm(a_star, axis=1)), 1.5])
-        ].reset_index(drop=True)
+        xy_com = self.recip_latt.loc[:, 'x_com':'y_com'].to_numpy(dtype=float)
+        xy_ref = self.recip_latt.loc[:, 'x_ref':'y_ref'].to_numpy(dtype=float)
+
+        nearest = np.where(
+            norm(xy_com - xy_ref, axis=1)
+            < np.max([0.1*np.max(norm(a_star, axis=1)), 1.5]),
+            True, False)
+
+        self.recip_latt.loc[:, 'x_com':'y_com'] = np.array([
+            xy_com[i] if match else [np.nan, np.nan]
+            for i, match in enumerate(nearest)
+        ])
 
         # Refine reciprocal basis vectors
-        M_star = self.recip_latt.loc[:, 'h':'k'].to_numpy(dtype=float)
-        xy = self.recip_latt.loc[:, 'x_max':'y_max'].to_numpy(dtype=float)
+
+        xy = self.recip_latt.loc[:, 'x_com':'y_com'].to_numpy(dtype=float)
+        xy_nonan = np.isfinite(xy)[:, 0]
+        xy = xy[xy_nonan]
+        M_star = self.recip_latt.loc[:, 'h':'k'
+                                     ].to_numpy(dtype=float)[xy_nonan]
 
         p0 = np.concatenate((a_star.flatten(), origin))
 
-        params = fit_lattice(p0, xy, M_star, fix_origin=fix_origin)
+        params = fit_lattice(
+            p0,
+            xy,
+            M_star,
+            fix_origin=fix_origin,
+        )
 
-        # Save data and report key values
+        # Recalculate reference lattice points
         self.a1_star = params[:2]
         self.a2_star = params[2:4]
         if len(params) == 6:
             self.origin = params[4:]
         else:
             self.origin = origin
 
@@ -1521,14 +1590,22 @@
 
         self.recip_latt[['x_ref', 'y_ref']] = (
             self.recip_latt.loc[:, 'h':'k'].to_numpy(dtype=float)
             @ self.a_star
             + self.origin
         )
 
+        # Remove lattice points outside image bounds
+        self.recip_latt = self.recip_latt[(
+            (self.recip_latt.x_ref >= 0) &
+            (self.recip_latt.x_ref <= self.dp_w-1) &
+            (self.recip_latt.y_ref >= 0) &
+            (self.recip_latt.y_ref <= self.dp_h-1)
+        )]
+
         theta = absolute_angle_bt_vectors(
             self.a1_star,
             self.a2_star,
             np.identity(2)
         )
 
         ratio = norm(self.a1_star)/norm(self.a2_star)
@@ -1536,26 +1613,28 @@
         if verbose:
             print(f'Reciproal lattice angle (degrees): {theta :.{3}f}')
             print(f'Reciproal vector ratio (a1*/a2*): {ratio :.{5}f}')
 
         # Plot refined basis
         if show_fit:
             fig2, ax = plt.subplots(figsize=(10, 10))
-            ax.imshow(display_im**0.2, cmap='plasma')
+            ax.imshow(im_meas, cmap='plasma', norm=imnorm)
             ax.scatter(
                 self.recip_latt.loc[:, 'x_ref'].to_numpy(dtype=float),
                 self.recip_latt.loc[:, 'y_ref'].to_numpy(dtype=float),
                 marker='+',
-                c='red'
+                c='red',
+                # s=100
             )
             ax.scatter(
-                self.recip_latt.loc[:, 'x_max'].to_numpy(dtype=float),
-                self.recip_latt.loc[:, 'y_max'].to_numpy(dtype=float),
-                marker='+',
-                c='black'
+                self.recip_latt.loc[:, 'x_com'].to_numpy(dtype=float),
+                self.recip_latt.loc[:, 'y_com'].to_numpy(dtype=float),
+                marker='o',
+                fc='none',
+                ec='black'
             )
             ax.scatter(self.origin[0], self.origin[1], marker='+', c='white')
 
             ax.arrow(
                 self.origin[0],
                 self.origin[1],
                 self.a1_star[0],
@@ -1584,24 +1663,28 @@
                 ax.set_xlim(np.min(self.recip_latt.loc[:, 'x_ref']) - 100,
                             np.max(self.recip_latt.loc[:, 'x_ref']) + 100)
                 ax.set_ylim(np.max(self.recip_latt.loc[:, 'y_ref']) + 100,
                             np.min(self.recip_latt.loc[:, 'y_ref']) - 100)
 
             ax.set_xticks([])
             ax.set_yticks([])
+            # ax.set_xlim(0, self.dp_w-1)
+            # ax.set_ylim(self.dp_h-1, 0)
             plt.title('Reciprocal Lattice Fit')
 
     def initalize_superlattice(
         self,
         n_superlatt=1,
         superlatt_order=(1,),
         min_order=1,
-        max_order=2,
+        max_order=1,
         show_fit=True,
         verbose=True,
+        logscale=True,
+        pwrscale=None,
     ):
         """Find superlattice peaks relative to previously located Bragg peaks.
 
         Uses previously detected peaks in diffraction pattern, so make sure
         the desired superlattice peaks were found in the initialize_lattice
         step.
 
@@ -1635,89 +1718,101 @@
         ...
 
         """
 
         if min_order < 1:
             min_order = 1
 
+        if (len(superlatt_order) != n_superlatt) & (superlatt_order == (1,)):
+            superlatt_order *= n_superlatt
+
+        elif len(superlatt_order) != n_superlatt:
+            raise Exception('len(superlatt_order) must equal n_superlatt')
+
         if self.datatype == 'image':
             n_picks = n_superlatt
             U = self.h // 2
-            display_im = fft_square(self.data_mean)
-            U = display_im.shape[0] // 2
+            im_meas = fft_square(self.data_mean)
+            U = im_meas.shape[0] // 2
             origin = np.array([U, U])
+            imnorm = None
 
         elif self.datatype == 'dp':
-            n_picks = n_superlatt + 1
-            display_im = self.data_mean
+            n_picks = 2 * n_superlatt
+            im_meas = self.data_mean
+            if logscale:
+                imnorm = LogNorm()
+            elif pwrscale is not None:
+                imnorm = PowerNorm(pwrscale)
+            else:
+                imnorm = None
+
         else:
             raise Exception(
                 "'datatype' must be 'image' or 'dp'."
             )
 
-        h, w = display_im.shape
+        h, w = im_meas.shape
 
-        xy = self.all_peaks
+        xy = self.all_peaks.loc[:, 'x':'y'].to_numpy()
 
         # Get vmin for plotting (helps with dead camera pixels)
-        vmin = np.max([np.mean(display_im) - 5*np.std(display_im), 0])
+        # vmin = np.max([np.mean(im_meas) - 1*np.std(im_meas), 0])
 
         if n_picks > 0:
             fig, ax = plt.subplots(figsize=(10, 10))
-            ax.imshow(display_im, cmap='plasma', vmin=vmin)
+            ax.imshow(im_meas, cmap='plasma', norm=imnorm)
             ax.scatter(xy[:, 0], xy[:, 1], c='black', marker='+')
             ax.scatter(
                 self.recip_latt.loc[:, 'x_ref'],
                 self.recip_latt.loc[:, 'y_ref'],
                 ec='white',
                 fc='none',
                 marker='o',
                 s=100,
             )
 
             if self.datatype == 'image':
                 ax.scatter(origin[0], origin[1], c='white', marker='+')
                 fig.suptitle(
-                    'Pick peaks for the a1* and a2* reciprocal basis vectors' +
-                    ' \n in that order).',
+                    'Pick peaks for the q1, q2, etc. superlattice vectors',
                     fontsize=12,
                     c='black',
                 )
 
             elif self.datatype == 'dp':
                 fig.suptitle(
-                    'Pick peaks for the origin, a1* and a2* reciprocal basis' +
-                    ' \n vectors (in that order).',
+                    'Pick a Bragg peak followed by a corresponding ' +
+                    'superlattice peak. Repeat for each superlattice.',
                     fontsize=12,
                     c='black',
                 )
 
             ax.set_xticks([])
             ax.set_yticks([])
 
             if self.datatype == 'image':
                 ax.set_xlim(np.min(xy[:, 0]) - 100, np.max(xy[:, 0]) + 100)
                 ax.set_ylim(np.max(xy[:, 1]) + 100, np.min(xy[:, 1]) - 100)
 
-            basis_picks_xy = np.array(plt.ginput(n_picks, timeout=30))
+            basis_picks_xy = np.array(plt.ginput(n_picks, timeout=60))
 
             plt.close('all')
 
         # Match peaks to  click points to get reciprocal superspace basis
         vects = np.array([xy - i for i in basis_picks_xy])
         inds = np.argmin(norm(vects, axis=2), axis=1)
         basis_picks_xy = xy[inds, :]
 
         if self.datatype == 'dp':
-            origin = basis_picks_xy[0, :]
 
-        a_4_star = np.array([
-            (basis_picks_xy[i+1, :] - origin) / superlatt_order[i]
-            for i in range(n_superlatt)
-        ])
+            origin = basis_picks_xy[::2, :]
+            suplat = basis_picks_xy[1::2, :]
+
+        a_4_star = (suplat - origin) / np.array(superlatt_order)[:, None]
 
         super_latt_indices = np.array([
             i for i in range(-max_order, max_order+1) if np.abs(i) >= min_order
         ])
 
         # Make array of all superlattice reflection vectors to max_order
         q_vects = a_4_star[:, :, None] * super_latt_indices
@@ -1755,35 +1850,35 @@
         q_order = np.concatenate([q_order] * xy_bragg.shape[0]).T
 
         self.recip_suplatt = pd.DataFrame({
             'h': h_inds,
             'k': k_inds,
             'x_ref': q_pos[:, 0],
             'y_ref': q_pos[:, 1],
-            'x_max': [xy[ind, 0] for ind in inds],
-            'y_max': [xy[ind, 1] for ind in inds],
+            'x_com': [xy[ind, 0] for ind in inds],
+            'y_com': [xy[ind, 1] for ind in inds],
         })
 
         for i, col in enumerate(q_order):
             self.recip_suplatt[q_keys[i]] = col
 
         # Remove peaks that are too far from initial reciprocal lattice
         self.recip_suplatt = self.recip_suplatt[norm(
-            self.recip_suplatt.loc[:, 'x_max':'y_max'].to_numpy(dtype=float)
+            self.recip_suplatt.loc[:, 'x_com':'y_com'].to_numpy(dtype=float)
             - self.recip_suplatt.loc[:, 'x_ref':'y_ref'].to_numpy(dtype=float),
             axis=1
         ) < 0.1*np.max(norm(a_4_star, axis=1))
         ].reset_index(drop=True)
 
         # Refine reciprocal basis vectors
         M_star = self.recip_suplatt.loc[:, 'h': 'k'].to_numpy(dtype=float)
 
         xy_bragg = M_star @ self.a_star + self.origin
 
-        q_vect_xy = self.recip_suplatt.loc[:, 'x_max': 'y_max'
+        q_vect_xy = self.recip_suplatt.loc[:, 'x_com': 'y_com'
                                            ].to_numpy(dtype=float) - xy_bragg
 
         q_order = self.recip_suplatt.loc[:, q_keys[0]:q_keys[-1]
                                          ].to_numpy(dtype=float)
 
         p0 = np.concatenate((a_4_star.flatten(), np.array([0, 0])))
 
@@ -1792,107 +1887,111 @@
         # Save data and report key values
         self.a_4_star = params[:n_superlatt*2].reshape((n_superlatt, 2))
 
         self.recip_suplatt[['x_ref', 'y_ref']] = (
             q_order @ self.a_4_star + xy_bragg
         )
 
-        theta_super = [absolute_angle_bt_vectors(
-            self.a_4_star[i],
-            self.a_4_star[int((i+1) % n_superlatt)],
-            np.identity(2))
-            for i in range(n_superlatt)
-        ]
+        if n_superlatt > 1:
+            theta_super = [absolute_angle_bt_vectors(
+                self.a_4_star[i],
+                self.a_4_star[int((i+1) % n_superlatt)],
+                np.identity(2))
+                for i in range(n_superlatt)
+            ]
 
         self.theta_bragg_to_super = [rotation_angle_bt_vectors(
             self.a1_star, self.a_4_star[i], np.identity(2))
             for i in range(n_superlatt)
         ]
 
         ratios = np.around(
             [norm(self.a_4_star[i]) /
-             norm(self.a_4_star[int((i+1) % n_superlatt)])
+             norm(self.a_star, axis=1)
              for i in range(n_superlatt)],
             decimals=5
         )
 
         if verbose:
-            print(
-                'Rotation angles between superlattice vectors (degrees): ',
-                f'{theta_super}.'
-            )
+            if n_superlatt > 1:
+                print(
+                    'Rotation angles between superlattice vectors (degrees): ',
+                    f'{theta_super}.'
+                )
+
             print(
                 'Superlattice rotation angle from a1_star (degrees): ',
                 f'{self.theta_bragg_to_super}.'
             )
-            print(f'Superlattice vector ratios: {ratios}')
+            print(f'a1 : q norm ratios: {ratios}')
 
         # Plot refined basis
         if show_fit:
             fig2, ax = plt.subplots(figsize=(10, 10))
-            ax.imshow(display_im, cmap='plasma', vmin=vmin)
+            ax.imshow(im_meas, cmap='plasma', norm=imnorm)
             ax.scatter(
-                self.recip_suplatt.loc[:, 'x_max'].to_numpy(dtype=float),
-                self.recip_suplatt.loc[:, 'y_max'].to_numpy(dtype=float),
+                self.recip_suplatt.loc[:, 'x_ref'].to_numpy(dtype=float),
+                self.recip_suplatt.loc[:, 'y_ref'].to_numpy(dtype=float),
                 marker='+',
                 c='red',
-                label='Superlattice Peaks'
+                label='Superlattice Fit'
             )
             ax.scatter(
-                self.recip_latt.loc[:, 'x_max'].to_numpy(dtype=float),
-                self.recip_latt.loc[:, 'y_max'].to_numpy(dtype=float),
+                self.recip_latt.loc[:, 'x_ref'].to_numpy(dtype=float),
+                self.recip_latt.loc[:, 'y_ref'].to_numpy(dtype=float),
                 marker='+',
                 c='black',
-                label='Bragg Peaks'
+                label='Bragg Lattice Fit'
             )
             ax.scatter(self.origin[0], self.origin[1], marker='+', c='white')
 
             ax.arrow(
                 self.origin[0],
                 self.origin[1],
                 self.a1_star[0],
                 self.a1_star[1],
                 fc='black',
                 ec='black',
                 width=1,
                 length_includes_head=True,
-                head_width=10,
-                head_length=15
+                # head_width=10,
+                # head_length=15
             )
             ax.arrow(
                 self.origin[0],
                 self.origin[1],
                 self.a2_star[0],
                 self.a2_star[1],
                 fc='black',
                 ec='black',
                 width=1,
                 length_includes_head=True,
-                head_width=10,
-                head_length=15
+                # head_width=10,
+                # head_length=15
             )
 
             for q in self.a_4_star:
                 ax.arrow(
                     self.origin[0],
                     self.origin[1],
                     q[0],
                     q[1],
                     fc='red',
                     ec='red',
                     width=1,
                     length_includes_head=True,
-                    head_width=10,
-                    head_length=15
+                    # head_width=10,
+                    # head_length=15
                 )
 
             if self.datatype == 'image':
                 ax.set_xlim(np.min(self.recip_suplatt.loc[:, 'x_ref']) - 100,
                             np.max(self.recip_suplatt.loc[:, 'x_ref']) + 100)
                 ax.set_ylim(np.max(self.recip_suplatt.loc[:, 'y_ref']) + 100,
                             np.min(self.recip_suplatt.loc[:, 'y_ref']) - 100)
 
             ax.set_xticks([])
             ax.set_yticks([])
+            ax.legend()
             plt.title('Superlattice Fit')
 
 # TODO: Add functions to analize lattice and superlattice over series or scan
```

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin/utils.py` & `singleorigin-2.5.7/src/SingleOrigin/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,23 @@
 import warnings
 import io
 import json
 from contextlib import redirect_stdout
 from tqdm import tqdm
 
 import numpy as np
+from numpy import exp, sin, cos
 from numpy.linalg import norm, lstsq
 
 import pandas as pd
 
 from matplotlib import pyplot as plt
+from matplotlib.backend_bases import MouseButton
+from matplotlib.colors import LogNorm, PowerNorm
+
 
 from matplotlib_scalebar.scalebar import ScaleBar
 
 from scipy.signal import convolve2d
 from scipy.optimize import minimize
 
 from scipy.ndimage import (
@@ -45,32 +49,30 @@
     maximum_filter,
     fourier_shift,
     center_of_mass,
     binary_fill_holes,
     binary_dilation,
 )
 from scipy.interpolate import make_interp_spline
-from scipy.fft import (fft2, fftshift)
+from scipy.fft import (fft2, ifft2, fftshift)
 
 from PyQt5.QtWidgets import QFileDialog as qfd
 
 import imageio
 
 import hyperspy.api as hs
 
 from ncempy.io.dm import dmReader
 from ncempy.io.ser import serReader
 from ncempy.io.emdVelox import fileEMDVelox
 from ncempy.io.emd import emdReader
 
 from skimage.segmentation import watershed
-from skimage.morphology import binary_erosion  # erosion
+from skimage.morphology import binary_erosion, erosion
 from skimage.draw import polygon2mask
-
-
 from skimage.measure import (moments, moments_central)
 from skimage.feature import hessian_matrix_det
 
 from tifffile import imwrite
 
 pkg_dir, _ = os.path.split(__file__)
 
@@ -78,15 +80,15 @@
 
 
 """Error message string(s)"""
 no_mask_error = (
     "Float division by zero during moment estimation. No image intensity "
     + "columns, this means that no pixel region was found for fitting of at "
     + "least one atom column. This situation may result from: \n"
-    + "1) Too high a 'local_thresh_factor' value resulting in no pixels "
+    + "1) Too high a 'bkgd_thresh_factor' value resulting in no pixels "
     + "remaining for some atom columns. Check 'self.fit_masks' to see if some "
     + "atom columns do not have mask regions. \n "
     + "2) Due to mask regions splitting an atom column as a result of too "
     + "small or too large a value used for 'grouping_filter' or 'diff_filter'."
     + " Check 'self.group_masks' and 'self.fit_masks' to see if this may be "
     + "occuring. Too small a 'fitting_filter' value may cause noise peaks to "
     + "be detected, splitting an atom column. Too large a value for either "
@@ -117,17 +119,17 @@
         The metric tensor
 
     """
 
     [alpha, beta, gamma] = np.radians([alpha, beta, gamma])
 
     g = np.array(
-        [[a**2, a*b*np.cos(gamma), a*c*np.cos(beta)],
-         [b*a*np.cos(gamma), b**2, b*c*np.cos(alpha)],
-         [c*a*np.cos(beta), c*b*np.cos(alpha), c**2]]
+        [[a**2, a*b*cos(gamma), a*c*cos(beta)],
+         [b*a*cos(gamma), b**2, b*c*cos(alpha)],
+         [c*a*cos(beta), c*b*cos(alpha), c**2]]
     )
 
     g[abs(g) <= 1e-10] = 0
 
     return g
 
 
@@ -207,14 +209,15 @@
         Angle in degrees
 
     """
 
     p_q = np.array([vec1, vec2])
 
     [[pp, pq], [qp, qq]] = np.array(p_q @ g @ p_q.T)
+
     theta = np.degrees(np.arccos(pq/(pp**0.5 * qq**0.5)))
 
     return theta
 
 
 def rotation_angle_bt_vectors(vec1, vec2, trans_mat=None):
     """Calculate the rotation angle from one vector to a second vector. This
@@ -325,15 +328,15 @@
 
     a1_star = 1/IntPlSpc(g1, g)
     a2_star = 1/IntPlSpc(g2, g)
     alpha_star = np.radians(IntPlAng(g1, g2, g))
 
     a_star_2d = np.array([
         [a1_star, 0],
-        [a2_star*np.cos(alpha_star), a2_star*np.sin(alpha_star)]
+        [a2_star*cos(alpha_star), a2_star*sin(alpha_star)]
     ])
     a_star_2d[abs(a_star_2d) <= 1e-10] = 0
 
     return a_star_2d
 
 
 def TwoTheta(hkl, g, wavelength):
@@ -486,14 +489,15 @@
         path=None,
         display_image=True,
         images_from_stack='all',
         dsets_to_load=0,
         return_path=False,
         norm_image=True,
         full_metadata=False,
+        bin_dims=None,
 ):
     """Select image from 'Open File' dialog box, import and (optionally) plot
 
     Parameters
     ----------
     path : str or None
         The location of the image to load or the path to the folder containing
@@ -520,14 +524,19 @@
     full_metadata : bool
         For emd files ONLY, whether to load the entire metadata as nested
         dictionaries using JSON. If False, loads standard metadata using
         ncempy reader (including pixel size). If True, all metadata available
         in the file is loaded. It is a lot of metadata!
         Default: False
 
+    bin_dims : tuple or list or None
+        Binning factor for each dimension in the loaded dataset. If None, no
+        binning applied.
+        Default: None.
+
     Returns
     -------
     image : ndarray
         The imported image
 
     metadata : dict
         The metadata available in the original file
@@ -686,19 +695,14 @@
     elif path[-3:] == 'ser':
         ser_file = serReader(path)
         images = {0: ser_file['data']}
         metadata = {
             0: {key: val for key, val in ser_file.items() if key != 'data'}
         }
 
-        # images = {dsets_to_load: ser_file['data']}
-        # metadata = {dsets_to_load: {
-        #     key: val for key, val in ser_file.items() if key != 'data'
-        # }}
-
     else:
         images = {'image': imageio.volread(path)}
         # metadata = {'image': images['image'].meta}
         metadata = {'image': None}
 
     for key in images.keys():
         h, w = images[key].shape[-2:]
@@ -726,14 +730,29 @@
 
         if display_image is True:
             fig, axs = plt.subplots()
             axs.imshow(image_, cmap='gray')
             axs.set_xticks([])
             axs.set_yticks([])
 
+        if (type(bin_dims) in [tuple, list]):
+            if (len(bin_dims) != len(images[key].shape)):
+                raise Exception(
+                    'If binning, must specify binning factor for each ' +
+                    'dimension in the dataset and must be valid for all ' +
+                    'loaded datasets.')
+
+            dims = list(images[key].shape)
+            new_dims = np.array([
+                [dims[i]//bin_dims[i], bin_dims[i]] for i in range(len(dims))
+            ]).ravel()
+
+            images[key] = images[key].reshape(new_dims).mean(
+                axis=tuple([i for i in range(1, len(new_dims), 2)]))
+
     # If only one image, extract from dictionaries
     if len(images) == 1:
         key = list(images.keys())[0]
         images = images[key]
         metadata = metadata[key]
 
     if return_path:
@@ -906,124 +925,14 @@
 
     if return_binedges:
         return H, xedges, yedges
     else:
         return H
 
 
-# def linearKDE_2D_old(
-#         coords,
-#         xlim,
-#         ylim,
-#         d,
-#         w=1,
-#         weights=None,
-#         return_binedges=False
-# ):
-#     """
-#     Apply linear KDE to 2D coordinate set with optional weights.
-
-#     Parameters
-#     ----------
-#     coords : array of scalars (n, 2)
-#         the x, y coordinates of the data points.
-
-#     xlim : two-tuple of scalars
-#         The x limits of the resulting density estimate.
-
-#     ylim : two-tuple of scalars
-#         The y limits of the resulting density estimate.
-
-#     d : scalar
-#         The bin width.
-
-#     w : int
-#         The width of the kernal in integer number of bins.
-
-#     weights : array of scalars (n,) or None
-#         The values by which to weight each coordinates for the KDE. (e.g.
-#         the image intensity value of a pixel). If None, all data points are
-#         considered equal.
-
-#     return_binedges : bool
-#         Whether to return arrays with x & y coordinates of the bin edges.
-#         Default: False
-
-#     Returns
-#     -------
-#     H : array of scalars (h, w)
-#         The density estimate as a 2D histogram with shape defined by the
-#         specified xlim, ylim and d arguments.
-
-#     xedges, yedges : arrays of scalars with shapes (w+1,) and (h+1,)
-#         The bin edges of the pixels in H.
-
-#     """
-
-#     # Get bin spacing
-#     xedges = np.arange(xlim[0], xlim[1], d)
-#     yedges = np.arange(ylim[0], ylim[1], d)
-
-#     # Find edge closest to 0 and shift edges so (0,0) is exactly at the center
-#     # of a pixel
-#     x_min_ind = np.argmin(np.abs(xedges))
-#     y_min_ind = np.argmin(np.abs(yedges))
-#     xedges -= xedges[x_min_ind] + d/2
-#     yedges -= yedges[y_min_ind] + d/2
-
-#     # Get bin centers
-#     xcents = xedges[:-1] + d/2
-#     ycents = yedges[:-1] + d/2
-
-#     H = np.zeros((ycents.shape[0], xcents.shape[0]))
-
-#     xF = (coords[:, 0] // d) * d
-#     yF = (coords[:, 1] // d) * d
-
-#     # Get x and y position weights for the floor pixels
-#     xFw = 1 - coords[:, 0] % d
-#     yFw = 1 - coords[:, 1] % d
-
-#     # If intensity weights were not passed, get equal weighting array
-#     if weights is None:
-#         weights = np.ones(coords.shape[0])
-
-#     # Weighted histogram for x floor, y floor pixels
-#     H += np.histogram2d(
-#         yF, xF,
-#         bins=[yedges, xedges],
-#         weights=xFw * yFw * weights
-#     )[0]
-
-#     # Weighted histogram for x ceiling, y floor pixels
-#     H += np.histogram2d(
-#         yF, xF + d,
-#         bins=[yedges, xedges],
-#         weights=(1 - xFw) * yFw * weights
-#     )[0]
-
-#     # Weighted histogram for x floor, y ceiling pixels
-#     H += np.histogram2d(
-#         yF + d, xF,
-#         bins=[yedges, xedges],
-#         weights=xFw * (1 - yFw) * weights
-#     )[0]
-
-#     # Weighted histogram for x ceiling, y ceiling pixels
-#     H += np.histogram2d(
-#         yF + d, xF + d,
-#         bins=[yedges, xedges],
-#         weights=(1 - xFw) * (1 - yFw) * weights
-#     )[0]
-
-#     if return_binedges:
-#         return H, xedges, yedges
-#     else:
-#         return H
-
 def linearKDE_2D(
         coords,
         xlim,
         ylim,
         d,
         r=1,
         weights=None,
@@ -1042,14 +951,17 @@
 
     ylim : two-tuple of scalars
         The y limits of the resulting density estimate.
 
     d : positive scalar
         The bin width.
 
+    r : int
+        The bandwidth of the KDE.
+
     w : int
         The width of the kernal in integer number of bins.
 
     weights : array of scalars (n,) or None
         The values by which to weight each coordinates for the KDE. (e.g.
         the image intensity value of a pixel). If None, all data points are
         considered equal.
@@ -1066,16 +978,16 @@
 
     xedges, yedges : arrays of scalars with shapes (w+1,) and (h+1,)
         The bin edges of the pixels in H.
 
     """
 
     # Get bin spacing
-    xedges = np.arange(xlim[0], xlim[1], d)
-    yedges = np.arange(ylim[0], ylim[1], d)
+    xedges = np.arange(xlim[0], xlim[1], d).astype(float)
+    yedges = np.arange(ylim[0], ylim[1], d).astype(float)
 
     # Find edge closest to 0 and shift edges so (0,0) is exactly at the center
     # of a pixel
     x_min_ind = np.argmin(np.abs(xedges))
     y_min_ind = np.argmin(np.abs(yedges))
     xedges -= xedges[x_min_ind] + d/2
     yedges -= yedges[y_min_ind] + d/2
@@ -1185,16 +1097,16 @@
     -------
     tmat : array of shape (3, 3)
         The origin-shifted rotation matrix.
     """
     theta = np.radians(angle)
 
     tmat = np.array(
-        [[np.cos(theta), np.sin(theta), 0],
-         [-np.sin(theta), np.cos(theta), 0],
+        [[cos(theta), sin(theta), 0],
+         [-sin(theta), cos(theta), 0],
          [0, 0, 1]]
     )
     tau = np.array(
         [[1, 0, origin[0]],
          [0, 1, origin[1]],
          [0, 0, 1]]
     )
@@ -1248,28 +1160,27 @@
         bandwidth=0.5,
         reshape_method='original',
         fill_value=0
 ):
     """Rotate an image to arbitrary angle & interpolate using KDE.
 
     Apply an aribtrary image rotation and interpolate new pixel values using
-    the kernel density estimate (KDE) method with a Gaussian kernel. This
-    method is fairly slow and MAY NOT offer improved performance over bilinear
-    interpolation methods.
+    a linear kernel density estimate (KDE). Check result carefully. May
+    produce artifacts.
 
     Parameters
     ----------
     image : ndarray of shape (h,w)
         The image.
 
     angle : scalar
         The angle by which to rotate the image.
 
     bandwidth : scalar
-        The bandwidth of the Gaussian kernel in pixels.
+        The bandwidth of the linear kernel in pixels.
 
     reshape_method : str
         Final frame shape after rotation: 'fulldata', 'original', or
         'only_data'.
         'original' returns an image with the same shape as the input image,
         with corners that were rotated out of the image cut off.
         'fulldata' returns a image with shape >= original shape, but without
@@ -1327,51 +1238,91 @@
         # Expand resulting image frame
 
         h, w = int(np.floor(h - 2*minxy[1])), int(np.floor(w - 2*minxy[0]))
         coords = np.array(
             np.meshgrid(np.arange(0, w), np.arange(0, h))
         ).transpose(1, 2, 0).reshape((-1, 2))
 
-    elif reshape_method == 'original':
+        xlim = (np.min(coords_[:, 0]), np.max(coords_[:, 0]) + 1)
+        ylim = (np.min(coords_[:, 1]), np.max(coords_[:, 1]) + 1)
+
+    elif (reshape_method == 'original') or (reshape_method == 'only_data'):
         # Select coordinates remaining inside original image frame
         coords_ += minxy
         vertices += minxy
 
         inds = np.argwhere(
             ((coords_[:, 0] >= 0) &
-             (coords_[:, 0] < w - 1) &
+             (coords_[:, 0] <= w) &
              (coords_[:, 1] >= 0) &
-             (coords_[:, 1] < h - 1)
+             (coords_[:, 1] <= h)
              )
         )
 
+        xlim = (0, w + 1)
+        ylim = (0, h + 1)
+
         coords_ = np.squeeze(coords_[inds])
         weights = np.squeeze(weights[inds])
 
-    elif reshape_method == 'only_data':
-        raise Exception('Method not yet implimented')
+    # elif :
+    #     xlim = (0, w + 1)
+    #     ylim = (0, h + 1)
 
     else:
         raise Exception('reshape_method must be one of: "fulldata", '
                         '"original", or "only_data".')
 
     # Create rotated frame mask:
     mask = polygon2mask(
-        (np.int(np.ceil(np.max(coords[:, 1])) + 1),
-         np.int(np.ceil(np.max(coords[:, 0])) + 1)),
+        ((np.ceil(np.max(coords[:, 1])) + 1).astype(int),
+         (np.ceil(np.max(coords[:, 0])) + 1).astype(int)),
         np.fliplr(vertices))
 
-    # TODO: Use my KDE fumction instead
-    print('Need to update with my KDE function... This method does not currently work.')
+    image_rot = linearKDE_2D(
+        coords_,
+        xlim,
+        ylim,
+        d=1,
+        r=bandwidth,
+        weights=weights,
+        return_binedges=False,
+    )
+    image_rot *= mask
+
+    if reshape_method == 'only_data':
+        xlim, ylim, crop_sl = binary_find_largest_rectangle(mask)
+        image_rot = image_rot[ylim[0]:ylim[1], xlim[0]:xlim[1]]
+
+    return image_rot
+
+
+def get_circular_kernel(r):
+    """Get circular kernel
+
+    Parameters
+    ----------
+    r : int
+        Kernel radius.
 
-    # image_rot = np.reshape(image_rot, (h, w))
+    Returns
+    -------
+    kernel : 2D array
+        The circular kernel.
+    """
 
-    # image_rot = np.where(mask, image_rot, fill_value)
+    kern_rad = int(np.floor(r))
+    size = 2*kern_rad + 1
+    kernel = np.array(
+        [1 if np.hypot(i - kern_rad, j - kern_rad) <= r
+         else 0
+         for j in range(size) for i in range(size)]
+    ).reshape((size, size))
 
-    # return image_rot
+    return kernel
 
 
 def std_local(image, r):
     """Get local standard deviation of an image
     Parameters
     ----------
     image : ndarray of shape (h,w)
@@ -1386,22 +1337,15 @@
         The image local standard deviation of the image.
     """
 
     im = np.array(image, dtype=float)
     im2 = im**2
     ones = np.ones(im.shape)
 
-    # kernel = np.ones((2*r+1, 2*r+1))
-    kern_rad = int(np.floor(r))
-    size = 2*kern_rad + 1
-    kernel = np.array(
-        [1 if np.hypot(i - kern_rad, j - kern_rad) <= r
-         else 0
-         for j in range(size) for i in range(size)]
-    ).reshape((size, size))
+    kernel = get_circular_kernel(r)
 
     s = convolve2d(im, kernel, mode="same")
     s2 = convolve2d(im2, kernel, mode="same")
     ns = convolve2d(ones, kernel, mode="same")
     var = (s2/ns - (s/ns)**2)
     var = np.where(var < 0, 0, var)
 
@@ -1653,79 +1597,93 @@
                 peak_map_labeled,
                 np.arange(1, num_peaks+1)
             )
         ))).astype(int)
         peaks = pd.DataFrame.from_dict({
             'x': list(peak_xy[:, 0]),
             'y': list(peak_xy[:, 1]),
-            'max': image[peak_xy[:, 1], peak_xy[:, 0]],
+            'max': np.array(image[peak_xy[:, 1], peak_xy[:, 0]]).astype(float),
             'label': [i+1 for i in range(peak_xy.shape[0])]
         })
 
         return peak_map.astype(int), peaks
 
     else:
         return peak_map.astype(int)
 
 
 def watershed_segment(
         image,
         sigma=None,
         buffer=0,
-        local_thresh_factor=0.95,
-        peak_max_thresh_factor=0,
+        bkgd_thresh_factor=0.95,
+        peak_bkgd_thresh_factor=0,
         watershed_line=True,
-        min_dist=5
+        min_dist=5,
+        min_pixels=9,
 ):
     """Segment an image using the Watershed algorithm.
 
     Parameters
     ----------
     image : 2D array_like
         The image to be segmented.
 
-    sigma : int or float
+    sigma : scalar or None
         The Laplacian of Gaussian sigma value to use for peak sharpening. If
         None, no filtering is applied.
         Default: None
 
     buffer : int
         The border within which peaks are ignored.
         Default: 0
 
-    local_thresh_factor : float
+    bkgd_thresh_factor : float
         Removes background from each segmented region by thresholding.
         Threshold value determined by finding the maximum value of edge pixels
         in the segmented region and multipling this value by the
-        local_thresh_factor value. The filtered image is used for this
+        bkgd_thresh_factor value. The filtered image is used for this
         calculation.
         Default 0.95.
 
+    peak_bkgd_thresh_factor : float
+        Alternative local thresholding method that thresholds between the
+        watershed region edge maximum and the peak maximum. It is more
+        appropriate if center-of-mass measurements will be made on the
+        segmentation regions. Only active if bkgd_thresh_factor <= 0.
+        Default: 0.
+
     watershed_line : bool
-        Seperate segmented regions by one pixel.
+        Seperate segmented regions by a 1 pixel wide line of zero-value pixels.
         Default: True.
 
     min_dist : int or float
         The minimum distance allowed between detected peaks. Used to create
         a circular neighborhood kernel for peak detection.
-        Default: 4.
+        Default: 5.
+
+    min_pixels : int
+        The minimum number of pixels allowed in a mask region. If less than
+        this value, the mask and associated peak are discarded.
+        Default: 9.
 
     Returns
     -------
     masks : 2D array with same shape as image
 
     num_masks : int
         The number of masks
 
     slices : List of image slices which contain each region
 
     peaks : DataFrame with the coordinates and corresponding mask label for
         each peak not outside the buffer
 
     """
+
     img_der = copy.deepcopy(image)
     [h, w] = image.shape
 
     if type(sigma) in (int, float, tuple):
         img_der = image_norm(-gaussian_laplace(img_der, sigma))
 
     peak_map, peaks = detect_peaks(
@@ -1737,55 +1695,178 @@
     local_max, n_peaks = label(peak_map)
 
     masks = watershed(-img_der, local_max, watershed_line=watershed_line)
 
     slices = find_objects(masks)
     num_masks = int(np.max(masks))
 
-    """Refine masks with local_thresh_factor"""
-    if local_thresh_factor > 0:
+    # Refine masks with an optional threshold
+    if bkgd_thresh_factor > 0:
         masks_ref = np.zeros(image.shape)
 
         for i in range(0, num_masks):
             mask_sl = np.where(masks[slices[i][0], slices[i][1]] == i+1, 1, 0)
             img_der_sl = img_der[slices[i][0], slices[i][1]]
             edge = mask_sl - binary_erosion(mask_sl)
-            thresh = np.max(edge * img_der_sl) * (local_thresh_factor)
+            thresh = np.max(edge * img_der_sl) * (bkgd_thresh_factor)
             mask_sl = np.where(mask_sl*img_der_sl >= thresh, i+1, 0)
-            masks_ref[slices[i][0], slices[i][1]] += mask_sl
+            n_pixels = np.count_nonzero(mask_sl)
+            if n_pixels >= min_pixels:
+                masks_ref[slices[i][0], slices[i][1]] += mask_sl
 
         masks = masks_ref
 
-    elif peak_max_thresh_factor > 0:
+    elif peak_bkgd_thresh_factor > 0:
         masks_ref = np.zeros(image.shape)
 
         for i in range(0, num_masks):
             mask_sl = np.where(masks[slices[i][0], slices[i][1]] == i+1, 1, 0)
             img_der_sl = img_der[slices[i][0], slices[i][1]]
             edge = mask_sl - binary_erosion(mask_sl)
-            edge_max = np.max(edge * img_der_sl) * (local_thresh_factor)
+            edge_max = np.max(edge * img_der_sl)
             peak_max = np.max(img_der_sl)
-            thresh = peak_max_thresh_factor * (peak_max - edge_max) + edge_max
+            thresh = peak_bkgd_thresh_factor * (peak_max - edge_max) + edge_max
             mask_sl = np.where(mask_sl*img_der_sl >= thresh, i+1, 0)
-            masks_ref[slices[i][0], slices[i][1]] += mask_sl
+            n_pixels = np.count_nonzero(mask_sl)
+            if n_pixels >= min_pixels:
+                masks_ref[slices[i][0], slices[i][1]] += mask_sl
 
         masks = masks_ref
 
     peaks = peaks[
         ((peaks.x >= buffer) &
          (peaks.x <= w - buffer) &
          (peaks.y >= buffer) &
          (peaks.y <= h - buffer))
     ]
 
+    # Reduce all return elements to common remaining peaks/masks
+    unique_masks = np.unique(masks)
+
+    remaining = np.intersect1d(
+        unique_masks,
+        peaks.label.to_numpy()
+    ).astype(int)
+
+    masks = np.where(np.isin(masks, remaining), masks, 0)
+
+    peaks = peaks[np.isin(peaks.label.to_numpy(), remaining)]
     peaks = peaks.reset_index(drop=True)
 
+    slices = [slices[i] for i in range(len(slices)) if i in (remaining - 1)]
+
+    num_masks = remaining.shape[0]
+
     return masks, num_masks, slices, peaks
 
 
+def get_mask_polygon(
+        data,
+        vertices=None,
+        buffer=0,
+        invert=False,
+        show_mask=True,
+        return_vertices=False
+):
+    """Get a binary mask for an arbitrary shaped polygon.
+
+    Parameters
+    ----------
+    data : 2D array or 2-tuple
+        The data or data shape the mask will be applied to.
+
+    vertices : n x 2 array or None
+        The x, y coordinates of the polygon vertices. If None, will prompt to
+        graphically pick vertices with mouse clicks.
+        Default: None.
+
+    buffer : int
+        Edge border outside of which the mask will be cropped off regardless of
+        the vertices chosen.
+        Default: 0.
+
+    invert : bool
+        Whether to invert the mask so that pixel outside the specified polygon
+        are selected as the mask region (if True).
+        Default: False.
+
+    show_mask : bool
+        Whether to plot the resuting mask for verification.
+        Default: True.
+
+    return_vertices : bool
+        Whether to return the chosen vertices as an n x 2 array.
+        Default: False.
+
+    Returns
+    -------
+    mask : 2d array
+        The mask.
+
+    vertices : n x 2 array (optional)
+        The chosen vertices.
+
+    """
+
+    if type(data) == tuple:
+        data = np.zeros(data)
+
+    if vertices is not None:
+        vertices = np.fliplr(np.array(vertices))
+    if vertices is None:
+        fig, ax = plt.subplots(figsize=(8, 10))
+        ax.imshow(data, cmap='gist_gray')
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+        ax.set_title(
+            'Left click to add vertices.\n' +
+            'Right click or backspace key to remove last.\n' +
+            'Center click or enter key to complete.\n' +
+            'Must select in clockwise order.'
+        )
+
+        vertices = plt.ginput(
+            n=-1,
+            timeout=0,
+            show_clicks=True,
+            mouse_add=MouseButton.LEFT,
+            mouse_pop=MouseButton.RIGHT,
+            mouse_stop=MouseButton.MIDDLE
+        )
+
+        plt.close()
+        vertices = np.fliplr(np.array(vertices))
+
+    mask = polygon2mask(data.shape, vertices)
+
+    if buffer:
+        mask = erosion(
+            mask,
+            footprint=np.ones((3, 3))
+        )
+
+    if invert:
+        mask = np.where(mask == 1, 0, 1)
+
+    fig, ax = plt.subplots()
+    ax.imshow(data, cmap='gist_gray')
+
+    ax.imshow(
+        mask,
+        alpha=0.2,
+        cmap='Reds'
+    )
+
+    if return_vertices:
+        return mask, vertices
+    else:
+        return mask
+
+
 def img_equ_ellip(image):
     """Calculate the equivalent ellipse
 
     Parameters
     ----------
     image : ndarray
          Input image as an ndarray
@@ -1881,414 +1962,267 @@
         np.cross(np.array([1, 0]),
                  eigvects[major]).item()
     ))
 
     return x0, y0, eccen, theta, sig_maj, sig_min
 
 
-def gaussian_2d(x, y, x0, y0, sig_1, sig_2, ang, A=1, I_o=0):
-    """Sample a 2D, ellpitical Gaussian function.
-
-    Samples a specified 2D Gaussian function at an array of points.
+def gaussian_2d(x, y, x0, y0, sig_maj, sig_rat, ang, A=1, b=0):
+    """Sample a 2D, ellpitical Gaussian function or group of Gaussians.
 
     Parameters
     ----------
     x, y : ndarrays, must have the same shape
-        They x and y coordinates of each sampling point. If given arrays
+        The x and y coordinates of each sampling point. If given arrays
         generated by numpy.mgrid or numpy.meshgrid, will return an image
         of the Gaussian.
 
-    x0, y0 : center of the Gaussian
+    x0, y0 : scalars
+        Center coordinates of Gaussian(s).
 
-    sig_1 : sigma of the major axis
+    sig_maj : scalar(s)
+        Sigma of the major axix of the Gaussian(s).
 
-    sig_ratio : ratio of sigma major to sigma minor
+    sig_ratio : scalar(s)
+        Ratio of major to minor axis sigmas of the Gaussian(s).
 
-    ang : rotation angle of the major axis from horizontal
+    ang : scalar(s)
+        Rotation angle of the major axis from horizontal for the Gaussian(s).
+        In degrees.
 
-    A : Peak amplitude of the Gaussian
+    A : scalar(s)
+        Peak amplitude of the Gaussian(s).
 
-    I_o : Constant background value
+    b : scalar
+        Constant background value for the Gaussian(s).
 
     Returns
     -------
-    I : the value of the function at the specified points. Will have the same
+    z : the value of the function at the specified points. Will have the same
         shape as x, y inputs
 
     """
 
     ang = np.radians(-ang)  # negative due to inverted y axis in python
-    I = I_o + A*np.exp(-1/2*(
-        ((np.cos(ang) * (x - x0) + np.sin(ang) * (y - y0)) / sig_1)**2
-        + ((-np.sin(ang) * (x - x0) + np.cos(ang) * (y - y0)) / sig_2)**2))
+    sig_min = sig_maj / sig_rat
 
-    return I
+    z = np.sum(A * exp(-0.5 * (
+        ((cos(ang) * (x - x0) + sin(ang) * (y - y0)) / sig_maj)**2
+        + ((-sin(ang) * (x - x0) + cos(ang) * (y - y0)) / sig_min)**2)),
+        axis=0) + b
+
+    return z
 
 
-def gaussian_ellip_ss(p0, x, y, z, masks=None):
+def gaussian_ellip_ss(p0, x, y, z):
     """Sum of squares for a Gaussian function.
 
     Takes a parameter vector, coordinates, and corresponding data values;
     returns the sum of squares of the residuals.
 
     Parameters
     ----------
     p0 : array_like with shape (n,7)
         n = number of peaks to fit
         Array containing the Gaussian function parameter vector(s):
-            [x0, y0, sig_maj, sig_rat, ang, A, I_o]
+            [x0, y0, sig_maj, sig_rat, ang, A, b]
 
     x, y : 1D array_like, must have the same shape
         The flattened arrays of x and y coordinates of image pixels
 
     z : 1D array_like, must have the same shape as x and y
         The flattened array of image values at the x, y coordinates
 
-    masks : 2d array_like of size (n, m)
-        n = number of peaks to fit
-        m = number of unmasked pixels
-        The flattened masks for each peak. Each of the "n" rows is 1 where the
-        mask for the corresponding peak and 0 elsewhere.
-
     Returns
     -------
     r_sum_sqrd : float
         The sum of the squares of the residuals
 
     """
 
     if p0.shape[0] > 7:
-        I0 = p0[-1]
+        b = p0[-1]
         p0_ = p0[:-1].reshape((-1, 6))
         x0, y0, sig_maj, sig_rat, ang, A = np.split(p0_, 6, axis=1)
     else:
-        x0, y0, sig_maj, sig_rat, ang, A, I0 = p0
+        x0, y0, sig_maj, sig_rat, ang, A, b = p0
 
-    sig_min = sig_maj/sig_rat
+    ang *= -1
 
     # Sum the functions for each peak:
-    model = np.sum(A*np.exp(-1/2*(((np.cos(ang) * (x - x0)
-                                  + np.sin(ang) * (y - y0))
-                                   / sig_maj)**2
-                                  + ((-np.sin(ang) * (x - x0)
-                                      + np.cos(ang) * (y - y0))
-                                     / sig_min)**2)),
-                   axis=0) + I0
+    model = gaussian_2d(x, y, x0, y0, sig_maj, sig_rat, ang, A, b)
 
     # Subtract from data to get residuals:
     R = z - model
     r_sum_sqrd = (R @ R.T).flatten()
 
     return r_sum_sqrd
 
 
-def gaussian_circ_ss(p0, x, y, z, masks=None):
+def gaussian_circ_ss(p0, x, y, z):
     """Sum of squares for a Gaussian function.
 
     Takes a parameter vector, coordinates, and corresponding data values;
     returns the sum of squares of the residuals.
 
     Parameters
     ----------
     p0 : array_like with shape (n,7)
         n = number of peaks to fit
         Array containing the Gaussian function parameter vector(s):
-            [x0, y0, sig_maj, sig_rat, ang, A, I_o]
+            [x0, y0, sig_maj, sig_rat, ang, A, b]
 
     x, y : 1D array_like, must have the same shape
         The flattened arrays of x and y coordinates of image pixels
 
     z : 1D array_like, must have the same shape as x and y
         The flattened array of image values at the x, y coordinates
 
-    masks : 2d array_like of size (n, m)
-        n = number of peaks to fit
-        m = number of unmasked pixels
-        The flattened masks for each peak. Each of the "n" rows is 1 where the
-        mask for the corresponding peak and 0 elsewhere.
-
     Returns
     -------
     r_sum_sqrd : float
         The sum of the squares of the residuals
 
     """
 
     if p0.shape[0] > 5:
-        I0 = p0[-1]
+        b = p0[-1]
         p0_ = p0[:-1].reshape((-1, 4))
         x0, y0, sig, A = np.split(p0_, 4, axis=1)
     else:
-        x0, y0, sig, A, I0 = p0
+        x0, y0, sig, A, b = p0
 
     # Sum the functions for each peak:
-    model = np.sum(A*np.exp(-1/2*(
-        (((x - x0)) / sig)**2
-        + (((y - y0)) / sig)**2)),
-        axis=0) + I0
+    model = gaussian_2d(x, y, x0, y0, sig, 1, 0, A, b)
 
     # Subtract from data to get residuals:
     R = z - model
     r_sum_sqrd = (R @ R.T).flatten()
 
     return r_sum_sqrd
 
 
-def fit_gaussian_ellip(
+def fit_gaussians(
         data,
         p0,
-        masks=None,
         method='BFGS',
-        bounds=None
+        bounds=None,
+        circular=True,
 ):
     """Fit an elliptical 2D Gaussain function to data.
 
     Fits a 2D, elliptical Gaussian to an image. Intensity values equal to zero
     are ignored.
 
     Parameters
     ----------
     data : ndarray
         Image containing a Gaussian peak
 
     p0 : array_like with shape (n*6 + 1,)
         Initial guess for the n-Gaussian parameter vector where each peak
         has 6 independent parameters (x0, y0, sig_maj, sig_ratio, ang, A) the
-        whole region has a constant background (I_0) which is the last item in
+        whole region has a constant background (b) which is the last item in
         the array.
 
-    masks : 2d array_like of size (n, m)
-        n = number of peaks to fit
-        m = number of unmasked pixels
-        The flattened masks for each peak. Each of the "n" rows is 1 where the
-        mask for the corresponding peak and 0 elsewhere.
-
     method : str, the minimization solver name
         Supported solvers are: ''BFGS', 'L-BFGS-B', 'Powell', 'trust-constr'.
         Default: 'BFGS'
 
     bounds : list of two-tuples of length 7*n or None
         The bounds for Gaussian fitting parameters. Only works with methods
         that accept bounds (e.g. 'L-BFGS-B', but not 'BFGS'). Otherwise must
         be set to None.
         Each two-tuple is in the form: (upper, lower).
-        Order of bounds must be: [x0, y0, sig_maj, sig_ratio, ang, A, I_0] * n
+        Order of bounds must be: [x0, y0, sig_maj, sig_ratio, ang, A, b] * n
         Default: None
 
+    circular : bool
+        Whether to use a circular Gaussian for fitting. If False, uses an
+        elliptical Gaussian.
+        Default: True
+
     Returns
     -------
     params : 1D array
         The best fit parameter vector found by least squares
 
     """
 
     num_gauss = int(np.ceil(p0.shape[0]/7))
     img_shape = data.shape
 
-    I0 = p0[-1]
-    p0_ = p0[:-1].reshape((num_gauss, 6))
-
-    p0_[:, 4] *= -1
-
     y, x = np.indices(img_shape)
     z = data.flatten()
 
     unmasked_data = np.nonzero(z)
     z = np.take(z, unmasked_data)
     x = np.take(x.flatten(), unmasked_data)
     y = np.take(y.flatten(), unmasked_data)
 
-    x0y0 = p0_[:, :2]
-    if masks is None:
-        image = np.zeros(img_shape)
-        image[y, x] = z
-        masks_labeled, _ = label(image)
-
-    elif (type(masks) is imageio.core.util.Array
-          or type(masks) is np.ndarray):
-        masks_labeled, _ = label(masks)
-
-    masks_to_peaks = map_coordinates(
-        masks_labeled,
-        np.flipud(x0y0.T),
-        order=0
-    ).astype(int)
-
-    masks_labeled = np.take(masks_labeled, unmasked_data).flatten()
-
-    masks_labeled = np.array(
-        [np.where(masks_labeled == mask_num, 1, 0)
-         for i, mask_num in enumerate(masks_to_peaks)]
-    )
-
-    p0_ = np.append(p0_.flatten(), I0)
-
     with warnings.catch_warnings():
         warnings.filterwarnings(
             'ignore',
             category=UserWarning,
             lineno=182
         )
 
         warnings.filterwarnings(
             'ignore',
             category=RuntimeWarning,
             lineno=579
         )
 
-    params = minimize(
-        gaussian_ellip_ss,
-        p0_,
-        args=(x, y, z, masks_labeled),
-        bounds=bounds,
-        method=method
-    ).x
-
-    params = np.concatenate(
-        (params[:-1].reshape((-1, 6)),
-         np.ones((num_gauss, 1))*params[-1]),
-        axis=1
-    )
-
-    params[:, 4] *= -1
-    params[:, 4] = ((params[:, 4] + np.pi/2) % np.pi) - np.pi/2
-
-    return params
-
-
-def fit_gaussian_circ(
-        data,
-        p0,
-        masks=None,
-        method='BFGS',
-        bounds=None
-):
-    """Fit a circular 2D Gaussain function to data.
-
-    Fits a 2D, elliptical Gaussian to an image. Intensity values equal to zero
-    are ignored.
-
-    Parameters
-    ----------
-    data : ndarray
-        Image containing a Gaussian peak
-
-    p0 : array_like with shape (n, 5)
-        Initial guess for the n-Gaussian parameter vector where each peak
-        has 4 independent parameters (x0, y0, sig, A) the
-        whole region has a constant background (I_0).
-
-    masks : 2d array_like of size (n, m)
-        n = number of peaks to fit
-        m = number of unmasked pixels
-        The flattened masks for each peak. Each of the "n" rows is 1 where the
-        mask for the corresponding peak and 0 elsewhere.
-
-    method : str, the minimization solver name
-        Supported solvers are: 'BFGS', 'L-BFGS-B', 'Powell', 'trust-constr'.
-        Default: 'BFGS'
-
-    bounds : list of two-tuples of length 7*n or None
-        The bounds for Gaussian fitting parameters. Only works with methods
-        that accept bounds (e.g. 'L-BFGS-B', but not 'BFGS'). Otherwise must
-        be set to None.
-        Each two-tuple is in the form: (upper, lower).
-        Order of bounds must be: [x0, y0, sig, A, I_0] * n
-        Default: None
-
-    Returns
-    -------
-    params : 1D array
-        The best fit parameter vector found by least squares
-
-    """
-
-    num_gauss = p0.shape[0] // 4
-    img_shape = data.shape
-    I0 = p0[-1]
-    p0_ = p0[:-1].reshape((num_gauss, 4))
-
-    y, x = np.indices(img_shape)
-    z = data.flatten()
-
-    unmasked_data = np.nonzero(z)
-    z = np.take(z, unmasked_data)
-    x = np.take(x.flatten(), unmasked_data)
-    y = np.take(y.flatten(), unmasked_data)
+    if circular:
+        params = minimize(
+            gaussian_circ_ss,
+            p0,
+            args=(x, y, z),
+            bounds=bounds,
+            method=method
+        ).x
 
-    x0y0 = p0_[:, :2]
-    if masks is None:
-        image = np.zeros(img_shape)
-        image[y, x] = z
-        masks_labeled, _ = label(image)
-
-    elif (type(masks) is imageio.core.util.Array
-          or type(masks) is np.ndarray):
-        masks_labeled, _ = label(masks)
-
-    masks_to_peaks = map_coordinates(
-        masks_labeled,
-        np.flipud(x0y0.T),
-        order=0
-    ).astype(int)
+        n_params = 4
 
-    masks_labeled = np.take(
-        masks_labeled,
-        unmasked_data
-    ).flatten()
-
-    masks_labeled = np.array(
-        [np.where(masks_labeled == mask_num, 1, 0)
-         for i, mask_num in enumerate(masks_to_peaks)]
-    )
-
-    p0_ = np.append(p0_.flatten(), I0)
+    else:
+        params = minimize(
+            gaussian_ellip_ss,
+            p0,
+            args=(x, y, z),
+            bounds=bounds,
+            method=method
+        ).x
 
-    with warnings.catch_warnings():
-        warnings.filterwarnings('ignore', category=UserWarning,
-                                lineno=182)
-        warnings.filterwarnings('ignore', category=RuntimeWarning,
-                                lineno=579)
-
-    params = minimize(
-        gaussian_circ_ss,
-        p0_,
-        args=(x, y, z, masks_labeled),
-        bounds=bounds,
-        method=method
-    ).x
+        n_params = 6
 
     params = np.concatenate(
-        (params[:-1].reshape((-1, 4)),
+        (params[:-1].reshape((-1, n_params)),
          np.ones((num_gauss, 1))*params[-1]),
         axis=1
     )
+    if circular:
+        params = np.insert(params, [-1, -1], [1, 0], axis=1)
 
-    # Add dummy columns for sigma ratio and rotation angle:
-    params = np.insert(
-        params,
-        3,
-        np.array([1, 0]*num_gauss).reshape(-1, 2).T,
-        axis=1
-    )
+    else:
+        params[:, 4] *= -1
+        params[:, 4] = ((params[:, 4] + 90) % 180) - 90
 
     return params
 
 
 def pack_data_prefit(
         data,
         slices,
         masks,
         xy_peaks,
         peak_mask_index,
         peak_groups,
         pos_bound_dist=None,
         use_circ_gauss=False,
         use_bounds=False,
-        use_background_param=True,
 ):
     """Function to group data for the parallelized fitting process.
 
     Parameters
     ----------
     data : ndarray
         The data in which peaks are to be fit.
@@ -2337,15 +2271,14 @@
         [slices[counter][-1].start,
          slices[counter][-2].start
          ],
         xy_peaks[inds, :].reshape((-1, 2)),
         pos_bound_dist,
         use_circ_gauss,
         use_bounds,
-        use_background_param,
     ]
         for counter, inds
         in enumerate(peak_groups)
     ]
 
     return packed_data
 
@@ -2355,15 +2288,14 @@
         masks,
         mask_nums,
         xy_start,
         xy_peaks,
         pos_bound_dist=None,
         use_circ_gauss=False,
         use_bounds=False,
-        use_background_param=True,
 ):
     """Master function for simultaneously fitting one or more Gaussians to a
     piece of data.
 
     Parameters
     ----------
     data : 2d array
@@ -2405,20 +2337,14 @@
         Whether to apply bounds to minimization algorithm. This may be
         needed if unphysical results are obtained (e.g. negative
         background, negative amplitude, highly elliptical fits, etc.).
         The bounded version of the minimization runs slower than the
         unbounded.
         Default: False
 
-    use_background_param : bool
-        Whether to use the background parameter when fitting each atom
-        column or group of columns. If False, background value is forced
-        to be 0.
-        Default: True
-
     Returns
     -------
     params : array of shape (n,2)
         The fitted parameters for the Gaussian(s).
 
     """
 
@@ -2437,100 +2363,69 @@
             sig_2 = sig_replace
 
         if sig_1/sig_2 > 3:
             sig_1 = sig_2
             theta = 0
 
         sig_rat = sig_1/sig_2
-        I0 = (
+
+        b = (
             np.average(img_msk[img_msk != 0])
             - np.std(img_msk[img_msk != 0])
         )
-        A0 = np.max(img_msk) - I0
+        A0 = np.max(img_msk) - b
 
         if use_circ_gauss:
             if use_bounds:
                 bounds = [
                     (x0-pos_bound_dist/2, x0+pos_bound_dist),
                     (y0-pos_bound_dist/2, y0+pos_bound_dist),
-                    (1, None),
-                    (0, 1.2),
-                ] * num + [(0, None)]
-                method = 'L-BFGS-B'
+                    (1, 1.2),
+                    (0, None),
+                ] * num
 
-                if not use_background_param:
-                    bounds[-1] = (0, 0)
+                + [(0, None)]
+                method = 'L-BFGS-B'
 
             else:
                 bounds = None
                 method = 'BFGS'
 
             p0 = np.array(
-                [x0, y0, np.mean([sig_1, sig_2]),  A0, I0]
-            )
-
-            params = fit_gaussian_circ(
-                img_msk,
-                p0,
-                masks,
-                method=method,
-                bounds=bounds
+                [x0, y0, A0, np.mean([sig_1, sig_2]), b]
             )
 
         else:
             if use_bounds:
                 bounds = [
                     (x0 - pos_bound_dist/2, x0 + pos_bound_dist),
                     (y0 - pos_bound_dist/2, y0 + pos_bound_dist),
                     (1, None),
                     (1, None),
                     (None, None),
                     (0, 1.2),
                 ] * num + [(0, None)]
                 method = 'L-BFGS-B'
 
-                if not use_background_param:
-                    bounds[-1] = (0, 0)
-
             else:
                 bounds = None
                 method = 'BFGS'
 
-            p0 = np.array(
-                [x0, y0, sig_1, sig_rat,  np.radians(theta), A0, I0]
-            )
-
-            params = fit_gaussian_ellip(
-                img_msk,
-                p0,
-                masks,
-                method=method,
-                bounds=bounds
-            )
-
-        params = np.array(
-            [params[:, 0] + xy_start[0],
-             params[:, 1] + xy_start[1],
-             params[:, 2],
-             params[:, 2]/params[:, 3],
-             np.degrees(params[:, 4]),
-             params[:, 5],
-             params[:, 6]]
-        ).T
+            p0 = np.array([x0, y0, sig_1, sig_rat, theta, A0, b])
 
     if num > 1:
         x0y0 = xy_peaks - xy_start
         x0 = x0y0[:, 0]
         y0 = x0y0[:, 1]
 
         sig_1 = []
         sig_2 = []
         sig_rat = []
         theta = []
-        I0 = []
+        b = []
         A0 = []
 
         for i, mask_num in enumerate(mask_nums):
             mask = np.where(masks == mask_num, 1, 0)
             masked_sl = data * mask
             _, _, _, theta_, sig_1_, sig_2_ = (
                 img_ellip_param(masked_sl))
@@ -2544,18 +2439,18 @@
             if sig_1_/sig_2_ > 3:
                 sig_1_ = sig_2_
                 theta_ = 0
 
             sig_1 += [sig_1_]
             sig_2 += [sig_2_]
             sig_rat += [sig_1_ / sig_2_]
-            theta += [np.radians(theta_)]
-            I0 += [(np.average(masked_sl[masked_sl != 0])
-                    - np.std(masked_sl[masked_sl != 0]))]
-            A0 += [np.max(masked_sl) - I0[i]]
+            theta += [theta_]
+            b += [(np.average(masked_sl[masked_sl != 0])
+                   - np.std(masked_sl[masked_sl != 0]))]
+            A0 += [np.max(masked_sl) - b[i]]
 
         if use_circ_gauss:
             if use_bounds:
                 bounds = [
                     (None, None),
                     (None, None),
                     (1, None),
@@ -2567,34 +2462,23 @@
                     bounds[i*4] = (x0[i] - pos_bound_dist,
                                    x0[i] + pos_bound_dist)
                     bounds[i*4 + 1] = (y0[i] - pos_bound_dist,
                                        y0[i] + pos_bound_dist)
 
                 method = 'L-BFGS-B'
 
-                if not use_background_param:
-                    bounds[-1] = (0, 0)
-
             else:
                 bounds = None
                 method = 'BFGS'
 
             p0 = np.array(
                 [x0, y0, np.mean([sig_1, sig_2], axis=0), A0]
             ).T
 
-            p0 = np.append(p0.flatten(), np.mean(I0))
-
-            params = fit_gaussian_circ(
-                img_msk,
-                p0,
-                masks,
-                method=method,
-                bounds=bounds
-            )
+            p0 = np.append(p0.flatten(), np.mean(b))
 
         else:
             if use_bounds:
                 bounds = [
                     (None, None),
                     (None, None),
                     (1, None),
@@ -2609,128 +2493,139 @@
                     bounds[i*6] = (x0[i] - pos_bound_dist,
                                    x0[i] + pos_bound_dist)
                     bounds[i*6 + 1] = (y0[i] - pos_bound_dist,
                                        y0[i] + pos_bound_dist)
 
                 method = 'L-BFGS-B'
 
-                if not use_background_param:
-                    bounds[-1] = (0, 0)
-
             else:
                 bounds = None
                 method = 'BFGS'
 
             p0 = np.array(
                 [x0, y0, sig_1, sig_rat, theta, A0]
             ).T
 
-            p0 = np.append(p0.flatten(), np.mean(I0))
+            p0 = np.append(p0.flatten(), np.mean(b))
 
-            params = fit_gaussian_ellip(
-                img_msk,
-                p0,
-                masks,
-                method=method,
-                bounds=bounds
-            )
+    params = fit_gaussians(
+        img_msk,
+        p0,
+        method=method,
+        bounds=bounds,
+        circular=use_circ_gauss,
+    )
 
-        params = np.array(
-            [params[:, 0] + xy_start[0],
-             params[:, 1] + xy_start[1],
-             params[:, 2],
-             params[:, 2]/params[:, 3],
-             np.degrees(params[:, 4]),
-             params[:, 5],
-             params[:, 6]]
-        ).T
+    params = np.array(
+        [params[:, 0] + xy_start[0],
+         params[:, 1] + xy_start[1],
+         params[:, 2],
+         params[:, 2]/params[:, 3],
+         params[:, 4],
+         params[:, 5],
+         params[:, 6]]
+    ).T
 
     return params
 
 
-def plane_2d(x, y, mx, my, b):
-
-    z = mx*x + my*y + b
-
-    return z
-
-
-def plane_ss(p0, x, y, z):
-    """Sum of squares for a plane fit to 2D intensity data.
+def plane_2d(x, y, params):
+    """
+    Calculate z values for a plane at specified x and y positions.
 
     Parameters
     ----------
-    p0 : array_like with shape (n,7)
-        n = number of peaks to fit
-        Array containing the Gaussian function parameter vector(s):
-            [x0, y0, sig_maj, sig_rat, ang, A, I_o]
-
-    x, y : 1D array_like, must have the same shape
-        The flattened arrays of x and y coordinates of image pixels
+    x, y : ndarrays
+        The x and y coordinates at which to calculate the z height of the
+        plane. Must be the same shape.
 
-    z : 1D array_like, must have the same shape as x and y
-        The flattened array of image values at the x, y coordinates
-
-    masks : 2d array_like of size (n, m)
-        n = number of peaks to fit
-        m = number of unmasked pixels
-        The flattened masks for each peak. Each of the "n" rows is 1 where the
-        mask for the corresponding peak and 0 elsewhere.
+    params : 3-typle of scalars
+        The x and y slopes and z-intercept of the plane.
 
     Returns
     -------
-    r_sum_sqrd : float
-        The sum of the squares of the residuals
+    z : ndarray
+        The z values of the plane at the x, y coordinates. Will be the same
+        shape as x & y.
 
     """
 
+    [mx, my, b] = params
+
+    z = mx*x + my*y + b
+
+    return z
+
+
+def sum_squares(p0, args, fn):
+
     # Sum the functions for each peak:
-    model = plane_2d(x, y, *p0)
+    z = args[-1]
+    model = fn(*args[:-1], p0)
 
     # Subtract from data to get residuals:
     R = z - model
     r_sum_sqrd = (R @ R.T).flatten()
 
     return r_sum_sqrd
 
 
 def plane_fit(
         data,
         p0,
 ):
+    """Fit a plane to 3D coordinate data or 2D intensity data.
+
+    Parameters
+    ----------
+    data: 2D array
+        The intensity values or z-coordinates in a regularly sampled array.
+
+    p0 : 3-list
+        Initial guess for the plane fitting parameters: the x & y
+        slopes and the z intercept.
+
+    Returns
+    -------
+    params : array
+        The fitted parameters.
+
+    """
 
     y, x = np.indices(data.shape)
     z = data.flatten()
 
     unmasked_data = np.nonzero(z)
     z = np.take(z, unmasked_data)
     x = np.take(x.flatten(), unmasked_data)
     y = np.take(y.flatten(), unmasked_data)
 
+    args = [x, y, z]
+
     params = minimize(
-        plane_ss,
+        sum_squares,
         p0,
-        args=(x, y, z),
-        bounds=[(None, None), (None, None), (0, None)],
-        method='L-BFGS-B'
+        args=(args, plane_2d),
+        method='L-BFGS-B',
     ).x
 
     return params
 
 
 # %%
 """Fourier Analysis"""
 
 
-def fft_square(image,
-               hann_window=False,
-               upsample_factor=None,
-               abs_val=True,
-               pre_shift=False,
-               ):
+def fft_square(
+    image,
+    hann_window=False,
+    upsample_factor=None,
+    abs_val=True,
+    pre_shift=False,
+):
     """Gets FFT with equal x & y pixel sizes
 
     Parameters
     ----------
     image : ndarray
         The image or image stack. May be an image stack or 4D array of images
         (e.g. a 4D dataset of diffraction patterns, 4D STEM). The FFT will
@@ -2816,15 +2711,15 @@
     inds = np.arange(dim)
 
     origin = np.array([dim/2] * 2, ndmin=3).T
 
     r = norm(np.array(np.meshgrid(inds, inds)) - origin, axis=0
              ) * 2*np.pi / dim
 
-    hann = np.where(r > np.pi, 0, np.cos(r) + 1) / 2
+    hann = np.where(r > np.pi, 0, cos(r) + 1) / 2
 
     return hann
 
 
 def get_fft_pixel_size(image, pixel_size):
     """Gets FFT pixel size for a real-space image.
 
@@ -2876,16 +2771,16 @@
     h, w = im.shape
     j = np.arange(h)[:, None]
     k = np.arange(w)[None, :]
 
     x += w/2  # because the coordinates are zero-centered
     y += h/2
 
-    val = np.sum((im * (np.exp(-2 * np.pi * 1j * j * y / h) @
-                        np.exp(-2 * np.pi * 1j * k * x / w))))
+    val = np.sum((im * (exp(-2 * np.pi * 1j * j * y / h) @
+                        exp(-2 * np.pi * 1j * k * x / w))))
 
     return val
 
 
 def get_ewpc(data, upsample_factor=1, window=None):
     """
     Calculate the exit wave power cepstrum of a dataset.
@@ -3014,16 +2909,16 @@
 
     h, w = image.shape[-2:]
 
     x0, y0 = np.array([w, h]) // 2 - np.array(x0y0)
 
     shift = [0 for _ in range(len(image.shape)-2)] + [y0, x0]
 
-    im_cent = np.abs(np.fft.ifft2(
-        fourier_shift(np.fft.fft2(image, axes=(-2, -1)), shift),
+    im_cent = np.abs(ifft2(
+        fourier_shift(fft2(image, axes=(-2, -1)), shift),
         axes=(-2, -1)))
 
     return im_cent
 
 
 def dp_center_obj_fn(xy, dp):
     """
@@ -3444,15 +3339,15 @@
         pcf_sm = copy.deepcopy(vpcf)
         sigma = 2
 
     masks_indiv, n_peaks, _, peaks = watershed_segment(
         pcf_sm,
         min_dist=sigma,
         # max_thresh_factor=0.5,
-        # local_thresh_factor=0,
+        # bkgd_thresh_factor=0,
         sigma=None,
         buffer=buffer,
         watershed_line=False,
     )
 
     peaks['peak_max'] = vpcf[
         peaks.loc[:, 'y'].to_numpy(dtype=int),
@@ -3477,15 +3372,15 @@
             sigma=sigma_group,
             truncate=3
         )
 
         group_masks, _, _, _ = watershed_segment(
             pcf_sm,
             min_dist=sigma_group,
-            local_thresh_factor=0,
+            bkgd_thresh_factor=0,
             sigma=None,
             buffer=0,
             watershed_line=True
         )
 
         group_masks_to_peaks = map_coordinates(
             group_masks,
@@ -3568,20 +3463,20 @@
                            (0, None),
                            (0, None),
                            ]
 
             p0 = np.array(p0 + [0])
             bounds += [(0, 0)]
 
-            params = fit_gaussian_ellip(
+            params = fit_gaussians(
                 pcf_masked,
                 p0,
-                masks=None,
                 method='L-BFGS-B',
-                bounds=bounds
+                bounds=bounds,
+                shape='ellip'
             )
 
             # params = params[:, :-1]
             params[:, 3] = params[:, 2] / params[:, 3]
             params[:, 4] = np.degrees(params[:, 4])
             params[:, -1] = np.sqrt(1 - params[:, 3]**2
                                     / params[:, 2]**2)
@@ -3890,15 +3785,15 @@
         label='2'
     )
 
     if return_fig:
         return fig, ax
 
 
-def disp_vect_sum_squares(p0, xy, M):
+def disp_vect_sum_squares(p0, xy, M, weights=None):
     """Objective function for 'fit_lattice()'.
 
     Parameters
     ----------
     p0 : list-like of shape (6,)
         The current basis guess of the form: [a1x, a1y, a2x, a2y, x0, y0].
         Where [a1x, a1y] is the first basis vector, [a2x, a2y] is the second
@@ -3918,22 +3813,24 @@
     sum_sq : scalar
         The sum of squared errors given p0.
 
     """
 
     dir_struct_matrix = p0[:-2].reshape((-1, 2))
     origin = p0[-2:]
+    if weights is None:
+        weights = 1
 
-    err_xy = xy - M @ dir_struct_matrix - origin
-    sum_sq = np.sum(err_xy**2)
+    err_xy = norm(xy - (M @ dir_struct_matrix + origin), axis=1)
+    sum_sq = np.sum((err_xy * weights)**2)
 
     return sum_sq
 
 
-def fit_lattice(p0, xy, M, fix_origin=False):
+def fit_lattice(p0, xy, M, fix_origin=False, weights=None):
     """Find the best fit of a rigid lattice to a set of points.
 
     Parameters
     ----------
     p0 : list-like of shape (6,)
         The initial basis guess of the form: [a1x, a1y, a2x, a2y, x0, y0].
         Where [a1x, a1y] is the first basis vector, [a2x, a2y] is the second
@@ -3960,22 +3857,26 @@
         The refined basis, using the same form as p0.
 
     """
 
     p0 = np.array(p0).flatten()
     x0y0 = p0[-2:]
 
+    # dists = norm(xy - x0y0, axis=1)
+
+    # weights = 0 * dists / np.max(dists) + 1
+
     if fix_origin is True:
         params = (lstsq(M, xy - x0y0, rcond=-1)[0]).flatten()
     else:
         params = minimize(
             disp_vect_sum_squares,
             p0,
-            args=(xy, M),
-            method='L-BFGS-B',
+            args=(xy, M, weights),
+            method='BFGS',
         ).x
 
     return params
 
 
 def fft_amplitude_area(
         image,
@@ -4027,27 +3928,27 @@
     """
 
     if not (type(r) is int) | (type(r) is float):
         if xy_fft.shape[0] != r.shape[0]:
             raise Exception("If'r' is not an int or float, its length "
                             "must match the first dimension of xy_fft.")
 
-    fft = np.fft.fftshift(np.fft.fft2(image))
+    fft = fftshift(fft2(image))
     mask = np.zeros(fft.shape)
     xy = np.mgrid[:mask.shape[0], : mask.shape[1]]
     xy = np.array([xy[1], xy[0]]).transpose((1, 2, 0))
     if (type(r) is int) | (type(r) is float):
         for xy_ in xy_fft:
             mask += np.where(norm(xy - xy_, axis=2) <= r, 1, 0)
 
     else:
         for i, xy_ in enumerate(xy_fft):
             mask += np.where(norm(xy - xy_, axis=2) <= r[i], 1, 0)
 
-    amplitude = np.abs(np.fft.ifft2(np.fft.fftshift(fft * mask)))
+    amplitude = np.abs(ifft2(fftshift(fft * mask)))
     amplitude = image_norm(gaussian_filter(amplitude, sigma=blur))
     mask = np.where(amplitude > thresh, 1, 0)
     if fill_holes:
         mask = binary_fill_holes(mask)
     mask = np.where(mask, 1, 0)
     mask = binary_dilation(mask, iterations=buffer)
 
@@ -4059,14 +3960,17 @@
         cmap='inferno',
         figsize=(6, 6),
         hide_ticks=True,
         pixel_size=None,
         pixel_unit=None,
         scalebar_len=None,
         return_figax=False,
+        scaling='linear',
+        vmin=None,
+        vmax=None,
 ):
     """Convienience image plotting function.
 
     Parameters
     ----------
     im : 2D array
         The image.
@@ -4098,23 +4002,36 @@
         function.
         Default: None
 
     return_fig : bool
         Whether to return the figure and axes objects for modification by user.
         Default: False
 
+    scaling : float or str
+        Linear ('linear'), log ('log') or power law (float on interval [0, 1])
+        scaling of the image intensity.
+        Default: 'linear'
+
     Returns
     -------
-    mask : 2D array
-        The final amplitude mask.
+    fig, ax : matplotlib figure and axes objects
+        The resulting figure and axes objects for possible further
+        modifications.
 
     """
 
+    if scaling == 'log':
+        norm = LogNorm()
+    elif type(scaling) in [float, int]:
+        norm = PowerNorm(scaling)
+    else:
+        norm = None
+
     fig, ax = plt.subplots(1, figsize=figsize)
-    ax.imshow(im, cmap=cmap)
+    ax.imshow(im, cmap=cmap, norm=norm, vmin=vmin, vmax=vmax)
 
     if hide_ticks:
         ax.set_xticks([])
         ax.set_yticks([])
 
     if pixel_size is not None:
         if pixel_unit is None:
```

### Comparing `SingleOrigin-2.5.6/src/SingleOrigin.egg-info/PKG-INFO` & `singleorigin-2.5.7/src/SingleOrigin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleOrigin
-Version: 2.5.6
+Version: 2.5.7
 Summary: Crystallographic analysis for STEM data
 Author-email: Stephen Funni <sdf68@cornell.edu>
 Project-URL: homepage, https://github.com/sdfunni/SingleOrigin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

