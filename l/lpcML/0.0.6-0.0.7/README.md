# Comparing `tmp/lpcML-0.0.6.tar.gz` & `tmp/lpcML-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpcML-0.0.6.tar", last modified: Tue Apr 30 10:05:28 2024, max compression
+gzip compressed data, was "lpcML-0.0.7.tar", last modified: Tue Apr 30 10:52:57 2024, max compression
```

## Comparing `lpcML-0.0.6.tar` & `lpcML-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:05:28.765441 lpcML-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 10:05:16.000000 lpcML-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 10:05:28.765441 lpcML-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-30 10:05:16.000000 lpcML-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:05:28.765441 lpcML-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 10:05:16.000000 lpcML-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:05:28.761441 lpcML-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:05:28.765441 lpcML-0.0.6/src/lpcML/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 10:05:16.000000 lpcML-0.0.6/src/lpcML/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6581 2024-04-30 10:05:16.000000 lpcML-0.0.6/src/lpcML/data_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 10:05:16.000000 lpcML-0.0.6/src/lpcML/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4175 2024-04-30 10:05:16.000000 lpcML-0.0.6/src/lpcML/model_fitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:05:28.765441 lpcML-0.0.6/src/lpcML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 10:05:28.000000 lpcML-0.0.6/src/lpcML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 10:05:28.000000 lpcML-0.0.6/src/lpcML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:05:28.000000 lpcML-0.0.6/src/lpcML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 10:05:28.000000 lpcML-0.0.6/src/lpcML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 10:05:28.000000 lpcML-0.0.6/src/lpcML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:52:57.828336 lpcML-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 10:52:45.000000 lpcML-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-30 10:52:57.828336 lpcML-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-30 10:52:45.000000 lpcML-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:52:57.828336 lpcML-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 10:52:45.000000 lpcML-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:52:57.824336 lpcML-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:52:57.828336 lpcML-0.0.7/src/lpcML/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 10:52:45.000000 lpcML-0.0.7/src/lpcML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6817 2024-04-30 10:52:45.000000 lpcML-0.0.7/src/lpcML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 10:52:45.000000 lpcML-0.0.7/src/lpcML/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4175 2024-04-30 10:52:45.000000 lpcML-0.0.7/src/lpcML/model_fitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:52:57.828336 lpcML-0.0.7/src/lpcML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-30 10:52:57.000000 lpcML-0.0.7/src/lpcML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 10:52:57.000000 lpcML-0.0.7/src/lpcML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:52:57.000000 lpcML-0.0.7/src/lpcML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 10:52:57.000000 lpcML-0.0.7/src/lpcML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 10:52:57.000000 lpcML-0.0.7/src/lpcML.egg-info/top_level.txt
```

### Comparing `lpcML-0.0.6/LICENSE` & `lpcML-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.6/PKG-INFO` & `lpcML-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.6
+Version: 0.0.7
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -15,26 +15,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LPC ML
 
 LPC ML is a tool developed in the CiTIUS, USC by the MODEV group for training a multi-layer perceptron (MLP) neural network to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells.
 
-![img](images/lpc.PNG)
+<img src="images/lpc.png" width="500">
 
-**Fig.1:** LPC SCHEME
-<!-- Data used to feed the neural networks is shared in the following Zenodo Repository [https://doi.org/10.5281/zenodo.11032095](https://doi.org/10.5281/zenodo.11032095). -->
+**Fig.1:** GaAs-based horizontal laser power converter
+
+Data used to feed the neural networks is shared in [data/hLPC_GaAS_5W_ml.csv](data/hLPC_GaAS_5W_ml.csv).
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
 
-**Instalation of MLFoMpy via pip3**
+**Installation of lpcML via pip3**
 
 Install the tool using pip3:
 
     pip3 install lpcML
 
 and check the library is installed by importing it from a **python3 terminal**:
```

### Comparing `lpcML-0.0.6/setup.py` & `lpcML-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='lpcML',
-    version='0.0.6',
+    version='0.0.7',
     description='LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML',
     setup_requires=['setuptools'],
```

### Comparing `lpcML-0.0.6/src/lpcML/data_processing.py` & `lpcML-0.0.7/src/lpcML/data_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 
 def split_data(X, Y, test_split = 0.2, verbosity=False):
     '''Split data into train, validation and test subsets
     ---------
     Input:
     ------
     X: torch.tensor
-        Scaled input tensor
+        Input tensor
     Y: torch.tensor
-        Scaled output tensor
+        Output tensor
     test_split: float
         Percentage of subsets distribution, 20% test by default
     
     Output:
     -------
     X_train, Y_train: torch.tensor
         Input, Output train subsets
@@ -89,18 +89,22 @@
     data: pd.Dataframe
         hLPC optimization data
     scaler: str
         Choose the scaler to apply to the data, two options: StandardScaler 'standard' (default) and MinMaxScaler 'minmax'
 
     Output:
     ------
-    X_list: torch.tensor
-        Input tensor
+    X_train: torch.tensor
+        Input train tensor
+    X_val: torch.tensor
+        Input validation tensor
+    X_test: torch.tensor
+        Input test tensor
     scaler_inputs: object
-        Scaler object for inputs
+        Scaler object for inputs, standard by default
     '''
     if scaler == 'standard':
         scaler_inputs = StandardScaler()
     elif scaler == 'minmax':
         scaler_inputs = MinMaxScaler()
     X_train_scaled = scaler_inputs.fit_transform(X_train)
     X_val_scaled = scaler_inputs.transform(X_val)
@@ -116,18 +120,22 @@
     -----
     data: pd.Dataframe
         hLPC optimization data
     scaler: str
         Choose the scaler to apply to the data, two options: StandardScaler 'standard' (default) and MinMaxScaler 'minmax'
     Output:
     ------
-    Y_list: torch.tensor
+    Y_train: torch.tensor
+        Output tensor
+    Y_val: torch.tensor
+        Output tensor
+    Y_test: torch.tensor
         Output tensor
     scaler_outputs: object
-        Scaler object for outputs
+        Scaler object for outputs, standard by default
     '''
     if scaler == 'standard':
         scaler_output = StandardScaler()
     elif scaler == 'minmax':
         scaler_output = MinMaxScaler()
     Y_train_scaled = scaler_output.fit_transform(Y_train)
     Y_val_scaled = scaler_output.transform(Y_val)
```

### Comparing `lpcML-0.0.6/src/lpcML/model.py` & `lpcML-0.0.7/src/lpcML/model.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.6/src/lpcML/model_fitting.py` & `lpcML-0.0.7/src/lpcML/model_fitting.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.6/src/lpcML.egg-info/PKG-INFO` & `lpcML-0.0.7/src/lpcML.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.6
+Version: 0.0.7
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -15,26 +15,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LPC ML
 
 LPC ML is a tool developed in the CiTIUS, USC by the MODEV group for training a multi-layer perceptron (MLP) neural network to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells.
 
-![img](images/lpc.PNG)
+<img src="images/lpc.png" width="500">
 
-**Fig.1:** LPC SCHEME
-<!-- Data used to feed the neural networks is shared in the following Zenodo Repository [https://doi.org/10.5281/zenodo.11032095](https://doi.org/10.5281/zenodo.11032095). -->
+**Fig.1:** GaAs-based horizontal laser power converter
+
+Data used to feed the neural networks is shared in [data/hLPC_GaAS_5W_ml.csv](data/hLPC_GaAS_5W_ml.csv).
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
 
-**Instalation of MLFoMpy via pip3**
+**Installation of lpcML via pip3**
 
 Install the tool using pip3:
 
     pip3 install lpcML
 
 and check the library is installed by importing it from a **python3 terminal**:
```

