# Comparing `tmp/meg_qc-0.1.6.tar.gz` & `tmp/meg_qc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.1.6.tar", last modified: Thu Apr 11 13:20:14 2024, max compression
+gzip compressed data, was "meg_qc-0.1.7.tar", last modified: Tue Apr 30 09:32:26 2024, max compression
```

## Comparing `meg_qc-0.1.6.tar` & `meg_qc-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.926919 meg_qc-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-11 13:20:06.000000 meg_qc-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-11 13:20:14.926919 meg_qc-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-11 13:20:06.000000 meg_qc-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.926919 meg_qc-0.1.6/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 13:20:14.926919 meg_qc-0.1.6/meg_qc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.922918 meg_qc-0.1.6/meg_qc/calculation/
--rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/initial_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20690 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/meg_qc_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.926919 meg_qc-0.1.6/meg_qc/calculation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)   116229 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/Head_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    52964 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/PSD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25659 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/STD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/calculation/metrics/muscle_meg_qc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.926919 meg_qc-0.1.6/meg_qc/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/plotting/meg_qc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/plotting/universal_html_report.py
--rw-r--r--   0 runner    (1001) docker     (127)   125049 2024-04-11 13:20:06.000000 meg_qc-0.1.6/meg_qc/plotting/universal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:14.922918 meg_qc-0.1.6/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-11 13:20:14.000000 meg_qc-0.1.6/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-11 13:20:14.000000 meg_qc-0.1.6/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:20:14.000000 meg_qc-0.1.6/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 13:20:14.000000 meg_qc-0.1.6/meg_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 13:20:14.000000 meg_qc-0.1.6/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 13:20:06.000000 meg_qc-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 13:20:14.926919 meg_qc-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-11 13:20:06.000000 meg_qc-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-11 13:20:06.000000 meg_qc-0.1.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 09:32:16.000000 meg_qc-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-30 09:32:26.585735 meg_qc-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-30 09:32:16.000000 meg_qc-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.581735 meg_qc-0.1.7/meg_qc/calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/initial_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/meg_qc_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/calculation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)   112596 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Head_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/PSD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25659 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/STD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/muscle_meg_qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/meg_qc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/universal_html_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130403 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/universal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.581735 meg_qc-0.1.7/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:32:16.000000 meg_qc-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 09:32:26.585735 meg_qc-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 09:32:16.000000 meg_qc-0.1.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-30 09:32:16.000000 meg_qc-0.1.7/versioneer.py
```

### Comparing `meg_qc-0.1.6/LICENSE` & `meg_qc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/PKG-INFO` & `meg_qc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg_qc
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.6/README.md` & `meg_qc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/__main__.py` & `meg_qc-0.1.7/meg_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/initial_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/initial_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/meg_qc_pipeline.py` & `meg_qc-0.1.7/meg_qc/calculation/meg_qc_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,14 +267,16 @@
                 'Peak-to-Peak manual': pp_manual_derivs, 
                 'Peak-to-Peak auto from MNE': pp_auto_derivs, 
                 'ECG': ecg_derivs, 
                 'EOG': eog_derivs,
                 'Head movement artifacts': head_derivs,
                 'High frequency (Muscle) artifacts': muscle_derivs}
 
+                print('___MEGqc___: ', 'QC_derivs', QC_derivs)  
+
 
                 QC_simple={
                 'STD': simple_metrics_std, 
                 'PSD': simple_metrics_psd,
                 'PTP_MANUAL': simple_metrics_pp_manual, 
                 'PTP_AUTO': simple_metrics_pp_auto,
                 'ECG': simple_metrics_ecg,
```

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,19 @@
     allowed_range_of_peaks_stds : float, optional
         Allowed range of standard deviations of peak amplitudes, by default 0.05. Works for ECG channel, but not good for EOG channel.
     height_multiplier: float
         Will define how high the peaks on the ECG channel should be to be counted as peaks. Higher value - higher the peak need to be, hense less peaks will be found.
     
     Returns
     -------
-    similar_ampl : bool
-        True if peaks have similar amplitude
-    no_breaks : bool
-        True if there are up to allowed number of breaks in the data
-    no_bursts : bool
-        True if there are up to allowed number of bursts in the data
+    ecg_eval : dict
+        Dictionary with 3 booleans, indicating if the channel is good or bad according to 3 conditions:
+        - similar_ampl: True if peaks have similar amplitudes, False otherwise
+        - no_breaks: True if there are no breaks longer than normal max distance between peaks of hear beats, False otherwise
+        - no_bursts: True if there are no bursts: too short intervals between peaks, False otherwise
     fig : plotly.graph_objects.Figure
         Plot of the channel data and detected peaks
 
     """
 
     # 1. Check if R peaks (or EOG peaks)  have similar amplitude. If not - data is too noisy:
     # Find R peaks (or peaks of EOG wave) using find_peaks
@@ -94,64 +93,17 @@
     if n_breaks > len(rr_intervals)/60*10/n_breaks_bursts_allowed_per_10min:
         print("___MEGqc___: There are more than 2 breaks in the data, number: ", n_breaks)
         no_breaks = False
     if n_bursts > len(rr_intervals)/60*10/n_breaks_bursts_allowed_per_10min:
         print("___MEGqc___: There are more than 2 bursts in the data, number: ", n_bursts)
         no_bursts = False
 
+    ecg_eval = {'similar_ampl': similar_ampl, 'no_breaks': no_breaks, 'no_bursts': no_bursts}
+    return ecg_eval, peaks
 
-    return (similar_ampl, no_breaks, no_bursts), peaks
-
-
-
-def plot_ECG_EOG_channel(ch_data: np.ndarray or list, peaks: np.ndarray or list, ch_name: str, fs: float, verbose_plots: bool):
-
-    """
-    Plot the ECG channel data and detected peaks
-    
-    Parameters
-    ----------
-    ch_data : list or np.ndarray
-        Data of the channel
-    peaks : list or np.ndarray
-        Indices of the peaks in the data
-    ch_name : str
-        Name of the channel
-    fs : int
-        Sampling frequency of the data
-    verbose_plots : bool
-        If True, show the figure in the notebook
-        
-    Returns
-    -------
-    fig : plotly.graph_objects.Figure
-        Plot of the channel data and detected peaks
-        
-    """
-
-    time = np.arange(len(ch_data))/fs
-    fig = go.Figure()
-    fig.add_trace(go.Scatter(x=time, y=ch_data, mode='lines', name=ch_name + ' data'))
-    fig.add_trace(go.Scatter(x=time[peaks], y=ch_data[peaks], mode='markers', name='peaks'))
-    fig.update_layout(xaxis_title='time, s', 
-                yaxis = dict(
-                showexponent = 'all',
-                exponentformat = 'e'),
-                yaxis_title='Amplitude',
-                title={
-                'text': ch_name,
-                'y':0.85,
-                'x':0.5,
-                'xanchor': 'center',
-                'yanchor': 'top'})
-    
-    if verbose_plots is True:
-        fig.show()
-
-    return fig
 
 def detect_noisy_ecg(raw: mne.io.Raw, ecg_ch: str,  ecg_or_eog: str, n_breaks_bursts_allowed_per_10min: int, allowed_range_of_peaks_stds: float, height_multiplier: float):
     
     """
     Detects noisy ecg or eog channels.
 
     The channel is noisy when:
@@ -185,40 +137,43 @@
     Returns
     -------
     bad_ecg_eog : dict
         Dictionary with channel names as keys and 'good' or 'bad' as values.
     all_ch_data[0] : list
         data of the ECG channel recorded.
     ecg_eval : tuple
-        Tuple of 3 booleans, indicating if the channel is good or bad according to 3 conditions.
-
+        Tuple of 3 booleans, indicating if the channel is good or bad according to 3 conditions:
+        - similar_ampl: True if peaks have similar amplitudes, False otherwise
+        - no_breaks: True if there are no breaks longer than normal max distance between peaks of hear beats, False otherwise
+        - no_bursts: True if there are no bursts: too short intervals between peaks, False otherwise
 
-        
     """
 
     sfreq=raw.info['sfreq']
 
     bad_ecg_eog = {}
     peaks = []
 
     ch_data = raw.get_data(picks=ecg_ch)[0] #here ch_data will be the RAW DATA
     # get_data creates list inside of a list becausee expects to create a list for each channel. 
     # but iteration takes 1 ch at a time. this is why [0]
 
     ecg_eval, peaks = check_3_conditions(ch_data, sfreq, ecg_or_eog, n_breaks_bursts_allowed_per_10min, allowed_range_of_peaks_stds, height_multiplier)
     print(f'___MEGqc___: {ecg_ch} satisfied conditions for a good channel: ', ecg_eval)
 
-    if all(ecg_eval):
-        print(f'___MEGqc___: Overall good {ecg_or_eog} channel: {ecg_ch}')
+    #If all values in disct are true:
+    if all(value == True for value in ecg_eval.values()):
         bad_ecg_eog[ecg_ch] = 'good'
     else:
-        print(f'___MEGqc___: Overall bad {ecg_or_eog} channel: {ecg_ch}')
         bad_ecg_eog[ecg_ch] = 'bad'
 
-    return bad_ecg_eog, ch_data, peaks, ecg_eval
+    ecg_eval_str = 'Overall ' + bad_ecg_eog[ecg_ch] + ' ' + ecg_or_eog + ' channel: ' + ecg_ch + ': \n - Peaks have similar amplitude: ' + str(ecg_eval["similar_ampl"]) + ' \n - No breaks (too long distances between peaks): ' + str(ecg_eval["no_breaks"]) + ' \n - No bursts (too short distances between peaks): ' + str(ecg_eval["no_bursts"]) + '\n'
+    print(f'___MEGqc___: ', ecg_eval_str)
+
+    return bad_ecg_eog, ch_data, peaks, ecg_eval_str
 
 
 def find_epoch_peaks(ch_data: np.ndarray, thresh_lvl_peakfinder: float):
     
     """
     Find the peaks in the epoch data using the peakfinder algorithm.
 
@@ -309,24 +264,21 @@
         p-value of the correlation coefficient between the ECG/EOG channels data and average data of this mag/grad channel
     lobe: str
         which lobe his channel belongs to
     color: str
         color code for this channel according to the lobe it belongs to
     
 
-
-        
     Methods
     -------
     __init__(self, name: str, artif_data:list, peak_loc=None, peak_magnitude=None, wave_shape:bool=None, artif_over_threshold:bool=None, main_peak_loc: int=None, main_peak_magnitude: float=None)
         Constructor
     __repr__(self)
         Returns a string representation of the object
 
-        
     """
 
     def __init__(self, name: str, artif_data:list, peak_loc=None, peak_magnitude=None, wave_shape:bool=None, artif_over_threshold:bool=None, main_peak_loc: int=None, main_peak_magnitude: float=None, artif_data_smoothed: list or None = None, peak_loc_smoothed=None, peak_magnitude_smoothed=None, wave_shape_smoothed:bool=None, artif_over_threshold_smoothed:bool=None, main_peak_loc_smoothed: int=None, main_peak_magnitude_smoothed: float=None, corr_coef: float = None, p_value: float = None, lobe: str = None, color: str = None):
         """Constructor"""
         
         self.name =  name
         self.artif_data = artif_data
@@ -904,111 +856,14 @@
 
     if verbose_plots is True:
         fig.show()
 
     return fig
 
 
-def plot_affected_channels_csv(artif_affected_channels: list, artifact_lvl: float, t: np.ndarray, ch_type: str, fig_tit: str, chs_by_lobe: dict, flip_data: bool or str = 'flip', smoothed: bool = False, verbose_plots: bool = True):
-
-    """
-    Plot the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
-    
-    Parameters
-    ----------
-    artif_affected_channels : list
-        List of ECG/EOG artifact affected channels.
-    artifact_lvl : float
-        The threshold for the artifact amplitude: average over all channels*norm_lvl.
-    t : np.ndarray
-        Time vector.
-    ch_type : str
-        Either 'mag' or 'grad'.
-    fig_tit: str
-        The title of the figure.
-    chs_by_lobe : dict
-        dictionary with channel objects sorted by lobe
-    flip_data : bool
-        If True, the absolute value of the data will be used for the calculation of the mean artifact amplitude. Default to 'flip'. 
-        'flip' means that the data will be flipped if the peak of the artifact is negative. 
-        This is donr to get the same sign of the artifact for all channels, then to get the mean artifact amplitude over all channels and the threshold for the artifact amplitude onbase of this mean
-        And also for the reasons of visualization: the artifact amplitude is always positive.
-    smoothed: bool
-        Plot smoothed data (true) or nonrmal (false)
-    verbose_plots : bool
-        True for showing plot in notebook.
-
-    Returns
-    -------
-    fig : plotly.graph_objects.Figure
-        The plotly figure with the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
-
-        
-    """
-
-    if artif_affected_channels: #if affected channels present:
-
-        #plot channels separated by lobes:
-        affected_names_list = []
-        affected_data_list = []
-        for ch in artif_affected_channels:
-            affected_names_list.append(ch.name)
-            if smoothed is True:
-                affected_data_list.append(ch.artif_data_smoothed)
-            else:
-                affected_data_list.append(ch.artif_data)
-
-        affected_data_arr = np.array(affected_data_list)
-
-        df_affected=pd.DataFrame(affected_data_arr.T, columns=affected_names_list)
-
-        #fig = plot_df_of_channels_data_as_lines_by_lobe(chs_by_lobe, df_affected, t)
-        fig = plot_df_of_channels_data_as_lines_by_lobe_csv(f_path, 'ecg', t, m_or_g)
-
-        #decorate the plot:
-        ch_type_tit, unit = get_tit_and_unit(ch_type)
-        fig.update_layout(
-            xaxis_title='Time in seconds',
-            yaxis = dict(
-                showexponent = 'all',
-                exponentformat = 'e'),
-            yaxis_title='Mean artifact magnitude in '+unit,
-            title={
-                'text': fig_tit+str(len(artif_affected_channels))+' '+ch_type_tit,
-                'y':0.85,
-                'x':0.5,
-                'xanchor': 'center',
-                'yanchor': 'top'})
-
-
-    else:
-        fig=go.Figure()
-        ch_type_tit, _ = get_tit_and_unit(ch_type)
-        title=fig_tit+'0 ' +ch_type_tit
-        fig.update_layout(
-            title={
-            'text': title,
-            'x': 0.5,
-            'y': 0.9,
-            'xanchor': 'center',
-            'yanchor': 'top'})
-        
-    #in any case - add the threshold on the plot
-    fig.add_trace(go.Scatter(x=t, y=[(artifact_lvl)]*len(t), line=dict(color='red'), name='Thres=mean_peak/norm_lvl')) #add threshold level
-
-    if flip_data is False and artifact_lvl is not None: 
-        fig.add_trace(go.Scatter(x=t, y=[(-artifact_lvl)]*len(t), line=dict(color='black'), name='-Thres=mean_peak/norm_lvl'))
-
-    if verbose_plots is True:
-        fig.show()
-
-    return fig
-
-
-
 def flip_channels(artif_per_ch_nonflipped: list, tmin: float, tmax: float, sfreq: int, params_internal: dict):
 
     """
     Flip the channels if the peak of the artifact is negative and located close to the estimated t0.
 
     Flip approach: 
 
@@ -1862,15 +1717,15 @@
     # for example tmin is  set to -0.05 to 0.02, but it  can only plot between -0.0496 and 0.02.
 
     mne_ecg_derivs += [QC_derivative(fig_ecg_sensors, 'ECG_field_pattern_sensors_'+m_or_g, 'matplotlib')]
 
     return mne_ecg_derivs
 
 
-def get_ECG_data_choose_method(raw: mne.io.Raw, ecg_params: dict, verbose_plots: bool):
+def get_ECG_data_choose_method(raw: mne.io.Raw, ecg_params: dict):
 
     """
     Choose the method of finding affected channels based on the presense and quality of ECG channel.
 
     Options:
     - Channel present and good: correlation with ECG channel
     - Channel present and bad or missing:correlation with reconstructed channel
@@ -1908,37 +1763,47 @@
     if len(ecg_ch)>=1: #ecg channel present
 
         if len(ecg_ch)>1: #more than 1 ecg channel present
             ecg_str = 'More than 1 ECG channel found. The first one is used to identify hearbeats. '
 
         ecg_ch = ecg_ch[0]
 
-        bad_ecg_eog, ecg_data, event_indexes, ecg_eval = detect_noisy_ecg(raw, ecg_ch,  ecg_or_eog = 'ECG', n_breaks_bursts_allowed_per_10min = ecg_params['n_breaks_bursts_allowed_per_10min'], allowed_range_of_peaks_stds = ecg_params['allowed_range_of_peaks_stds'], height_multiplier = ecg_params['height_multiplier'])
+        bad_ecg_eog, ecg_data, event_indexes, ecg_eval_str = detect_noisy_ecg(raw, ecg_ch,  ecg_or_eog = 'ECG', n_breaks_bursts_allowed_per_10min = ecg_params['n_breaks_bursts_allowed_per_10min'], allowed_range_of_peaks_stds = ecg_params['allowed_range_of_peaks_stds'], height_multiplier = ecg_params['height_multiplier'])
 
-        fig = plot_ECG_EOG_channel(ecg_data, event_indexes, ch_name = ecg_ch, fs = raw.info['sfreq'], verbose_plots = verbose_plots)
-        noisy_ch_derivs = [QC_derivative(fig, bad_ecg_eog[ecg_ch]+' '+ecg_ch, 'plotly', description_for_user = ecg_ch+' is '+ bad_ecg_eog[ecg_ch]+ ': 1) peaks have similar amplitude: '+str(ecg_eval[0])+', 2) tolerable number of breaks: '+str(ecg_eval[1])+', 3) tolerable number of bursts: '+str(ecg_eval[2]))]
+        #Collect the data into 1 df for plotting later. ecg_ch as name of first column, ecg_data as data, event_indexes as indexes of the events:
+        event_indexes_with_none = event_indexes.tolist() + [None] * (len(ecg_data) - len(event_indexes))
+        fs_with_none = [raw.info['sfreq']] + [None] * (len(ecg_data) - 1)
+
+        ecg_ch_df = pd.DataFrame({
+            ecg_ch: ecg_data,
+            'event_indexes': event_indexes_with_none,
+            'fs': fs_with_none})
 
         if bad_ecg_eog[ecg_ch] == 'bad': #ecg channel present but noisy:
-            ecg_str = 'ECG channel data is too noisy, cardio artifacts were reconstructed. ECG channel was dropped from the analysis. Consider checking the quality of ECG channel on your recording device. '
+            ecg_str = 'ECG channel data is too noisy, cardio artifacts were reconstructed. ECG channel was dropped from the analysis. Consider checking the quality of ECG channel on your recording device. \n'
             print('___MEGqc___: ', ecg_str)
             raw.drop_channels(ecg_ch)
             use_method = 'correlation_reconstructed'
 
         elif bad_ecg_eog[ecg_ch] == 'good': #ecg channel present and good - use it
-            ecg_str = ecg_ch + ' is good and is used to identify hearbeats. '
+            ecg_str = ecg_ch + ' is used to identify hearbeats. \n'
             use_method = 'correlation'
 
     else: #no ecg channel present
 
-        noisy_ch_derivs, ecg_data, event_indexes = [], [], []
-        ecg_str = 'No ECG channel found. The signal is reconstructed based on magnetometers data. '
+        ecg_ch_df, ecg_data, event_indexes = [], [], []
+        ecg_str = 'No ECG channel found. The signal is reconstructed based on magnetometers data. \n'
         use_method = 'correlation_reconstructed'
         print('___MEGqc___: ', ecg_str)
 
-    return use_method, ecg_str, noisy_ch_derivs, ecg_data, event_indexes
+    ecg_str_total = ecg_eval_str + ecg_str 
+    #Replace all \n with <br> for the html report:
+    ecg_str_total = ecg_str_total.replace('\n', '<br>')
+
+    return use_method, ecg_str_total, ecg_ch_df, ecg_data, event_indexes
 
 def get_EOG_data(raw: mne.io.Raw):
 
     """
     Find if the EOG channel is present anfd get its data.
     
     Parameters
@@ -2070,31 +1935,31 @@
     else:
         ecg_str_checked = 'Mean events of '+ecg_or_eog+' channel does not have expected shape. Artifact detection was not performed.'
         print('___MEGqc___: ', ecg_str_checked)
 
 
     #Plot:
     if mean_rwave.size > 0:
-        t = np.linspace(tmin, tmax, len(mean_rwave))
+        mean_rwave_time = np.linspace(tmin, tmax, len(mean_rwave))
         if use_method == 'correlation_reconstructed':
             title = 'Mean data of the RECONSTRUCTED '
         elif use_method == 'correlation':
             title = 'Mean data of the RECORDED '
         else:
             title = 'Mean data of '
 
-        mean_rwave_fig = mean_rwave_obj.plot_epoch_and_peak(t, title, ecg_or_eog, fig = None, plot_original = True, plot_smoothed = False)
+        mean_rwave_fig = mean_rwave_obj.plot_epoch_and_peak(mean_rwave_time, title, ecg_or_eog, fig = None, plot_original = True, plot_smoothed = False)
         if verbose_plots is True:
             mean_rwave_fig.show()
 
         fig_derivs = [QC_derivative(mean_rwave_fig, 'Mean_artifact'+ecg_or_eog, 'plotly', description_for_user = ecg_str_checked)]
     else:
         fig_derivs = []
 
-    return mean_rwave_obj.wave_shape, ecg_str_checked, mean_rwave, fig_derivs
+    return mean_rwave_obj.wave_shape, ecg_str_checked, mean_rwave, mean_rwave_time, fig_derivs
 
 
 # Functions for alignment of ECG with meg channels:
 
 def find_t0_mean(ch_data: np.ndarray or list):
 
     """
@@ -2430,22 +2295,26 @@
     #tmin, tmax can be anything from -0.1/0.1 to -0.04/0.04. for CORRELATION method. But if we do mean and threshold - time best has to be -0.04/0.04. 
     # For this method number of peaks in particular time frame is calculated and based on that good/bad rwave is decided.
     norm_lvl=ecg_params['norm_lvl']
     gaussian_sigma=ecg_params['gaussian_sigma']
     thresh_lvl_peakfinder=ecg_params['thresh_lvl_peakfinder']
 
     ecg_derivs = []
-    use_method, ecg_str, noisy_ch_derivs, ecg_data, event_indexes = get_ECG_data_choose_method(raw, ecg_params, verbose_plots)
+    use_method, ecg_str, ecg_ch_df, ecg_data, event_indexes = get_ECG_data_choose_method(raw, ecg_params)
     
-    #ecg_derivs += noisy_ch_derivs
-
 
-    mean_good, ecg_str_checked, mean_rwave, rwave_derivs = check_mean_wave(raw, use_method, ecg_data, 'ECG', event_indexes, tmin, tmax, sfreq, ecg_params_internal, thresh_lvl_peakfinder, verbose_plots)
+    mean_good, ecg_str_checked, mean_rwave, mean_rwave_time, rwave_derivs = check_mean_wave(raw, use_method, ecg_data, 'ECG', event_indexes, tmin, tmax, sfreq, ecg_params_internal, thresh_lvl_peakfinder, verbose_plots)
+    
     ecg_str += ecg_str_checked
 
+    ecg_ch_df['mean_rwave'] = mean_rwave.tolist() + [None] * (len(ecg_data) - len(mean_rwave))
+    ecg_ch_df['mean_rwave_time'] = mean_rwave_time.tolist() + [None] * (len(ecg_data) - len(mean_rwave_time))
+    print('___MEGqc___: mean_rwave_time:', ecg_ch_df['mean_rwave_time'])
+    ecg_ch_df['recorded_or_reconstructed'] = [use_method] + [None] * (len(ecg_data) - 1)
+    ecg_derivs += [QC_derivative(content=ecg_ch_df, name='ECGchannel', content_type = 'df')]
     ecg_derivs += rwave_derivs
 
     if mean_good is False:
         simple_metric_ECG = {'description': ecg_str}
         return ecg_derivs, simple_metric_ECG, ecg_str, []
 
     
@@ -2516,14 +2385,15 @@
     #TODO: above we always use tmin, tmax, sfreq to create time vector in every fuction. here it s done again, maybe change above?
 
     for m_or_g  in m_or_g_chosen:
         for lobe, lobe_channels in chs_by_lobe[m_or_g].items():
             for lobe_ch in lobe_channels:
                 lobe_ch.add_ecg_info(affected_channels[m_or_g], artif_time_vector)
 
+
     ecg_csv_deriv = chs_dict_to_csv(chs_by_lobe,  file_name_prefix = 'ECGs')
 
     ecg_derivs += ecg_csv_deriv
 
     return ecg_derivs, simple_metric_ECG, ecg_str, avg_objects_ecg
 
 
@@ -2598,15 +2468,15 @@
     event_indexes = event_indexes[0]
     print('___MEG_QC___: Blinks will be detected based on channel: ', eog_ch_name)
 
     
     use_method = 'correlation' #'mean_threshold' 
     #no need to choose method in EOG because we cant reconstruct channel, always correlaion (if channel present) or fail.
 
-    mean_good, eog_str_checked, mean_blink, blink_derivs = check_mean_wave(raw, use_method, eog_data, 'EOG', event_indexes, tmin, tmax, sfreq, eog_params_internal, thresh_lvl_peakfinder, verbose_plots)
+    mean_good, eog_str_checked, mean_blink, mean_rwave_time, blink_derivs = check_mean_wave(raw, use_method, eog_data, 'EOG', event_indexes, tmin, tmax, sfreq, eog_params_internal, thresh_lvl_peakfinder, verbose_plots)
     eog_str += eog_str_checked
 
     eog_derivs += blink_derivs
 
     if mean_good is False:
         simple_metric_EOG = {'description': eog_str}
         return eog_derivs, simple_metric_EOG, eog_str, []
```

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/Head_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/Head_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/PSD_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/PSD_meg_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import mne
 import plotly.graph_objects as go
 from scipy.integrate import simpson
 from scipy.signal import find_peaks, peak_widths
 from IPython.display import display
 from typing import List
 import copy
+import re
 
 from meg_qc.plotting.universal_plots import QC_derivative, get_tit_and_unit, plot_df_of_channels_data_as_lines_by_lobe
 from meg_qc.calculation.initial_meg_qc import chs_dict_to_csv
 from meg_qc.plotting.universal_html_report import simple_metric_basic
 
 # ISSUE IN /Volumes/M2_DATA/MEG_QC_stuff/data/from openneuro/ds004107/sub-mind004/ses-01/meg/sub-mind004_ses-01_task-auditory_meg.fif...
 # COULDNT SPLIT  when filtered data - check with new psd version
@@ -147,15 +148,15 @@
     fig_name='PSD_all_data_'+tit
 
     qc_derivative = QC_derivative(content=fig, name=fig_name, content_type='plotly')
 
     return qc_derivative
 
 
-def get_mean_bands_amplitude(freq_bands: list, freqs: list, psds: np.ndarray or list, channels: list):
+def get_mean_bands_amplitude(freq_bands: list, freqs: list, psds: np.ndarray or list, channels: list, bands_names: list = None):
 
     """
     Calculate the area under the curve of frequency bands (e.g. alpha, beta, gamma, delta, ...) for mag or grad.
     Adopted from: https://raphaelvallat.com/bandpower.html
     Take mean over all channels (mags/grads).
 
     
@@ -167,14 +168,17 @@
         List of frequencies.
     psds : np.ndarray or list
         numpy array (or list) of power spectrum dencities. Expects array of arrays: channels*psds. (or list of lists)
         Will not work properly if 1 dimentional array given. In this case do: np.array([your_1d_array])
     channels : list
         List of channel names. Expects list of strings: ['MEG 0111', 'MEG 0112', ...] 
         If only one channel is given, it should be a list of one string: ['Average]
+    bands_names : list, optional
+        List of names of the bands. If None, the names will be generated automatically, by default None
+        Important! taht these names are in the same order as in freq_bands. 
 
         
     Returns
     -------
     band_ampl_df : pd.DataFrame
         Dataframe of amplitudes of each frequency band like: [abs_power_of_delta, abs_power_of_gamma, etc...] - in absolute values
     band_ampl_relative_to_signal_df : pd.DataFrame
@@ -185,18 +189,36 @@
         (This is done to compare with RMSE later. But not used any more).
     total_signal_amplitude : list
         List of total signal amplitude for each channel.
 
 
     """
 
+    #Check that freq_bands correspond to band names corectly:
+    if bands_names is None:
+        bands_as_str=[str(band[0])+'-'+str(band[1])+'Hz' for band in freq_bands]
+    else:
+        bands_as_str = bands_names #assume everything is correct. then check:
+        # Iterate over wave_bands and bands_names
+        for band, name in zip(freq_bands, bands_names):
+            # Extract the frequency range from the name
+            freq_range = re.search(r'\((.*?) Hz\)', name).group(1).split('-')
+
+            freq_range = [float(freq) for freq in freq_range]
+
+            # If the frequency range doesn't match the band, correct bands_as_str
+            if freq_range != band:
+                bands_as_str = [str(band[0])+'-'+str(band[1])+'Hz' for band in freq_bands]
+                break
+
+
     freq_res = freqs[1] - freqs[0]
-    
+
     total_signal_amplitude = []
-    bands_as_str=[str(band[0])+'-'+str(band[1])+'Hz' for band in freq_bands]
+
     band_ampl_df = pd.DataFrame(index=channels, columns=bands_as_str)
     band_ampl_relative_to_signal_df = pd.DataFrame(index=channels, columns=bands_as_str)
     ampl_by_Nfreq_per_ch_list_df = pd.DataFrame(index=channels, columns=bands_as_str)
 
     for ch_n, _ in enumerate(psds):
         total_signal_amplitude.append(simpson(psds[ch_n], dx=freq_res)) #amplitudeof all bands 
 
@@ -260,45 +282,39 @@
 
     """
     
     # Calculate the band amplitude:
     wave_bands=[[0.5, 4], [4, 8], [8, 12], [12, 30], [30, 100]]
     bands_names = ["delta (0.5-4 Hz)", "theta (4-8 Hz)", "alpha (8-12 Hz)", "beta (12-30 Hz)", "gamma (30-100 Hz)"]
 
-    abs_band_ampl_df, band_ampl_relative_to_signal_df, ampl_by_Nfreq_per_ch_list_df, _ = get_mean_bands_amplitude(wave_bands, freqs, psds, channels)
-
-    # Rename columns and extract to csv:
-    abs_band_ampl_df.columns = bands_names
-    ampl_by_Nfreq_per_ch_list_df.columns = bands_names
-    band_ampl_relative_to_signal_df.columns = bands_names
-
+    abs_band_ampl_df, relative_band_ampl_df, ampl_by_Nfreq_per_ch_list_df, _ = get_mean_bands_amplitude(wave_bands, freqs, psds, channels, bands_names)
 
     dfs_with_name = [
         QC_derivative(abs_band_ampl_df,'abs_ampl_'+m_or_g, 'df'),
-        QC_derivative(band_ampl_relative_to_signal_df, 'relative_ampl_'+m_or_g, 'df'),
+        QC_derivative(relative_band_ampl_df, 'relative_ampl_'+m_or_g, 'df'),
         QC_derivative(ampl_by_Nfreq_per_ch_list_df, 'ampl_by_Nfreq_'+m_or_g, 'df')]
 
     # Calculate the mean amplitude of each band over all channels:
-    abs_band_ampl_df, relative_band_ampl_df, _, total_ampl = get_mean_bands_amplitude(wave_bands, freqs, [avg_psd], ['Average PSD'])
+    abs_mean_band_ampl_df, relative_mean_band_ampl_df, _, total_ampl = get_mean_bands_amplitude(wave_bands, freqs, [avg_psd], ['Average PSD'], bands_names)
     
     # Merge the dataframes and with 'absolute' and 'relative' raw names:
-    brain_bands_df = pd.concat([abs_band_ampl_df, relative_band_ampl_df], axis=0)  
+    brain_bands_df = pd.concat([abs_mean_band_ampl_df, relative_mean_band_ampl_df], axis=0)  
     brain_bands_df.index = ['absolute_'+m_or_g, 'relative_'+m_or_g]
 
     #add total_ampl as a new column in 'Absolute' raw and None in 'Relative' raw:
     brain_bands_df['total_amplitude'] = None
     brain_bands_df['total_amplitude']['absolute_'+m_or_g] = total_ampl[0]
     brain_bands_df['total_amplitude']['relative_'+m_or_g] = 1
 
     waves_pie_df_deriv = [QC_derivative(content=brain_bands_df, name='PSDwaves'+m_or_g.capitalize(), content_type = 'df')]
     
     #convert results to a list:
 
-    mean_brain_waves_abs=abs_band_ampl_df.iloc[0, :].values.tolist()
-    mean_brain_waves_relative=relative_band_ampl_df.iloc[0, :].values.tolist()
+    mean_brain_waves_abs=abs_mean_band_ampl_df.iloc[0, :].values.tolist()
+    mean_brain_waves_relative=relative_mean_band_ampl_df.iloc[0, :].values.tolist()
 
     mean_brain_waves_dict= {bands_names[i]: {'mean_brain_waves_relative': np.round(mean_brain_waves_relative[i]*100, 2), 'mean_brain_waves_abs': mean_brain_waves_abs[i]} for i in range(len(bands_names))}
 
     return waves_pie_df_deriv, dfs_with_name, mean_brain_waves_dict
 
 
 def split_blended_freqs_at_the_lowest_point(noisy_bands_indexes:List[list], one_psd:List[dict], noisy_freqs_indexes:List[dict]):
```

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/STD_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/STD_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/calculation/metrics/muscle_meg_qc.py` & `meg_qc-0.1.7/meg_qc/calculation/metrics/muscle_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/plotting/meg_qc_plots.py` & `meg_qc-0.1.7/meg_qc/plotting/meg_qc_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # Add the parent directory to sys.path
 sys.path.append(parent_dir)
 sys.path.append(gradparent_dir)
 
 # from meg_qc.source.universal_plots import QC_derivative, boxplot_all_time_csv, boxplot_epoched_xaxis_channels_csv, boxplot_epoched_xaxis_epochs_csv, Plot_psd_csv, plot_artif_per_ch_correlated_lobes_csv, plot_correlation_csv, plot_muscle_csv, make_head_pos_plot_csv
 # from meg_qc.source.universal_html_report import make_joined_report, make_joined_report_mne
 
-from meg_qc.plotting.universal_plots import QC_derivative, boxplot_all_time_csv, boxplot_epoched_xaxis_channels_csv, boxplot_epoched_xaxis_epochs_csv, Plot_psd_csv, plot_artif_per_ch_correlated_lobes_csv, plot_correlation_csv, plot_muscle_csv, make_head_pos_plot_csv, plot_sensors_3d_csv, plot_pie_chart_freq_csv
+# from meg_qc.plotting.universal_plots import QC_derivative, boxplot_all_time_csv, boxplot_epoched_xaxis_channels_csv, boxplot_epoched_xaxis_epochs_csv, Plot_psd_csv, plot_artif_per_ch_correlated_lobes_csv, plot_correlation_csv, plot_muscle_csv, make_head_pos_plot_csv, plot_sensors_3d_csv, plot_pie_chart_freq_csv, plot_ECG_EOG_channel
+from meg_qc.plotting.universal_plots import *
 from meg_qc.plotting.universal_html_report import make_joined_report, make_joined_report_mne
 
 
 # # Needed to import the modules without specifying the full path, for command line and jupyter notebook
 # sys.path.append('./')
 # sys.path.append('./meg_qc/source/')
 
@@ -225,15 +226,16 @@
     m_or_g_chosen = plot_settings['m_or_g'] 
     verbose_plots = bool(plot_settings['verbose_plots'][0]=='True')
 
     raw = [] # TODO: if empty - we cant print raw information. 
     # Or we need to save info from it somewhere separately and export as csv/jspn and then read back in.
 
     time_series_derivs, sensors_derivs, ptp_manual_derivs, pp_auto_derivs, ecg_derivs, eog_derivs, std_derivs, psd_derivs, muscle_derivs, head_derivs = [], [], [], [], [], [], [], [], [], []
-
+    #TODO: think about it! the order goes by tsv files so it s messed uo cos ecg channels comes seond!
+    
     for tsv_path in tsv_paths: #if we got several tsvs for same metric, like for PSD:
 
         if 'STD' in metric.upper():
 
             fig_std_epoch0 = []
             fig_std_epoch1 = []
 
@@ -268,17 +270,14 @@
                 #fig_std_epoch1 += [boxplot_epochs(df_mg=df_std, ch_type=m_or_g, what_data='stds', x_axis_boxes='channels', verbose_plots=verbose_plots)] #old version
                 #fig_std_epoch2 += [boxplot_epochs(df_mg=df_std, ch_type=m_or_g, what_data='stds', x_axis_boxes='epochs', verbose_plots=verbose_plots)]
 
                 ptp_manual_derivs += [fig_all_time] + [fig_ptp_epoch0] + [fig_ptp_epoch1] 
 
         elif 'PSD' in metric.upper():
 
-            print('___We plot PSDs!')
-            print(tsv_path)
-
             method = 'welch' #is also hard coded in PSD_meg_qc() for now
 
             psd_derivs += plot_sensors_3d_csv(tsv_path)
 
             for m_or_g in m_or_g_chosen:
 
                 psd_derivs += Plot_psd_csv(m_or_g, tsv_path, method, verbose_plots)
@@ -287,30 +286,32 @@
 
                 psd_derivs += plot_pie_chart_freq_csv(tsv_path, m_or_g=m_or_g, noise_or_waves = 'waves', verbose_plots=verbose_plots)
 
         elif 'ECG' in metric.upper():
 
             ecg_derivs += plot_sensors_3d_csv(tsv_path)
 
-            for m_or_g in m_or_g_chosen:
-                affected_derivs = plot_artif_per_ch_correlated_lobes_csv(tsv_path, m_or_g, 'ECG', flip_data=False, verbose_plots=verbose_plots)
-                correlation_derivs = plot_correlation_csv(tsv_path, 'ECG', m_or_g, verbose_plots=verbose_plots)
+            ecg_derivs += plot_ECG_EOG_channel_csv(tsv_path, verbose_plots)
+
+            ecg_derivs += plot_mean_ecg_ch_data_csv(tsv_path, 'ECG', verbose_plots)
 
-                ecg_derivs += affected_derivs + correlation_derivs
+            #TODO: add ch description like here? export it as separate report strings?
+            #noisy_ch_derivs += [QC_derivative(fig, bad_ecg_eog[ecg_ch]+' '+ecg_ch, 'plotly', description_for_user = ecg_ch+' is '+ bad_ecg_eog[ecg_ch]+ ': 1) peaks have similar amplitude: '+str(ecg_eval[0])+', 2) tolerable number of breaks: '+str(ecg_eval[1])+', 3) tolerable number of bursts: '+str(ecg_eval[2]))]
 
+            for m_or_g in m_or_g_chosen:
+                ecg_derivs += plot_artif_per_ch_correlated_lobes_csv(tsv_path, m_or_g, 'ECG', flip_data=False, verbose_plots=verbose_plots)
+                ecg_derivs += plot_correlation_csv(tsv_path, 'ECG', m_or_g, verbose_plots=verbose_plots)
 
         elif 'EOG' in metric.upper():
 
             eog_derivs += plot_sensors_3d_csv(tsv_path)
                 
             for m_or_g in m_or_g_chosen:
-                affected_derivs = plot_artif_per_ch_correlated_lobes_csv(tsv_path, m_or_g, 'EOG', flip_data=False, verbose_plots=verbose_plots)
-                correlation_derivs = plot_correlation_csv(tsv_path, 'EOG', m_or_g, verbose_plots=verbose_plots)
-
-                eog_derivs += affected_derivs + correlation_derivs 
+                eog_derivs += plot_artif_per_ch_correlated_lobes_csv(tsv_path, m_or_g, 'EOG', flip_data=False, verbose_plots=verbose_plots)
+                eog_derivs += plot_correlation_csv(tsv_path, 'EOG', m_or_g, verbose_plots=verbose_plots)
 
             
         elif 'MUSCLE' in metric.upper():
 
             if 'mag' in m_or_g_chosen:
                 m_or_g_decided=['mag']
             elif 'grad' in m_or_g_chosen and 'mag' not in m_or_g_chosen:
@@ -338,14 +339,20 @@
     'PtP_auto': pp_auto_derivs, 
     'ECG': ecg_derivs, 
     'EOG': eog_derivs,
     'Head': head_derivs,
     'Muscle': muscle_derivs,
     'Report_MNE': []}
 
+    #Sort all based on fig_order of QC_derivative:
+    #(To plot them in correct order in the report)
+    for metric, values in QC_derivs.items():
+        if values:
+            QC_derivs[metric] = sorted(values, key=lambda x: x.fig_order)
+
 
     if not report_str_path: #if no report strings were saved. happens when mags/grads didnt run to make tsvs.
         report_strings = {
         'INITIAL_INFO': '',
         'TIME_SERIES': '',
         'STD': '',
         'PSD': '',
@@ -413,32 +420,35 @@
 
                 if metric == 'PSDs':
                     tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseMag', scope='derivatives')))
                     tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseGrad', scope='derivatives')))
                     tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesMag', scope='derivatives')))
                     tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesGrad', scope='derivatives')))
                 
+                if metric == 'ECGs':
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'ECGchannel', scope='derivatives')))
+
+                if metric == 'EOGs':
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'EOGchannel', scope='derivatives')))
+
                 tsvs_to_plot[metric] = tsv_path
 
             print('___MEGqc___: TSVs to plot: ', tsvs_to_plot)
 
             counter = 0
             for metric, tsv_paths in tsvs_to_plot.items():
                 #for n_tsv, tsv_path in enumerate(files):
 
-                print('__THIS TSVs: ', tsv_paths)
-
                 meg_artifact = subject_folder.create_artifact(raw=list_of_sub_jsons[counter]) #shell. empty derivative
                 meg_artifact.add_entity('desc', metric) #file name
                 meg_artifact.suffix = 'meg'
                 meg_artifact.extension = '.html'
 
                 # Here convert csv into figure and into html report:
                 deriv = csv_to_html_report(metric, tsv_paths, report_str_path, plot_settings)
-                print('___MEGqc___: ', '___HERE DERIV', deriv)
 
                 meg_artifact.content = lambda file_path, cont=deriv['Report_MNE'][0].content: cont.save(file_path, overwrite=True, open_browser=False)
                 counter += 1
 
     ancpbids.write_derivative(dataset, derivative) 
 
     return tsvs_to_plot
```

### Comparing `meg_qc-0.1.6/meg_qc/plotting/universal_html_report.py` & `meg_qc-0.1.7/meg_qc/plotting/universal_html_report.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/meg_qc/plotting/universal_plots.py` & `meg_qc-0.1.7/meg_qc/plotting/universal_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,15 +464,15 @@
     description_for_user : str, optional
         The description of the derivative, by default 'Add measurement description for a user...'
         Used in the report to describe the derivative.
     
 
     """
 
-    def __init__(self, content, name, content_type, description_for_user = ''):
+    def __init__(self, content, name, content_type, description_for_user = '', fig_order = 0):
 
         """
         Constructor method
         
         Parameters
         ----------
         content : figure, pd.DataFrame or str
@@ -481,21 +481,25 @@
             The name of the derivative (used to save in to file system)
         content_type : str
             The type of the content: 'plotly', 'matplotlib', 'df', 'report' or 'mne_report'.
             Used to choose the right way to save the derivative in main function.
         description_for_user : str, optional
             The description of the derivative, by default 'Add measurement description for a user...'
             Used in the report to describe the derivative.
+        fig_order : int, optional
+            The order of the figure in the report, by default 0. Used for sorting.
+        
 
         """
 
         self.content =  content
         self.name = name
         self.content_type = content_type
         self.description_for_user = description_for_user
+        self.fig_order = fig_order
 
     def __repr__(self):
 
         """
         Returns the string representation of the object.
         """
 
@@ -1305,15 +1309,15 @@
 
 
     # Add the button to have names show up on hover or always:
     fig = switch_names_on_off(fig)
 
     fig.update_traces(hoverlabel=dict(font=dict(size=10))) #TEXT SIZE set to 10 again. This works for the "Show names on hover" option, but not for "Always show names" option
     
-    qc_derivative = [QC_derivative(content=fig, name='Sensors_positions', content_type='plotly', description_for_user="Magnetometers names end with '1' like 'MEG0111'. Gradiometers names end with '2' and '3' like 'MEG0112', 'MEG0113'. ")]
+    qc_derivative = [QC_derivative(content=fig, name='Sensors_positions', content_type='plotly', description_for_user="Magnetometers names end with '1' like 'MEG0111'. Gradiometers names end with '2' and '3' like 'MEG0112', 'MEG0113'. ", fig_order=-1)]
 
     return qc_derivative 
 
 
 def boxplot_epochs(df_mg: pd.DataFrame, ch_type: str, what_data: str, x_axis_boxes: str, verbose_plots: bool):
 
     """
@@ -1919,22 +1923,18 @@
     Returns
     -------
     QC_derivative
         QC_derivative object with plotly figure as content
 
     """
 
-    print('___Plot this', tsv_pie_path)
-
-    # Get the base name
+    #if it s not the right ch kind in the file
     base_name = os.path.basename(tsv_pie_path) #name of the fimal file
     
-    #if not any(df.columns.str.contains(m_or_g)) and not any(df.index.str.contains(m_or_g)): 
     if m_or_g not in base_name.lower():
-    #if it s not the right ch kind in the file
         return []
     
     # Read the data from the TSV file into a DataFrame
     df = pd.read_csv(tsv_pie_path, sep='\t')
 
     if noise_or_waves == 'noise' and 'PSDnoise' in base_name:
         #check that we input tsv file with the right data
@@ -1956,17 +1956,14 @@
         fig_tit = "Relative amplitude of each band: " 
         fig_name = 'PSD_Relative_band_amplitude_all_channels_'
 
 
         # Set the first column as the index
         df.set_index(df.columns[0], inplace=True)
 
-        print('__Check here__')
-        print(df)
-
         # Extract total_amplitude into a separate variable
         total_amplitude = df['total_amplitude'].loc['absolute_'+m_or_g]
 
         #drop total ampl:
         df_no_total = copy.deepcopy(df.drop('total_amplitude', axis=1))
 
         # Extract rows into lists
@@ -2852,14 +2849,123 @@
     head_derivs = [QC_derivative(fig1, 'Head_position_rotation_average_mne', 'matplotlib', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
 
     return head_derivs
 
 
 #__________ECG/EOG__________#
 
+def plot_ECG_EOG_channel(ch_data: np.ndarray or list, peaks: np.ndarray or list, ch_name: str, fs: float, verbose_plots: bool):
+
+    """
+    Plot the ECG channel data and detected peaks
+    
+    Parameters
+    ----------
+    ch_data : list or np.ndarray
+        Data of the channel
+    peaks : list or np.ndarray
+        Indices of the peaks in the data
+    ch_name : str
+        Name of the channel
+    fs : int
+        Sampling frequency of the data
+    verbose_plots : bool
+        If True, show the figure in the notebook
+        
+    Returns
+    -------
+    fig : plotly.graph_objects.Figure
+        Plot of the channel data and detected peaks
+        
+    """
+
+    time = np.arange(len(ch_data))/fs
+    fig = go.Figure()
+    fig.add_trace(go.Scatter(x=time, y=ch_data, mode='lines', name=ch_name + ' data'))
+    fig.add_trace(go.Scatter(x=time[peaks], y=ch_data[peaks], mode='markers', name='peaks'))
+    fig.update_layout(xaxis_title='time, s', 
+                yaxis = dict(
+                showexponent = 'all',
+                exponentformat = 'e'),
+                yaxis_title='Amplitude',
+                title={
+                'text': ch_name,
+                'y':0.85,
+                'x':0.5,
+                'xanchor': 'center',
+                'yanchor': 'top'})
+    
+    if verbose_plots is True:
+        fig.show()
+
+    return fig
+
+
+def plot_ECG_EOG_channel_csv(f_path, verbose_plots: bool):
+
+    """
+    Plot the ECG channel data and detected peaks
+    
+    Parameters
+    ----------
+    ch_data : list or np.ndarray
+        Data of the channel
+    peaks : list or np.ndarray
+        Indices of the peaks in the data
+    ch_name : str
+        Name of the channel
+    fs : int
+        Sampling frequency of the data
+    verbose_plots : bool
+        If True, show the figure in the notebook
+        
+    Returns
+    -------
+    fig : plotly.graph_objects.Figure
+        Plot of the channel data and detected peaks
+        
+    """
+
+    #if its not the right file, skip:
+    base_name = os.path.basename(f_path) #name of the fimal file
+    
+    if 'ecgchannel' not in base_name.lower() and 'eogchannel' not in base_name.lower():
+        return []
+
+    df = pd.read_csv(f_path, sep='\t') 
+
+    #name of the first column if it starts with 'ECG' or 'EOG':
+    ch_name = df.columns[1]
+    ch_data = df[ch_name].values
+    peaks = df['event_indexes'].dropna()
+    peaks = [int(x) for x in peaks]
+    fs = int(df['fs'].dropna())
+
+    time = np.arange(len(ch_data))/fs
+    fig = go.Figure()
+    fig.add_trace(go.Scatter(x=time, y=ch_data, mode='lines', name=ch_name + ' data'))
+    fig.add_trace(go.Scatter(x=time[peaks], y=ch_data[peaks], mode='markers', name='peaks'))
+    fig.update_layout(xaxis_title='time, s', 
+                yaxis = dict(
+                showexponent = 'all',
+                exponentformat = 'e'),
+                yaxis_title='Amplitude',
+                title={
+                'text': ch_name,
+                'y':0.85,
+                'x':0.5,
+                'xanchor': 'center',
+                'yanchor': 'top'})
+    
+    ch_deriv = [QC_derivative(fig, ch_name, 'plotly', fig_order = 1)]
+
+    if verbose_plots is True:
+        fig.show()
+
+    return ch_deriv
 
 def figure_x_axis(df, metric):
 
     ''''
     Get the x axis for the plot based on the metric.
     
     Parameters
@@ -2977,22 +3083,24 @@
     Plot the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
     Based on the data from tsv file.
     
     Parameters
     ----------
     df : pd.DataFrame
         Data frame with the data.
+    artifact_lvl : float
+        The threshold for the artifact amplitude.
     t : np.ndarray
         Time vector.
     m_or_g : str
         Either 'mag' or 'grad'.
-    fig_tit: str
+    ecg_or_eog : str
+        Either 'ECG' or 'EOG'.
+    title : str
         The title of the figure.
-    chs_by_lobe : dict
-        dictionary with channel objects sorted by lobe
     flip_data : bool
         If True, the absolute value of the data will be used for the calculation of the mean artifact amplitude. Default to 'flip'. 
         'flip' means that the data will be flipped if the peak of the artifact is negative. 
         This is donr to get the same sign of the artifact for all channels, then to get the mean artifact amplitude over all channels and the threshold for the artifact amplitude onbase of this mean
         And also for the reasons of visualization: the artifact amplitude is always positive.
     smoothed: bool
         Plot smoothed data (true) or nonrmal (false)
@@ -3003,32 +3111,31 @@
     -------
     fig : plotly.graph_objects.Figure
         The plotly figure with the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
 
         
     """
 
-    fig_tit=ecg_or_eog+title
+    fig_tit=ecg_or_eog.upper()+title
 
-    #if df and not df.empty: #if affected channels present:
     if df is not None:
         if smoothed is True:
             metric = ecg_or_eog+'_smoothed'
         elif smoothed is False:
             metric = ecg_or_eog
         fig = plot_df_of_channels_data_as_lines_by_lobe_csv(None, metric, t, m_or_g, df)
 
         #decorate the plot:
         ch_type_tit, unit = get_tit_and_unit(m_or_g)
         fig.update_layout(
             xaxis_title='Time in seconds',
             yaxis = dict(
                 showexponent = 'all',
                 exponentformat = 'e'),
-            yaxis_title='Mean artifact magnitude in '+unit,
+            yaxis_title='Mean magnitude in '+unit,
             title={
                 'text': fig_tit+str(len(df))+' '+ch_type_tit,
                 'y':0.85,
                 'x':0.5,
                 'xanchor': 'center',
                 'yanchor': 'top'})
 
@@ -3052,14 +3159,56 @@
         fig.add_trace(go.Scatter(x=t, y=[(-artifact_lvl)]*len(t), line=dict(color='black'), name='-Thres=mean_peak/norm_lvl'))
 
     if verbose_plots is True:
         fig.show()
 
     return fig
 
+def plot_mean_ecg_ch_data_csv(f_path: str, ecg_or_eog: str, verbose_plots: bool):
+
+    #if it s not the right ch kind in the file
+    base_name = os.path.basename(f_path) #name of the final file
+    if ecg_or_eog.lower() + 'channel' not in base_name.lower():
+        return []
+
+    # Load the data from the .tsv file into a DataFrame
+    df = pd.read_csv(f_path, sep='\t')
+
+    # Create a scatter plot
+    fig = go.Figure(data=go.Scatter(x=df['mean_rwave_time'], y=df['mean_rwave'], mode='lines'))
+
+    # Set the plot's title and labels
+    if 'recorded' in df['recorded_or_reconstructed'][0]:
+        which = 'recorded'
+    elif 'reconstructed' in df['recorded_or_reconstructed'][0]:
+        which = 'reconstructed'
+    else:
+        which = ''
+    
+    fig.update_layout(
+            xaxis_title='Time, s',
+            yaxis = dict(
+                showexponent = 'all',
+                exponentformat = 'e'),
+            yaxis_title='Signal amplitude, V',
+            title={
+                'text': 'Mean data of the '+ which +' ' + ecg_or_eog.upper() + ' channel',
+                'y':0.85,
+                'x':0.5,
+                'xanchor': 'center',
+                'yanchor': 'top'})
+    
+    # Show the plot
+    if verbose_plots is True:
+        fig.show()
+
+    mean_ecg_ch_deriv = [QC_derivative(fig, ecg_or_eog+'mean_ecg_ch_data', 'plotly', fig_order = 2)]
+
+    return mean_ecg_ch_deriv
+
 
 def plot_artif_per_ch_correlated_lobes_csv(f_path: str, m_or_g: str, ecg_or_eog: str, flip_data: bool, verbose_plots: bool):
 
     """
     This is the final function.
     Plot average artifact for each channel, colored by lobe, 
     channels are split into 3 separate plots, based on their correlation with mean_rwave: equal number of channels in each group.
@@ -3084,27 +3233,34 @@
         List of objects of class Avg_artif
     affected_derivs : list
         List of objects of class QC_derivative (plots)
     
 
     """
 
+    #if its not the right file, skip:
+    base_name = os.path.basename(f_path) #name of the fimal file
+    
+    if 'desc-ecgs' not in base_name.lower() and 'desc-eogs' not in base_name.lower():
+        return []
+
 
     ecg_or_eog = ecg_or_eog.lower()
 
     df = pd.read_csv(f_path, sep='\t') #TODO: maybe remove reading csv and pass directly the df here?
+    
     df = df.drop(df[df['Type'] != m_or_g].index) #remove non needed channel kind
 
     artif_time_vector = figure_x_axis(df, metric=ecg_or_eog)
 
     most_correlated, middle_correlated, least_correlated, _, _, _ = split_correlated_artifacts_into_3_groups_csv(df, ecg_or_eog)
 
     smoothed = True
     fig_most_affected = plot_affected_channels_csv(most_correlated, None, artif_time_vector, m_or_g, ecg_or_eog, title = ' most affected channels (smoothed): ', flip_data=flip_data, smoothed = smoothed, verbose_plots=False)
-    fig_middle_affected = plot_affected_channels_csv(middle_correlated, None, artif_time_vector, m_or_g, ecg_or_eog, title = ' middle affected channels (smoothed): ', flip_data=flip_data, smoothed = smoothed, verbose_plots=False)
+    fig_middle_affected = plot_affected_channels_csv(middle_correlated, None, artif_time_vector, m_or_g, ecg_or_eog, title = ' moderately affected channels (smoothed): ', flip_data=flip_data, smoothed = smoothed, verbose_plots=False)
     fig_least_affected = plot_affected_channels_csv(least_correlated, None, artif_time_vector, m_or_g, ecg_or_eog, title = ' least affected channels (smoothed): ', flip_data=flip_data, smoothed = smoothed, verbose_plots=False)
 
 
     #set the same Y axis limits for all 3 figures for clear comparison:
 
     if ecg_or_eog.lower() == 'ecg' and smoothed is False:
         prefix = 'mean_ecg_sec_'
@@ -3131,18 +3287,19 @@
     fig_least_affected.update_layout(yaxis_range=ylim)
 
     if verbose_plots is True:
         fig_most_affected.show()
         fig_middle_affected.show()
         fig_least_affected.show()
     
+    m_or_g_order = 0.1 if m_or_g == 'mag' else 0.2
     affected_derivs = []
-    affected_derivs += [QC_derivative(fig_most_affected, ecg_or_eog+'most_affected_channels_'+m_or_g, 'plotly')]
-    affected_derivs += [QC_derivative(fig_middle_affected, ecg_or_eog+'middle_affected_channels_'+m_or_g, 'plotly')]
-    affected_derivs += [QC_derivative(fig_least_affected, ecg_or_eog+'least_affected_channels_'+m_or_g, 'plotly')]
+    affected_derivs += [QC_derivative(fig_most_affected, ecg_or_eog+'most_affected_channels_'+m_or_g, 'plotly', fig_order = 3.01+m_or_g_order)] #for exaple for mage we get: 3.11
+    affected_derivs += [QC_derivative(fig_middle_affected, ecg_or_eog+'middle_affected_channels_'+m_or_g, 'plotly', fig_order = 3.02+m_or_g_order)]
+    affected_derivs += [QC_derivative(fig_least_affected, ecg_or_eog+'least_affected_channels_'+m_or_g, 'plotly', fig_order = 3.03+m_or_g_order)]
 
    
     return affected_derivs
 
 
 def plot_correlation_csv(f_path: str, ecg_or_eog: str, m_or_g: str, verbose_plots=False):
 
@@ -3164,14 +3321,20 @@
     Returns
     -------
     corr_derivs : list
         List with 1 QC_derivative instance: Figure with correlation coefficient and p-value between mean R wave and each channel in artif_per_ch.
     
     """
 
+    #if its not the right file, skip:
+    base_name = os.path.basename(f_path) #name of the fimal file
+    
+    if 'desc-ecgs' not in base_name.lower() and 'desc-eogs' not in base_name.lower():
+        return []
+
     ecg_or_eog = ecg_or_eog.lower()
 
     df = pd.read_csv(f_path, sep='\t') #TODO: maybe remove reading csv and pass directly the df here?
     df = df.drop(df[df['Type'] != m_or_g].index) #remove non needed channel kind
 
     _, _, _, corr_val_of_last_most_correlated, corr_val_of_last_middle_correlated, corr_val_of_last_least_correlated = split_correlated_artifacts_into_3_groups_csv(df, ecg_or_eog)
 
@@ -3184,20 +3347,24 @@
 
     fig = go.Figure(data=traces)
 
     fig.add_shape(type="rect", xref="x", yref="y", x0=0, y0=-0.1, x1=corr_val_of_last_least_correlated, y1=1.1, line=dict(color="Green", width=2), fillcolor="Green", opacity=0.1)
     fig.add_shape(type="rect", xref="x", yref="y", x0=corr_val_of_last_least_correlated, y0=-0.1, x1=corr_val_of_last_middle_correlated, y1=1.1, line=dict(color="Yellow", width=2), fillcolor="Yellow", opacity=0.1)
     fig.add_shape(type="rect", xref="x", yref="y", x0=corr_val_of_last_middle_correlated, y0=-0.1, x1=1, y1=1.1, line=dict(color="Red", width=2), fillcolor="Red", opacity=0.1)
 
-    #set axis titles:
-    fig.update_xaxes(title_text='Correlation coefficient')
-    fig.update_yaxes(title_text='P-value')
-
-    #set title:
-    fig.update_layout(title_text=tit+': Pearson correlation between reference '+ecg_or_eog+' epoch and '+ecg_or_eog+' epoch in each channel')
-
+    fig.update_layout(
+        title={
+            'text': tit+': Pearson correlation between reference '+ecg_or_eog.upper()+' epoch and '+ecg_or_eog.upper()+' epoch in each channel',
+            'y':0.85,
+            'x':0.5,
+            'xanchor': 'center',
+            'yanchor': 'top'},
+        xaxis_title='Correlation coefficient',
+        yaxis_title = 'P-value') 
+    
     if verbose_plots is True:
         fig.show()
 
-    corr_derivs = [QC_derivative(fig, 'Corr_values_'+ecg_or_eog, 'plotly', description_for_user='Absolute value of the correlation coefficient is shown here. The sign would only represent the position of the channel towards magnetic field. <p>- Green: 33% of all channels that have the weakest correlation with mean ' +ecg_or_eog +'; </p> <p>- Yellow: 33% of all channels that have mild correlation with mean ' +ecg_or_eog +';</p> <p>- Red: 33% of all channels that have the stronges correlation with mean ' +ecg_or_eog +'. </p>')]
+    m_or_g_order = 0.1 if m_or_g == 'mag' else 0.2
+    corr_derivs = [QC_derivative(fig, 'Corr_values_'+ecg_or_eog, 'plotly', description_for_user='Absolute value of the correlation coefficient is shown here. The sign would only represent the position of the channel towards magnetic field. <p>- Green: 33% of all channels that have the weakest correlation with mean ' +ecg_or_eog +'; </p> <p>- Yellow: 33% of all channels that have mild correlation with mean ' +ecg_or_eog +';</p> <p>- Red: 33% of all channels that have the stronges correlation with mean ' +ecg_or_eog +'. </p>', fig_order = 4+m_or_g_order)]
 
     return corr_derivs
```

### Comparing `meg_qc-0.1.6/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.1.7/meg_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg-qc
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.6/meg_qc.egg-info/SOURCES.txt` & `meg_qc-0.1.7/meg_qc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 versioneer.py
 meg_qc/__init__.py
 meg_qc/__main__.py
 meg_qc/_version.py
 meg_qc.egg-info/PKG-INFO
 meg_qc.egg-info/SOURCES.txt
 meg_qc.egg-info/dependency_links.txt
-meg_qc.egg-info/requires.txt
 meg_qc.egg-info/top_level.txt
 meg_qc/calculation/initial_meg_qc.py
 meg_qc/calculation/meg_qc_pipeline.py
 meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
 meg_qc/calculation/metrics/Head_meg_qc.py
 meg_qc/calculation/metrics/PSD_meg_qc.py
 meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
```

### Comparing `meg_qc-0.1.6/setup.cfg` & `meg_qc-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/setup.py` & `meg_qc-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.6/versioneer.py` & `meg_qc-0.1.7/versioneer.py`

 * *Files identical despite different names*

