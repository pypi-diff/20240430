# Comparing `tmp/qceltis-0.1-py3-none-any.whl.zip` & `tmp/qceltis-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 32139 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-11 21:56 mod/__init__.py
--rw-rw-rw-  2.0 fat    18150 b- defN 24-Apr-11 18:46 mod/general_functions.py
--rw-rw-rw-  2.0 fat    67344 b- defN 24-Apr-11 18:46 mod/idbased_metrics.py
--rw-rw-rw-  2.0 fat    33080 b- defN 24-Apr-11 18:46 mod/mzml_extract.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    31110 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      782 b- defN 24-Apr-18 21:01 qceltis-0.1.dist-info/RECORD
-10 files, 151698 bytes uncompressed, 30815 bytes compressed:  79.7%
+Zip file size: 41183 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-11 21:56 qceltis/__init__.py
+-rw-rw-rw-  2.0 fat    25014 b- defN 24-Apr-30 18:10 qceltis/main.py
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-11 21:56 qceltis/mod/__init__.py
+-rw-rw-rw-  2.0 fat    18150 b- defN 24-Apr-11 18:46 qceltis/mod/general_functions.py
+-rw-rw-rw-  2.0 fat    67355 b- defN 24-Apr-29 07:56 qceltis/mod/idbased_metrics.py
+-rw-rw-rw-  2.0 fat    33089 b- defN 24-Apr-29 07:56 qceltis/mod/mzml_extract.py
+-rw-rw-rw-  2.0 fat    26499 b- defN 24-Apr-11 18:46 qceltis/templates/report_template.html
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    31127 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       46 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1069 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/RECORD
+13 files, 203552 bytes uncompressed, 39399 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
-Filename: mod/__init__.py
+Filename: qceltis/__init__.py
 Comment: 
 
-Filename: mod/general_functions.py
+Filename: qceltis/main.py
 Comment: 
 
-Filename: mod/idbased_metrics.py
+Filename: qceltis/mod/__init__.py
 Comment: 
 
-Filename: mod/mzml_extract.py
+Filename: qceltis/mod/general_functions.py
 Comment: 
 
-Filename: qceltis-0.1.dist-info/LICENSE.txt
+Filename: qceltis/mod/idbased_metrics.py
 Comment: 
 
-Filename: qceltis-0.1.dist-info/METADATA
+Filename: qceltis/mod/mzml_extract.py
 Comment: 
 
-Filename: qceltis-0.1.dist-info/WHEEL
+Filename: qceltis/templates/report_template.html
 Comment: 
 
-Filename: qceltis-0.1.dist-info/entry_points.txt
+Filename: qceltis-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: qceltis-0.1.dist-info/top_level.txt
+Filename: qceltis-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: qceltis-0.1.dist-info/RECORD
+Filename: qceltis-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: qceltis-0.1.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: qceltis-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: qceltis-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mod/general_functions.py` & `qceltis/mod/general_functions.py`

 * *Files identical despite different names*

## Comparing `mod/idbased_metrics.py` & `qceltis/mod/idbased_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import collections
 from collections import defaultdict
 import plotly
 import plotly.express as px
 from sklearn.preprocessing import StandardScaler
 from sklearn.decomposition import PCA
 
-from mod.general_functions import cv, groupname, quant_status, check_threshold, transpose_DF, perc_qc, cv_status, color_list
+from qceltis.mod.general_functions import cv, groupname, quant_status, check_threshold, transpose_DF, perc_qc, cv_status, color_list
 
 enzyme_info =  {'asp-n':{'terminus' : 'N' , 'cleave' : ['D'], 'exceptions' : []},
                 'lys-c' : {'terminus' : 'C' , 'cleave' : ['K'], 'exceptions' : ['KP']},
                 'lys-n':{'terminus' : 'N' , 'cleave' : ['K'], 'exceptions' : []},
                 'thermolysin':{'terminus' : 'N' , 'cleave' : ['A','F','I','L','M','V'],
                                 'exceptions' : ['DA','DF','DI','DL','DM','DV','EA','EF','EI','EL','EM','EV']},
                 'proteinasek':{'terminus' : 'C' , 'cleave' : ['A','F','Y','W','L','I','V'], 'exceptions' : []},
@@ -991,15 +991,15 @@
         protein_report_writer = pd.ExcelWriter(f"{out_dir}/{reportname}_ProteinLevel_QC_Report.xlsx", engine='xlsxwriter')
         pt_quant.to_excel(protein_report_writer, index=False, sheet_name='Protein Quant Summary')
         if groupwise_comparison and threshold_dict['Protein Threshold']:
             pt_grouped_quant.to_excel(protein_report_writer, index=False, sheet_name='Groupwise Protein Quant')
         pt_level_cv.to_excel(protein_report_writer, index=False, sheet_name='Protein Level CV')
         if groupwise_comparison:
             pt_grouped_cv.to_excel(protein_report_writer, index=False, sheet_name='Protein CV Group Summary')
-        protein_report_writer.save()
+        protein_report_writer.close()
 
         #getting protein overall sample dataframe
         if threshold_dict["Protein Threshold"]:
             pt_sample_df = pt_quant[['Filename', f'Protein Threshold = {threshold_dict["Protein Threshold"]}']]
         else:
             pt_sample_df = ""
 
@@ -1099,15 +1099,15 @@
             pep_grouped_tic.to_excel(peptide_report_writer, index=False, sheet_name='Common Peptide TIC Group CV')
         if threshold_dict['Enzyme']:
             dig_df.to_excel(peptide_report_writer, index=False, sheet_name='Miscleavage Threshold')
         if threshold_dict['iRT Label'] and irt_plots:
             irt_level.to_excel(peptide_report_writer, index=False, sheet_name='iRT Peptide Intensity')
         if input_dict['Peptide List']:
             selected_pep_df.to_excel(peptide_threshold_dict, index=False, sheet_name='Selected Peptide Intensity')
-        peptide_report_writer.save()
+        peptide_report_writer.close()
 
         #getting peptide group overall dataframe
         if groupwise_comparison:
             if threshold_dict['Enzyme']:
                 pep_group_df = pep_group_df[["Group", "Peptide Threshold QC Status",
                             f"{threshold_dict['Data Percent Threshold']}% Peptides <= {threshold_dict['CV Percent Threshold']}% CV",
                             "Common Peptide TIC QC Status", "0 Miscleaved Peptides QC Status"]]
@@ -1220,15 +1220,15 @@
             if threshold_dict['Enzyme']:
                 dig_df.to_excel(precursor_report_writer, index=False, sheet_name='Miscleavage Threshold')
             if threshold_dict['iRT Label'] and irt_plots:
                 irt_level.to_excel(precursor_report_writer, index=False, sheet_name='iRT Precursor Intensity')
             if input_dict['Peptide List']:
                 selected_pep_df.to_excel(precursor_report_writer, index=False, sheet_name='Selected Precursor Intensity')
 
-        precursor_report_writer.save()
+        precursor_report_writer.close()
 
         if groupwise_comparison:
             if not input_dict['Peptide Level']:
                 if threshold_dict['Enzyme']:
                     pre_group_df = pre_group_df[["Group", "Precursor Threshold QC Status",f"{threshold_dict['Data Percent Threshold']}% Precursors <= {threshold_dict['CV Percent Threshold']}% CV",
                     "Common Precursor TIC QC Status", "0 Miscleaved Peptides QC Status"]]
                 else:
```

## Comparing `mod/mzml_extract.py` & `qceltis/mod/mzml_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import plotly
 import plotly.graph_objects as go
 import plotly.offline as offline
 from jinja2 import Environment, FileSystemLoader
 from scipy.stats import shapiro
 import time
 
-from mod.general_functions import cv, cv_status, check_threshold, groupname, label_outlier, get_outlier_and_cv_status, only_outlier_status, get_series_status, color_list
+from qceltis.mod.general_functions import cv, cv_status, check_threshold, groupname, label_outlier, get_outlier_and_cv_status, only_outlier_status, get_series_status, color_list
 
 #-------------------------------------------------------------------------- FUNCTIONS ---------------------------------------------------------------------------
 
 def get_mzml_list(mzml_dir):
 
     """
     Retrieves a list of .mzML files from the specified directory.
@@ -669,15 +669,15 @@
     logging.info(f"Saving ID-Free QC Report to {out_dir}/{reportname}_ID-Free_QC_Report.xlsx")
 
     #saving dataframes to excel document
     writer = pd.ExcelWriter(f"{out_dir}/{reportname}_ID-Free_QC_Report.xlsx", engine='xlsxwriter')
     mzml_df.to_excel(writer, index=False, sheet_name="ID-Free Metrics Summary")
     if groupwise_comparison:
         tic_cv.to_excel(writer, index=False, sheet_name='Group TIC CV')
-    writer.save()
+    writer.close()
 
     idfree_report_parameters = create_graphs(mzml_df, tic_cv, groupwise_comparison, groups, mzml_threshold_dict)
 
     mzml_sample_df = get_sample_qc(mzml_df, mzml_threshold_dict, groupwise_comparison, groups)
     if groupwise_comparison:
         idfree_grouped_df = get_idfree_grouped_df(mzml_sample_df, tic_cv, mzml_threshold_dict['TIC CV Threshold'], groups)
     else:
```

## Comparing `qceltis-0.1.dist-info/LICENSE.txt` & `qceltis-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `qceltis-0.1.dist-info/METADATA` & `qceltis-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: qceltis
-Version: 0.1
+Version: 0.1.1
 Summary: Quality Control Package for DIA Proteomics
 Home-page: https://github.com/csmc-vaneykjlab/QCeltis
 Author: Manasa Vegesna
 Author-email: vmanasa1129@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: pymzml ==2.5.0
-Requires-Dist: pandas ==0.25.3
-Requires-Dist: numpy ==1.22.0
-Requires-Dist: xlsxwriter ==3.0.1
-Requires-Dist: plotly ==5.13.0
-Requires-Dist: jinja2 ==3.1.2
-Requires-Dist: scipy ==1.3.3
-Requires-Dist: scikit-learn ==0.22.1
+License-File: LICENSE.txt
+Requires-Dist: pandas >=2.0.1
+Requires-Dist: numpy >=1.24.3
+Requires-Dist: xlsxwriter >=3.2.0
+Requires-Dist: plotly >=5.13.0
+Requires-Dist: jinja2 >=3.1.3
+Requires-Dist: scipy >=1.10.1
+Requires-Dist: scikit-learn >=1.2.2
+Requires-Dist: pymzml >=2.5.9
 
 # QCeltis
 A python package developed for performing quality control analysis on large-scale DIA proteomics datasets. It was designed to enable detection of technical variability due to several factors such as sample collection, transportation, storage, preparation, and/or instrument performance, thus helping improve the accuracy of any biological interpretations of large-scale mass spectrometry-based proteomics data. It allows users to monitor quality control (QC) samples within and across different batches and helps create metrics and plots to not only easily depict outliers, but also to tease out potential causes of these outliers.
 
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
@@ -78,20 +77,24 @@
 First, clone the repository from GitHub:
 
 git clone https://github.com/csmc-vaneykjlab/QCeltis.git
 
 Then, navigate to the downloaded directory and install the package using `pip`:
 
 ~~~bash
-cd qcp
+cd QCeltis
 pip install -r requirements.txt
 ~~~
 
 Alternatively, the package can be installed directly from PyPI
 
+~~~bash
+pip install qceltis
+~~~
+
 ## Usage
 
 If downloaded using github: 
 
 ```python
 python  main.py [-h] --outdirectory OUTDIRECTORY --reportname REPORTNAME [--mzml_directory MZML_DIRECTORY]
                [--ms1_tic_threshold MS1_TIC_THRESHOLD] [--ms2_tic_threshold MS2_TIC_THRESHOLD]
@@ -242,15 +245,15 @@
 MS1 and MS2 Total Ion Current Values are extracted from spectra present in the mzML files and are plotted using a line graph. Total Ion Current values from MS1 and MS2 Spectra are expected to be consistent across the replicate quality control samples. If 'MS1 TIC Threshold' or 'MS2 TIC Threshold' is provided by the user, a dotted line is used to display the threshold in the line graph. Any samples above that threshold are considered as failed samples. Apart from threshold-defined identification of failed samples, outlier analysis is also performed. If extreme values are found across the samples, they are labelled as outliers. 
 
 <ins>TIC Outlier Plot:</ins> 
 
 ![MS1 TIC Outlier Plot](https://github.com/vegesnam/QCeltis/assets/87665957/b73575cd-c6da-48cc-9444-8397b7a681c4)
 
 When outliers are identified, a scatter plot of the TIC values is produced, with the outlier highlighted in yellow. Outliers/Failed Samples found using this metric indicate issues with with data acquisition and LC-MS instrument performance such as improper autosampler sample pickup. 
-
+ 
 <ins>TIC CV% Across Groups Plot:</ins> 
 
 ![MS1 TIC CV% Plot](https://github.com/vegesnam/QCeltis/assets/87665957/6447f8ed-c446-4772-8693-333eef06d746)
 
 When a grouping file is provided, TIC CV% is calculated across samples within each provided group and the 'TIC CV Threshold' is applied. If any group isn't within the threshold, the group is labelled as a 'FAIL' and this indicates an inconsistent TIC pattern within the samples of the group. 
 
 #### Spectral Ratio
@@ -348,9 +351,7 @@
 ## Cite
 
 ## Support
 
 If you encounter any bugs or issues, please help us improve QCeltis by creating a new issue at: https://github.com/csmc-vaneykjlab/QCeltis/issues. For any other queries, email us at GroupHeartBioinformaticsSupport@cshs.org.
 
 ## release notes
-
-
```

