# Comparing `tmp/ecopipeline-0.2.7.tar.gz` & `tmp/ecopipeline-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.7.tar", last modified: Wed Apr 24 22:27:53 2024, max compression
+gzip compressed data, was "ecopipeline-0.2.8.tar", last modified: Mon Apr 29 18:43:16 2024, max compression
```

## Comparing `ecopipeline-0.2.7.tar` & `ecopipeline-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.049349 ecopipeline-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.049349 ecopipeline-0.2.8/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32173 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30170 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.7/PKG-INFO` & `ecopipeline-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.7
+Version: 0.2.8
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.7/README.md` & `ecopipeline-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/setup.cfg` & `ecopipeline-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.7
+version = 0.2.8
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.7/src/ecopipeline/extract/extract.py` & `ecopipeline-0.2.8/src/ecopipeline/extract/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -329,14 +329,105 @@
      #group and sort index
      df = df.groupby(df.index).mean()
      
      df.sort_index(inplace = True)
 
      return df
 
+def small_planet_control_to_df(config: ConfigManager, csv_filenames: List[str], site: str = "", system: str = "") -> pd.DataFrame:
+    """
+    Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for small planet control data.
+    This data will have variable names equal variable_name column is Variable_Names.csv so you will not need to use the rename_sensors function
+    afterwards.
+
+    Parameters
+    ---------- 
+    config : ecopipeline.ConfigManager
+        The ConfigManager object that holds configuration data for the pipeline. Among other things, this object will point to a file 
+        called Varriable_Names.csv in the input folder of the pipeline (e.g. "full/path/to/pipeline/input/Variable_Names.csv")
+        The csv this points to should have at least 2 columns called "variable_alias" (the raw name to be changed from) and "variable_name"
+        (the name to be changed to). All columns without a cooresponding variable_name will be dropped from the dataframe.
+    csv_filenames : List[str]
+        List of filenames 
+    site: str
+        If the pipeline is processing data for a particular site with a dataframe that contains data from multiple sites that 
+        need to be prossessed seperatly, fill in this optional varriable to drop data from all other sites in the returned dataframe. 
+        Appropriate varriables in your Variable_Names.csv must have a matching substring to this varriable in a column called "site".
+    system: str
+        If the pipeline is processing data for a particular system with a dataframe that contains data from multiple systems that 
+        need to be prossessed seperatly, fill in this optional varriable to drop data from all other systems in the returned dataframe. 
+        Appropriate varriables in your Variable_Names.csv must have a matching string to this varriable in a column called "system"
+    
+    Returns
+    ------- 
+    pd.DataFrame: 
+        Pandas Dataframe containing data from all files
+    """
+    variable_names_path = config.get_var_names_path()
+    try:
+        variable_data = pd.read_csv(variable_names_path)
+    except FileNotFoundError:
+        raise Exception("Variable names file Not Found: "+ variable_names_path)
+    
+    if (site != ""):
+        variable_data = variable_data.loc[variable_data['site'] == site]
+    if (system != ""):
+        variable_data = variable_data.loc[variable_data['system'].str.contains(system, na=False)]
+
+    variable_data = variable_data.loc[:, ['variable_alias', 'variable_name']]
+    variable_data.dropna(axis=0, inplace=True)
+    variable_alias = list(variable_data["variable_alias"])
+    variable_true = list(variable_data["variable_name"])
+    variable_alias_true_dict = dict(zip(variable_alias, variable_true))
+    
+    temp_dfs = []
+    for file in csv_filenames:
+        # each file contains a single variable in this format
+        try:
+            data = pd.read_csv(file)
+        except FileNotFoundError:
+            print("File Not Found: ", file)
+            return
+        except Exception as e:
+            print(f"Error reading {file}: {e}")
+            continue
+        
+        if len(data) != 0:
+            #prepend modbus prefix MOD_RTU_Nesbit_BTU_17_.Building_DHW_Energy_Total.1713078000
+            prefix = file.split('.')[0].split("/")[-1]
+
+            data['time_pt'] = pd.to_datetime(data['DateEpoch(secs)'], unit='s',  utc=True)
+            data['time_pt'] = data['time_pt'].dt.tz_convert('US/Pacific').dt.tz_localize(None)
+            data.set_index('time_pt', inplace = True)
+            data.drop(columns = 'DateEpoch(secs)', inplace = True)
+            data = data.rename(columns={col: f"{prefix}{col}".replace(" ","_").replace("*", "_") for col in data.columns})
+            data.rename(columns=variable_alias_true_dict, inplace=True)
+            # Because there was a name change of varriables in the middle of the data, we rename our sensors here before joining them
+            # =======================================================================================================================
+            # drop columns that do not have a corresponding true name
+            data.drop(columns=[col for col in data if col in variable_alias], inplace=True)
+            # drop columns that are not documented in variable names csv file at all
+            data.drop(columns=[col for col in data if col not in variable_true], inplace=True)
+            #drop null columns
+            data = data.dropna(how='all')
+            # =======================================================================================================================
+            temp_dfs.append(data)
+
+    df = pd.concat(temp_dfs, ignore_index=False)
+    
+    #note sure if we should be rounding down but best I can do atm
+    df.index = df.index.floor('T')
+
+    #group and sort index
+    df = df.groupby(df.index).mean()
+    
+    df.sort_index(inplace = True)
+
+    return df
+
 def fm_api_to_df(config: ConfigManager, startTime: datetime = None, endTime: datetime = None) -> pd.DataFrame:
     """
     Function connects to the field manager api to pull data and returns a dataframe.
 
     Parameters
     ----------  
     config : ecopipeline.ConfigManager
```

### Comparing `ecopipeline-0.2.7/src/ecopipeline/load/load.py` & `ecopipeline-0.2.8/src/ecopipeline/load/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.2.8/src/ecopipeline/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.2.8/src/ecopipeline/transform/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.2.8/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline/transform/transform.py` & `ecopipeline-0.2.8/src/ecopipeline/transform/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     ---------- 
     original_df: pd.DataFrame
         A dataframe that contains data labeled by the raw varriable names to be renamed.
     config : ecopipeline.ConfigManager
         The ConfigManager object that holds configuration data for the pipeline. Among other things, this object will point to a file 
         called Varriable_Names.csv in the input folder of the pipeline (e.g. "full/path/to/pipeline/input/Variable_Names.csv")
         The csv this points to should have at least 2 columns called "variable_alias" (the raw name to be changed from) and "variable_name"
-        (the name to be changed to). All columns without a cooresponding variable_name will be dropped from the datframe.
+        (the name to be changed to). All columns without a cooresponding variable_name will be dropped from the dataframe.
     site: str
         If the pipeline is processing data for a particular site with a dataframe that contains data from multiple sites that 
         need to be prossessed seperatly, fill in this optional varriable to drop data from all other sites in the returned dataframe. 
         Appropriate varriables in your Variable_Names.csv must have a matching substring to this varriable in a column called "site".
     system: str
         If the pipeline is processing data for a particular system with a dataframe that contains data from multiple systems that 
         need to be prossessed seperatly, fill in this optional varriable to drop data from all other systems in the returned dataframe.
```

### Comparing `ecopipeline-0.2.7/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.2.8/src/ecopipeline/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.2.8/src/ecopipeline/utils/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.7/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.2.8/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.7
+Version: 0.2.8
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.7/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.2.8/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

