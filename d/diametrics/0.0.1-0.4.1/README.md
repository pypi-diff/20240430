# Comparing `tmp/diametrics-0.0.1.tar.gz` & `tmp/diametrics-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diametrics-0.0.1.tar", max compression
+gzip compressed data, was "diametrics-0.4.1.tar", max compression
```

## Comparing `diametrics-0.0.1.tar` & `diametrics-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-04 11:01:59.635157 diametrics-0.0.1/LICENSE
--rw-r--r--   0        0        0     1531 2023-05-31 12:33:40.472427 diametrics-0.0.1/README.md
--rw-r--r--   0        0        0      561 2024-04-22 17:15:53.624066 diametrics-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 12:33:40.476428 diametrics-0.0.1/src/diametrics/__init__.py
--rw-r--r--   0        0        0     4916 2023-05-31 12:33:40.476428 diametrics-0.0.1/src/diametrics/_glycemic_events_helper.py
--rw-r--r--   0        0        0    13313 2023-05-31 12:33:40.476428 diametrics-0.0.1/src/diametrics/helper.py
--rw-r--r--   0        0        0    25859 2024-04-23 11:04:28.059173 diametrics-0.0.1/src/diametrics/metrics.py
--rw-r--r--   0        0        0     8469 2024-04-22 17:15:53.624066 diametrics-0.0.1/src/diametrics/preprocessing.py
--rw-r--r--   0        0        0     6299 2024-04-22 17:15:53.624066 diametrics-0.0.1/src/diametrics/transform.py
--rw-r--r--   0        0        0    11344 2024-04-22 17:22:56.116098 diametrics-0.0.1/src/diametrics/visualizations.py
--rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 diametrics-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 14:58:50.256220 diametrics-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1749 2024-04-30 14:58:50.256220 diametrics-0.4.1/README.md
+-rw-r--r--   0        0        0      562 2024-04-30 14:59:09.644250 diametrics-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 14:58:50.260220 diametrics-0.4.1/src/diametrics/__init__.py
+-rw-r--r--   0        0        0     4961 2024-04-30 14:58:50.260220 diametrics-0.4.1/src/diametrics/_glycemic_events_helper.py
+-rw-r--r--   0        0        0     1284 2024-04-30 14:58:50.260220 diametrics-0.4.1/src/diametrics/directory_structure.txt
+-rw-r--r--   0        0        0    13313 2024-04-30 14:58:50.264220 diametrics-0.4.1/src/diametrics/helper.py
+-rw-r--r--   0        0        0    26028 2024-04-30 14:58:50.264220 diametrics-0.4.1/src/diametrics/metrics.py
+-rw-r--r--   0        0        0     8522 2024-04-30 14:58:50.264220 diametrics-0.4.1/src/diametrics/preprocessing.py
+-rw-r--r--   0        0        0     6438 2024-04-30 14:58:50.264220 diametrics-0.4.1/src/diametrics/transform.py
+-rw-r--r--   0        0        0    10741 2024-04-30 14:58:50.264220 diametrics-0.4.1/src/diametrics/visualizations.py
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 diametrics-0.4.1/PKG-INFO
```

### Comparing `diametrics-0.0.1/LICENSE` & `diametrics-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diametrics-0.0.1/README.md` & `diametrics-0.4.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# diametrics
-A Python package for calculating the metrics for diabetes control from CGM and FGM data.
+# Diametrics
+Diametrics is a Python package and associated [WebApp](https://diametrics.org) designed for the analysis of Continuous Glucose Monitoring (CGM) data. 
 
-The goal of this project is to enable researchers to quickly calculate the metrics of diabetes control outlined in the Internation consensus on the use of continuous glucose monitors in Python.
+The goal of this package is to enable researchers to quickly calculate the metrics of diabetes control outlined in the [international consensus on the use of continuous glucose monitors](https://diabetesjournals.org/care/article/40/12/1631/37000/International-Consensus-on-Use-of-Continuous) in Python.
+ 
+
+Diametrics has functionality for data preprocessing, calculating standard metrics of glycemic control and data visualization, using Plotly.
 
-The method used for calculating the metrics are all based on the advice given in the consensus.
 
 ## Contents 
 The diametrics functions are contained within a metrics.py file. The functions are
 
 `all_metrics` calculates all of the below metrics
 
 `average_glucose` mean glucose data given
```

### Comparing `diametrics-0.0.1/pyproject.toml` & `diametrics-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "diametrics"
-version = "0.0.1"
+version = "0.4.1"
 description = "A package for calculating the metrics of glycemic control for Diabetes from CGM data"
 authors = ["Catherine Russon"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -19,7 +19,8 @@
 plotly = "^5.21.0"
 nbformat = "^5.10.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `diametrics-0.0.1/src/diametrics/_glycemic_events_helper.py` & `diametrics-0.4.1/src/diametrics/_glycemic_events_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from datetime import timedelta
 import numpy as np
 import warnings
 warnings.filterwarnings('ignore')
 
 def calc_diff(group):
-    row1 = group.iloc[0]
+    row1 = group.iloc[0].copy()
     endtime = group.iloc[-1]['time_rep']
     starttime = row1['time_rep']
     diff = endtime-starttime
     row1['diff'] = diff
     return row1
 
 def collapse_bool_array(df, bool_array):
@@ -18,35 +18,35 @@
     df_unique = pd.DataFrame({'time_rep': df['time'], 'glc_rep':
                             df['glc'], 'unique_number': unique_num,
                             'consec_readings': number_consec})
     df_unique['time_rep'] = pd.to_datetime(df_unique['time_rep'])
     # Drop any null glucose readings and reset index
     df_unique.dropna(subset=['glc_rep'], inplace=True)
     df_unique.reset_index(inplace=True, drop=True)
-    diff = df_unique.groupby('unique_number').apply(lambda group: calc_diff(group))
+    diff = df_unique.groupby('unique_number').apply((lambda group: calc_diff(group)), include_groups=False)
     diff = diff.drop(columns=['glc_rep'])#.reset_index()
     return diff
 
 def calc_duration(unique_min, mins):
     # Only keep hypos that are 15 mins or longer (smaller than this doesn't count)
-    results = unique_min[unique_min['diff'] >= timedelta(minutes=mins)]
+    results = unique_min[unique_min['diff'] >= timedelta(minutes=mins)].copy()
 
     # Fill the consec readings with binary value to show whether they are hypos or
     # the periods between hypos
     results['consec_readings'] = results['consec_readings'].fillna(-1)
     results['event'] = results['consec_readings'] > 0
 
     # Merge any consecutive values left by removal of too-short episodes using
     # a new unique number
     results['unique'] = results['event'].ne(results['event'].shift()).cumsum()
     return results
 
 def merge_events(results, mins):
     # Group by the unique number, select the min values and select relevant columns
-    results_grouped = results.groupby('unique').min()[['time_rep',  'event', 'diff']] #'glc_rep',
+    results_grouped = results.groupby('unique').min()[['time_rep',  'event', 'diff']].copy() #'glc_rep',
     results_grouped['diff2'] = results_grouped['time_rep'].diff().shift(-1)
     # Drop the non-hypo periods and then drop the hypo column
     final_results = results_grouped.loc[results_grouped['event'] ==
                                         True].drop(columns=['event'])
                                         # Rename columns
     final_results.columns = ['start_time',  'initial_duration', 'duration'] # 'min_glc',
```

### Comparing `diametrics-0.0.1/src/diametrics/helper.py` & `diametrics-0.4.1/src/diametrics/helper.py`

 * *Files identical despite different names*

### Comparing `diametrics-0.0.1/src/diametrics/metrics.py` & `diametrics-0.4.1/src/diametrics/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     def run(group):
         # Find peaks and troughs
         peaks, _ = signal.find_peaks(group['glc'], prominence=group['glc'].std())
         troughs, _ = signal.find_peaks(-group['glc'], prominence=group['glc'].std())
 
         # Consolidate peaks and troughs, and sort by time
         points = np.sort(np.concatenate((peaks, troughs, [0, len(group) - 1])))
-        selected_points = group.iloc[points]
+        selected_points = group.iloc[points].copy()
 
         # Calculate differences between consecutive points
         selected_points['diff'] = selected_points['glc'].diff().abs()
 
         # Calculate MAGE
         mage_value = selected_points['diff'].mean()
 
@@ -381,15 +381,15 @@
             'tir_lv1_hypo': tir_lv1_hypo,
             'tir_lv2_hypo': tir_lv2_hypo,
             'tir_lv1_hyper': tir_lv1_hyper,
             'tir_lv2_hyper': tir_lv2_hyper
         })
     
     if 'ID' in df.columns:
-        results = df.groupby('ID').apply(run, units=units).reset_index()        
+        results = df.groupby('ID').apply((lambda group: run(group, units=units)), include_groups=False).reset_index()        
         return results
     else:    
         results = run(df, units)
         return results
 
 
 def glycemic_episodes(df, units=None, hypo_lv1_thresh=None, hypo_lv2_thresh=None, hyper_lv1_thresh=None, hyper_lv2_thresh=None, mins=15, long_mins=120):
@@ -444,15 +444,15 @@
                     'number_lv2_hypers':lv2_hypers,
                     'number_prolonged_hypers':prolonged_hypers, 
                     'avg_length_hypers':avg_length_hypers,
                     'total_time_in_hyper':total_time_hypers})
         return results
     
     if 'ID' in df.columns:
-        results = df.groupby('ID').apply(lambda group: run(group, units, hypo_lv1_thresh, hypo_lv2_thresh, hyper_lv1_thresh, hyper_lv2_thresh, mins, long_mins))
+        results = df.groupby('ID').apply((lambda group: run(group, units, hypo_lv1_thresh, hypo_lv2_thresh, hyper_lv1_thresh, hyper_lv2_thresh, mins, long_mins)), include_groups=False)
         return results
     else:    
         results = run(df, units, hypo_lv1_thresh, hypo_lv2_thresh, hyper_lv1_thresh, hyper_lv2_thresh, mins, long_mins)
         return results
 
 
 def data_sufficiency(df, start_time=None, end_time=None, gap_size=None):
@@ -483,15 +483,19 @@
         end_time = end_time or df['time'].iloc[-1]
         days = (end_time-start_time).total_seconds()/86400
 
         # Subset the DataFrame based on the provided time range
         df = df.loc[(df['time'] >= start_time) & (df['time'] <= end_time)]
 
         # Calculate the interval size
-        gap_size = timedelta(minutes=gap_size) or df['time'].diff().mode().iloc[0]
+        if gap_size == None:
+            df['time'].diff().mode().iloc[0]
+        else:
+            gap_size = timedelta(minutes=gap_size)
+            
         # If it doesn't conform to 5 or 15 then don't count it
         if ((timedelta(minutes=4) < gap_size) & (gap_size < timedelta(minutes=6))):
             freq = '5min'
         elif ((timedelta(minutes=14) < gap_size) & (gap_size < timedelta(minutes=16))):
             freq = '15min'
         else:
             raise ValueError('Invalid gap size. Gap size must be 5 or 15.')
@@ -512,15 +516,15 @@
             'start_dt': str(start_time.round('min')),
             'end_dt': str(end_time.round('min')),
             'num_days':days,
             'data_sufficiency': np.round(data_sufficiency, 1)
         })
     
     if 'ID' in df.columns:
-        results = df.groupby('ID').apply(lambda group: run(group, gap_size, start_time, end_time)).reset_index()
+        results = df.groupby('ID').apply((lambda group: run(group, gap_size, start_time, end_time)), include_groups=False).reset_index()
         return results
     else:    
         results = run(df, gap_size, start_time, end_time)
         return results
 
 
 def calc_bgi(glucose, units):
```

### Comparing `diametrics-0.0.1/src/diametrics/preprocessing.py` & `diametrics-0.4.1/src/diametrics/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pandas as pd
 import datetime
 import numpy as np
 import warnings
 import copy
+pd.set_option('future.no_silent_downcasting', True)
+
 
 def check_df(df):
     """
     Check if the given object is a valid DataFrame.
     
     Args:
         df (object): The object to be checked.
```

### Comparing `diametrics-0.0.1/src/diametrics/transform.py` & `diametrics-0.4.1/src/diametrics/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,29 +44,29 @@
     df.columns = df.iloc[2]
     # Drop top rows
     df = df.iloc[3:]
     df.reset_index(inplace=True, drop=True)
     # Keep important columns based on column names
     if 'Historic Glucose(mmol/L)' in df.columns:
         df = df.loc[:, ('Meter Timestamp', 'Historic Glucose(mmol/L)', 'Scan Glucose(mmol/L)')]
-        dayfirst = True
+        format = '%d-%m-%Y %H:%M'
     elif 'Historic Glucose(mg/dL)' in df.columns:
         df = df.loc[:, ('Meter Timestamp', 'Historic Glucose(mg/dL)', 'Scan Glucose(mg/dL)')]
-        dayfirst = False
+        format = '%m-%d-%Y %H:%M'
     elif 'Historic Glucose mmol/L' in df.columns:
         df = df.loc[:, ('Device Timestamp', 'Historic Glucose mmol/L', 'Scan Glucose mmol/L')]
-        dayfirst = True
+        format = '%d-%m-%Y %I:%M %p' 
     else:
         df = df = df.loc[:, ('Device Timestamp', 'Historic Glucose mg/dL', 'Scan Glucose mg/dL')]
-        dayfirst = False
+        format = '%m-%d-%Y %I:%M %p'
     # Rename columns
     df.columns = ['time', 'glc', 'scan_glc']
 
     # Convert 'time' column to datetime
-    df['time'] = pd.to_datetime(df['time'], dayfirst=dayfirst)
+    df['time'] = pd.to_datetime(df['time'], format=format)
 
     # Drop NaN values and sort by 'time'
     df = df.dropna(subset=['time', 'glc']).sort_values('time').reset_index(drop=True)
 
     return df
 
 def convert_dexcom(df):
@@ -185,9 +185,10 @@
                 print('autoprocessing')
 
             # Set ID
             df_std['ID'] = filename.split('.')[0]
 
             # Append
             total_cgm.append(df_std)
-
-    return pd.concat(total_cgm, ignore_index=True)
+    final_df = pd.concat(total_cgm, ignore_index=True)
+    final_df = final_df.sort_values(['ID', 'time']).reset_index(drop=True)
+    return final_df
```

### Comparing `diametrics-0.0.1/src/diametrics/visualizations.py` & `diametrics-0.4.1/src/diametrics/visualizations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import plotly.express as px
 import pandas as pd
 import numpy as np
 import plotly.graph_objects as go
-from diametrics import preprocessing
+from diametrics import preprocessing, metrics
 
 UNIT_THRESHOLDS = {
     'mmol': {
         'low': 2.1,
         'norm_tight': 7.8,
         'hypo_lv1': 3.9,
         'hypo_lv2': 3,
@@ -36,18 +36,27 @@
         df (pd.DataFrame): DataFrame containing glucose data.
         violin (bool): If True, generate a violin plot. If False, generate a box plot.
 
     Returns:
         fig: Plotly figure object representing the box plot or violin plot.
     """
     if violin:
-        return px.violin(df, y='glc', x='ID')
+        fig = px.violin(df, y='glc', x='ID', box=True)
+
     else:
-        return px.box(df, x='ID', y="glc")
+        fig = px.box(df, x='ID', y="glc")
 
+    fig.update_layout(
+        title = 'Overall Glucose Distribution',
+        yaxis_title = 'Glucose',
+        xaxis_title = 'ID',
+        #width=figure_width,  # Set the width of the figure
+        #height=figure_height  # Set the height of the figure
+    )   
+    return fig
 
 
 
 def glucose_trace(df, ID=None, figure_width=800, figure_height=400):
     """
     Generate a glucose trace plot.
 
@@ -130,40 +139,14 @@
         xaxis_title = 'Date',
         width=figure_width,  # Set the width of the figure
         height=figure_height  # Set the height of the figure
         )
     return fig
 
 
-def get_pie(df):
-    """
-    Calculate the counts for different glucose level ranges.
-
-    Args:
-        df (pd.DataFrame): DataFrame containing glucose data.
-
-    Returns:
-        list: List of values representing the counts for different glucose level ranges.
-    """
-    units = preprocessing.detect_units(df)
-    # Use this to get the thresholds from the global dictionary
-    thresholds = UNIT_THRESHOLDS.get(units, {})
-    norm_tight = thresholds.get('norm_tight')
-    hypo_lv1 = thresholds.get('hypo_lv1')
-    hypo_lv2 = thresholds.get('hypo_lv2')
-    hyper_lv1 = thresholds.get('hyper_lv1')
-    hyper_lv2 = thresholds.get('hyper_lv2')
-    
-    hypo2 = (df['glc']<hypo_lv2).sum()
-    hypo1 = ((df['glc']>=hypo_lv2) & (df['glc']<hypo_lv1)).sum()
-    norm1 = ((df['glc']>=hypo_lv1 )& (df['glc']<=norm_tight)).sum()
-    norm2 = ((df['glc']>=norm_tight )& (df['glc']<=hyper_lv1)).sum()
-    hyper1 = ((df['glc']>hyper_lv1) & (df['glc']<=hyper_lv2)).sum()
-    hyper2 = (df['glc']>hyper_lv2).sum()
-    return [hypo2, hypo1, norm1, norm2, hyper1, hyper2]
     
 
 def tir_pie(df, ID=None):
     """
     Generate a pie chart to visualize the time spent in different glucose level ranges.
 
     Args:
@@ -172,18 +155,18 @@
 
     Returns:
         fig: Plotly figure object representing the pie chart.
     """
     if 'ID' in df.columns:
         ID = ID or df['ID'].iloc[0]
         df = df.loc[df['ID']==ID]
-    print('HEEEELP')
-    values = get_pie(df)
-    labels = ['Level 2 hypoglycemia (<3mmol/L)', 'Level 1 hypoglycemia (3-3.9mmol/L)', 'Normal range 1 (3.9-7.8mmol/L)','Normal range 2 (3.9-10mmol/L)', 'Level 1 hyperglycemia (10-13.9mmol/L)','Level 2 hyperglycemia (>13.9mmol/L)',]
+    labels = ['Level 2 hypoglycemia (<3mmol/L)', 'Level 1 hypoglycemia (3-3.9mmol/L)', 'Normal range 1 (3.9-7.8mmol/L)', 'Normal range 2 (7.8-10mmol/L)', 'Level 1 hyperglycemia (10-13.9mmol/L)','Level 2 hyperglycemia (>13.9mmol/L)',]
     
+    tir = metrics.time_in_range(df)
+    values = [tir['tir_lv2_hypo'], tir['tir_lv1_hypo'], tir['tir_norm_tight'], tir['tir_normal']-tir['tir_norm_tight'], tir['tir_lv1_hyper'], tir['tir_lv2_hyper']]
     fig = go.Figure()
     fig.add_trace(go.Pie(values=values, labels=labels),) # marker_colors=COLORS, ,opacity=0.5
     fig.update_layout(
         title = 'Percentage time in range')
         
     return fig
```

