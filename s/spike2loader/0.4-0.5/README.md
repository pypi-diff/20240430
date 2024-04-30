# Comparing `tmp/spike2loader-0.4.tar.gz` & `tmp/spike2loader-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2loader-0.4.tar", last modified: Tue Apr 30 12:48:52 2024, max compression
+gzip compressed data, was "spike2loader-0.5.tar", last modified: Tue Apr 30 13:04:15 2024, max compression
```

## Comparing `spike2loader-0.4.tar` & `spike2loader-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 12:48:52.232141 spike2loader-0.4/
--rw-rw-r--   0 julienb   (1000) julienb   (1000)     1065 2024-04-29 11:33:59.000000 spike2loader-0.4/LICENSE.txt
--rw-r--r--   0 julienb   (1000) julienb   (1000)      445 2024-04-30 12:48:52.232141 spike2loader-0.4/PKG-INFO
--rw-rw-r--   0 julienb   (1000) julienb   (1000)      149 2024-04-29 16:22:43.000000 spike2loader-0.4/README.md
--rw-rw-r--   0 julienb   (1000) julienb   (1000)       38 2024-04-30 12:48:52.232141 spike2loader-0.4/setup.cfg
--rw-rw-r--   0 julienb   (1000) julienb   (1000)      709 2024-04-30 12:48:42.000000 spike2loader-0.4/setup.py
-drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 12:48:52.232141 spike2loader-0.4/src/
-drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 12:48:52.232141 spike2loader-0.4/src/spike2loader/
--rw-rw-r--   0 julienb   (1000) julienb   (1000)       46 2024-04-29 11:44:18.000000 spike2loader-0.4/src/spike2loader/__init__.py
--rw-rw-r--   0 julienb   (1000) julienb   (1000)     4607 2024-04-30 12:45:50.000000 spike2loader-0.4/src/spike2loader/spike2loader.py
-drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 12:48:52.232141 spike2loader-0.4/src/spike2loader.egg-info/
--rw-r--r--   0 julienb   (1000) julienb   (1000)      445 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/PKG-INFO
--rw-rw-r--   0 julienb   (1000) julienb   (1000)      334 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/SOURCES.txt
--rw-rw-r--   0 julienb   (1000) julienb   (1000)        1 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/dependency_links.txt
--rw-rw-r--   0 julienb   (1000) julienb   (1000)       51 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/entry_points.txt
--rw-rw-r--   0 julienb   (1000) julienb   (1000)       34 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/requires.txt
--rw-rw-r--   0 julienb   (1000) julienb   (1000)       13 2024-04-30 12:48:52.000000 spike2loader-0.4/src/spike2loader.egg-info/top_level.txt
+drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 13:04:15.831450 spike2loader-0.5/
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)     1065 2024-04-29 11:33:59.000000 spike2loader-0.5/LICENSE.txt
+-rw-r--r--   0 julienb   (1000) julienb   (1000)     1748 2024-04-30 13:04:15.831450 spike2loader-0.5/PKG-INFO
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)     1267 2024-04-30 13:04:03.000000 spike2loader-0.5/README.md
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)       38 2024-04-30 13:04:15.831450 spike2loader-0.5/setup.cfg
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)      832 2024-04-30 13:04:13.000000 spike2loader-0.5/setup.py
+drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 13:04:15.831450 spike2loader-0.5/src/
+drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 13:04:15.831450 spike2loader-0.5/src/spike2loader/
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)       46 2024-04-29 11:44:18.000000 spike2loader-0.5/src/spike2loader/__init__.py
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)     4620 2024-04-30 12:54:29.000000 spike2loader-0.5/src/spike2loader/spike2loader.py
+drwxrwxr-x   0 julienb   (1000) julienb   (1000)        0 2024-04-30 13:04:15.831450 spike2loader-0.5/src/spike2loader.egg-info/
+-rw-r--r--   0 julienb   (1000) julienb   (1000)     1748 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/PKG-INFO
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)      334 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)        1 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)       57 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/entry_points.txt
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)       34 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/requires.txt
+-rw-rw-r--   0 julienb   (1000) julienb   (1000)       13 2024-04-30 13:04:15.000000 spike2loader-0.5/src/spike2loader.egg-info/top_level.txt
```

### Comparing `spike2loader-0.4/LICENSE.txt` & `spike2loader-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spike2loader-0.4/src/spike2loader/spike2loader.py` & `spike2loader-0.5/src/spike2loader/spike2loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger(__name__)
 
 events_channel_types = [sp.DataType.EventFall, sp.DataType.EventRise, sp.DataType.EventBoth]
 continuous_channel_types =  [sp.DataType.Adc]
 
 
-def to_pandas_dataframes(
+def as_python_data(
         file: Union[str, Path], 
         channels: AbstractSet[Union[int, str]] =[...], 
         channel_types: AbstractSet[Union[str, sp.DataType]] =[...], 
         progress:bool=True
 ) -> Tuple[pd.DataFrame, Mapping[str, np.ndarray]]:
     
     path = Path(file)
@@ -26,15 +26,15 @@
     channels = set(all_channels[c] if isinstance(c, str) else c for c in channels)
     if ... in channels:
         channels = set(all_channels.values()) - channels
 
     time_base = MyFile.GetTimeBase()
     df_data = []
     channel_data = {}
-    for i in tqdm.tqdm(channels, desc="Loading data"):
+    for i in tqdm.tqdm(channels, desc="Loading data", disable=not progress):
         name=MyFile.GetChannelTitle(i)
         type=MyFile.ChannelType(i)
         unit=MyFile.GetChannelUnits(i)
         size=MyFile.ChannelBytes(i)
         item_size=MyFile.ItemSize(i)
         scale=MyFile.GetChannelScale(i)/6553.6
         offset=MyFile.GetChannelOffset(i)
@@ -71,15 +71,15 @@
             raise Exception(f"Some data will be missing in channel {name}")
         
         df_data.append(dict(name=name, data_kind=data_kind, smrx_channel_num=i, smrx_type=str(type), unit=str(unit), n_data=n_data, fs=fs))
         channel_data[name]=data
     df = pd.DataFrame(df_data).set_index("name")
     return df, channel_data
 
-def smrx2tsv():
+def smrx2python():
     import beautifullogger, argparse, string
     parser = argparse.ArgumentParser(description='Converts smrx files into a tsv file and a set of numpy files')
     # parser.add_argument('verbose', metavar='v', type=str, default="Info",
     #                 help='change logging level possibilities are [Debug, Info, Warning, Error]')
     parser.add_argument('-i', type=str, required=True,
                     help='input smrx file to convert')
     parser.add_argument('-o', type=str, default="{smrx_path}.tsv", required=False,
@@ -91,15 +91,15 @@
     keys = dict(smrx_path=input.parent/input.stem)
     ouputtsv = Path(string.Formatter().format(args.o, **keys))
     ouputnpy = Path(string.Formatter().format(args.onp, **keys))
     beautifullogger.setup(displayLevel=logging.INFO)
 
 
     logger.info("Starting")
-    df, d = to_pandas_dataframes(input)
+    df, d = as_python_data(input)
     logger.info(f"Dataframe is\n{df}")
     logger.info(f"Saving dataframe")
     df.to_csv(ouputtsv, index=True, sep="\t")
     ouputnpy.mkdir(parents=True, exist_ok=True)
     logger.info(f"Saving npys")
     for k,v in tqdm.tqdm(d.items(), desc="Saving npys"):
         np.save(ouputnpy / f"{k}.npy", v)
```

