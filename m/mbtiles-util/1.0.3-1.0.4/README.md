# Comparing `tmp/mbtiles_util-1.0.3.tar.gz` & `tmp/mbtiles_util-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbtiles_util-1.0.3.tar", last modified: Wed Apr 24 08:50:11 2024, max compression
+gzip compressed data, was "mbtiles_util-1.0.4.tar", last modified: Tue Apr 30 11:18:38 2024, max compression
```

## Comparing `mbtiles_util-1.0.3.tar` & `mbtiles_util-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:50:11.835231 mbtiles_util-1.0.3/
--rw-rw-rw-   0        0        0    11524 2024-04-22 09:15:57.000000 mbtiles_util-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1122 2024-04-24 08:50:11.834224 mbtiles_util-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-04-23 07:42:20.000000 mbtiles_util-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:50:11.787087 mbtiles_util-1.0.3/mbtiles_util/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:34:15.000000 mbtiles_util-1.0.3/mbtiles_util/__init__.py
--rw-rw-rw-   0        0        0     2963 2024-04-23 07:34:27.000000 mbtiles_util-1.0.3/mbtiles_util/mbtiles2folder.py
--rw-rw-rw-   0        0        0     3899 2024-04-24 08:48:50.000000 mbtiles_util-1.0.3/mbtiles_util/mbtiles2s3.py
--rw-rw-rw-   0        0        0     4389 2024-04-23 03:19:55.000000 mbtiles_util-1.0.3/mbtiles_util/mbtilesinfo.py
--rw-rw-rw-   0        0        0     3755 2024-04-24 04:27:18.000000 mbtiles_util-1.0.3/mbtiles_util/osm2mbtiles.py
--rw-rw-rw-   0        0        0     2097 2024-04-24 08:49:24.000000 mbtiles_util-1.0.3/mbtiles_util/pbfinfo.py
--rw-rw-rw-   0        0        0      668 2024-04-22 09:14:25.000000 mbtiles_util-1.0.3/mbtiles_util/tileserve.py
--rw-rw-rw-   0        0        0    15360 2024-04-22 12:20:34.000000 mbtiles_util-1.0.3/mbtiles_util/util.py
--rw-rw-rw-   0        0        0      710 2024-04-24 04:27:43.000000 mbtiles_util-1.0.3/mbtiles_util/versatiles.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:50:11.833243 mbtiles_util-1.0.3/mbtiles_util.egg-info/
--rw-rw-rw-   0        0        0     1122 2024-04-24 08:50:11.000000 mbtiles_util-1.0.3/mbtiles_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-24 08:50:11.000000 mbtiles_util-1.0.3/mbtiles_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:50:11.000000 mbtiles_util-1.0.3/mbtiles_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2024-04-24 08:50:11.000000 mbtiles_util-1.0.3/mbtiles_util.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-04-24 08:50:11.000000 mbtiles_util-1.0.3/mbtiles_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 08:50:11.836232 mbtiles_util-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1014 2024-04-24 08:49:14.000000 mbtiles_util-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:18:38.793306 mbtiles_util-1.0.4/
+-rw-rw-rw-   0        0        0    11524 2024-04-22 09:15:57.000000 mbtiles_util-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1218 2024-04-30 11:18:38.792090 mbtiles_util-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-04-30 11:15:55.000000 mbtiles_util-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:18:38.756891 mbtiles_util-1.0.4/mbtiles_util/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:34:15.000000 mbtiles_util-1.0.4/mbtiles_util/__init__.py
+-rw-rw-rw-   0        0        0     1945 2024-04-30 10:11:53.000000 mbtiles_util-1.0.4/mbtiles_util/folder2s3.py
+-rw-rw-rw-   0        0        0     3636 2024-04-30 11:08:08.000000 mbtiles_util-1.0.4/mbtiles_util/mbtiles2folder.py
+-rw-rw-rw-   0        0        0     4276 2024-04-30 09:47:08.000000 mbtiles_util-1.0.4/mbtiles_util/mbtiles2s3.py
+-rw-rw-rw-   0        0        0     4296 2024-04-25 04:04:06.000000 mbtiles_util-1.0.4/mbtiles_util/mbtilesinfo.py
+-rw-rw-rw-   0        0        0     2219 2024-04-26 04:03:39.000000 mbtiles_util-1.0.4/mbtiles_util/osm2geojson.py
+-rw-rw-rw-   0        0        0     3755 2024-04-24 04:27:18.000000 mbtiles_util-1.0.4/mbtiles_util/osm2mbtiles.py
+-rw-rw-rw-   0        0        0     5066 2024-04-26 07:27:17.000000 mbtiles_util-1.0.4/mbtiles_util/osm2streets.py
+-rw-rw-rw-   0        0        0      668 2024-04-22 09:14:25.000000 mbtiles_util-1.0.4/mbtiles_util/tileserve.py
+-rw-rw-rw-   0        0        0     1837 2024-04-30 02:06:41.000000 mbtiles_util-1.0.4/mbtiles_util/tms2xyz.py
+-rw-rw-rw-   0        0        0     1857 2024-04-30 02:58:45.000000 mbtiles_util-1.0.4/mbtiles_util/tms2xyz_raster.py
+-rw-rw-rw-   0        0        0    15360 2024-04-22 12:20:34.000000 mbtiles_util-1.0.4/mbtiles_util/util.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:18:38.791091 mbtiles_util-1.0.4/mbtiles_util.egg-info/
+-rw-rw-rw-   0        0        0     1218 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 11:18:38.000000 mbtiles_util-1.0.4/mbtiles_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 11:18:38.793306 mbtiles_util-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2024-04-30 11:17:22.000000 mbtiles_util-1.0.4/setup.py
```

### Comparing `mbtiles_util-1.0.3/LICENSE` & `mbtiles_util-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mbtiles_util-1.0.3/mbtiles_util/mbtiles2folder.py` & `mbtiles_util-1.0.4/mbtiles_util/mbtiles2folder.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     return
   os.makedirs(d)
 
 def set_dir(d):
   safe_makedir(d)
   os.chdir(d)
 
+def flip_y(zoom, y, tms=0):
+    if tms==0:
+      return y 
+    else:
+      return (2**zoom-1) - y
+
 def extract_metadata(cursor):
   """Extract metadata from MBTiles file."""
   cursor.execute("SELECT name, value FROM metadata")
   metadata_rows = cursor.fetchall()
   metadata = {}
   for name, value in metadata_rows:
       metadata[name] = value
@@ -43,55 +49,66 @@
   return ''
 
 def count_total_tiles(cursor):
   """Count total number of tiles."""
   cursor.execute('SELECT COUNT(*) FROM tiles')
   return cursor.fetchone()[0]
 
-def convert_mbtiles_to_folder(input_filename, output_folder):
+def convert_mbtiles_to_folder(input_filename, output_folder, tms=0):
   """Convert MBTiles file to folder."""
   os.makedirs(output_folder)
   connection = sqlite3.connect(input_filename)
   cursor = connection.cursor()  
 
   
   tile_format = determine_tile_format(cursor)
   total_tiles = count_total_tiles(cursor)
   metadata = extract_metadata(cursor)
   write_metadata_to_json(metadata, output_folder)
  
   os.chdir(output_folder)
   cursor.execute('SELECT zoom_level, tile_column, tile_row, tile_data FROM tiles order by zoom_level')
-  with tqdm(total=total_tiles, desc="Progress", unit="tile") as pbar:      
+  with tqdm(total=total_tiles, desc="Converting mbtiles to folder", unit="tile") as pbar:      
     for row in cursor:
-      set_dir(str(row[0]))
-      set_dir(str(row[1]))
-      output_file = open(str(row[2]) + tile_format, 'wb')
-      output_file.write(row[3])
+      z = row[0]
+      x = row[1]
+      tile_data = row[3]
+      set_dir(str(z))
+      set_dir(str(x))
+      y = row[2]
+      if tms ==1:
+        y = flip_y(row[0], y, tms)
+      output_file = open(str(y) + tile_format, 'wb')
+      output_file.write(tile_data)
       output_file.close()
       os.chdir('..')
       os.chdir('..')
       pbar.update(1)
 
   print('Converting mbtiles to folder done!')
   connection.close()
 
 def main():
   parser = argparse.ArgumentParser(description='Convert MBTiles file to folder')
   parser.add_argument('-i', help='Input MBTiles file name')
-  parser.add_argument('-o', help='Output folder name')
+  parser.add_argument('-o', help='Output folder name (optional)', default=None)
+  parser.add_argument('-tms', help='Use TMS (flip y) format: 1 or 0', type=int, default=0)
+
   args = parser.parse_args()
 
   if not args.i:
     print('Please provide the mbtiles input filename.')
     exit()
   if not os.path.exists(args.i):
     print('MBTiles file does not exist!. Please recheck and input a correct file path.')
     exit()
+
   if not args.o:
-    print('Please provide the output folder name.')
-    exit()
-  
-  convert_mbtiles_to_folder(args.i, args.o)
+    output_folder = os.path.splitext(os.path.basename(args.i))[0]  # Get file name without extension
+    output_folder_path = os.path.join(os.path.dirname(args.i), output_folder)
+    args.o = output_folder_path
+    print(f'Output folder not provided. Creating folder with the same name as the input file in the same directory: {output_folder_path}')
+
+  convert_mbtiles_to_folder(args.i, args.o, args.tms)
 
 if __name__ == "__main__":
     main()
```

### Comparing `mbtiles_util-1.0.3/mbtiles_util/mbtiles2s3.py` & `mbtiles_util-1.0.4/mbtiles_util/mbtiles2s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   return ''
 
 def count_total_tiles(cursor):
   """Count total number of tiles."""
   cursor.execute('SELECT COUNT(*) FROM tiles')
   return cursor.fetchone()[0]
 
-def convert_mbtiles_to_folder(input_filename, output_folder):
+def mbtiles2folder(input_filename, output_folder):
   """Convert MBTiles file to folder."""
   os.makedirs(output_folder)
   connection = sqlite3.connect(input_filename)
   cursor = connection.cursor()  
   tile_format = determine_tile_format(cursor)
   total_tiles = count_total_tiles(cursor)
   metadata = extract_metadata(cursor)
@@ -70,49 +70,53 @@
       output_file.close()
       os.chdir('..')
       os.chdir('..')
       pbar.update(1)
   print('Converting mbtiles to folder done!')
   connection.close()
 
-def folder_to_s3(output_folder,bucket_name, s3_prefix=''):
-  # s3_client = boto3.client('s3')
-  # with tqdm(total=5000, desc="Progress", unit="tile") as pbar:
-  #   for root, dirs, files in os.walk(output_folder):
-  #     for file in files:
-  #       local_file_path = os.path.join(root, file)
-  #       s3_key = os.path.relpath(local_file_path, output_folder)
-  #       s3_key = os.path.join(s3_prefix, s3_key).replace('\\', '/')  # for Windows compatibility
-  #       s3_client.upload_file(local_file_path, bucket_name, s3_key)
-  #   pbar.update(1)
-  s3 = boto3.client(
-    's3',
-    aws_access_key_id='aws_access_key_id',
-    aws_secret_access_key='aws_secret_access_key'
+def folder_to_s3(input_filename, output_folder, bucket_name, s3_prefix='', region=None, aws_access_key_id=None, aws_secret_access_key=None):
+  mbtiles2folder(input_filename, output_folder);
+  session = boto3.Session(
+      region_name=region,
+      aws_access_key_id=aws_access_key_id,
+      aws_secret_access_key=aws_secret_access_key,
   )
-  file_name = '0.png'
-  s3.upload_file(file_name, bucket_name, s3_prefix + file_name)
+  s3 = session.client('s3')
+  total_files = sum(len(files) for _, _, files in os.walk(output_folder))
+  with tqdm(total=total_files, desc="Uploading", unit="file") as pbar:
+    for root, dirs, files in os.walk(output_folder):
+      for file in files:
+          local_file_path = os.path.join(root, file)
+          s3_key = os.path.relpath(local_file_path, output_folder)
+          s3_key = os.path.join(s3_prefix, s3_key).replace('\\', '/')  # for Windows compatibility
+          s3.upload_file(local_file_path, bucket_name, s3_key)
+          pbar.update(1)
   print('Uploading folder to S3 done!')
 
 def main():
-  parser = argparse.ArgumentParser(description='Convert MBTiles file to folder')
-  parser.add_argument('-i', help='Input MBTiles file name')
-  parser.add_argument('-o', help='Output folder name')
+  parser = argparse.ArgumentParser(description='Upload a folder to S3')
+  parser.add_argument('-i', help='Input folder name', required=True)
+  parser.add_argument('-b', help='S3 bucket name', required=True)
+  parser.add_argument('-p', help='S3 prefix (optional)', default='')
+  parser.add_argument('-r', help='AWS region (optional)', default='us-east-1')
+  args = parser.parse_args()
+
   args = parser.parse_args()
 
   if not args.i:
-    print('Please provide the mbtiles input filename.')
-    exit()
+      print('Please provide the input folder name.')
+      exit()
   if not os.path.exists(args.i):
-    print('MBTiles file does not exist!. Please recheck and input a correct file path.')
-    exit()
-  if not args.o:
-    print('Please provide the output folder name.')
-    exit()
-  
-  # convert_mbtiles_to_folder(args.i, args.o)
-  bucket_name='bucket_name'
-  s3_prefix= 's3_prefix'
-  folder_to_s3(args.o,bucket_name,s3_prefix)
+      print('Input folder does not exist!. Please recheck and input a correct folder path.')
+      exit()
+  if not args.b:
+      print('Please provide the S3 bucket name.')
+      exit()
+
+  aws_access_key_id = input('Enter AWS Access Key ID: ')
+  aws_secret_access_key = input('Enter AWS Secret Access Key: ')
+  folder_to_s3(args.i, args.b, args.p, aws_access_key_id, aws_secret_access_key)
 
 if __name__ == "__main__":
-    main()
+  main()
+
```

### Comparing `mbtiles_util-1.0.3/mbtiles_util/mbtilesinfo.py` & `mbtiles_util-1.0.4/mbtiles_util/mbtilesinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,30 +67,30 @@
     return num_tiles
 
 # list all vector layers
 def read_vector_layers(input_filename):    
     connection = sqlite3.connect(input_filename)
     cursor = connection.cursor()
     cursor.execute("SELECT name, value FROM metadata where name = 'json'")
-    json_content = cursor.fetchone()[1]
-    layers_json = json.loads(json_content)
-    # print (layers_json)
-    if "vector_layers" in layers_json:
-      vector_layers = layers_json["vector_layers"]
-      print("Vector layers:")
-      for index, layer in enumerate(vector_layers):
-          row_index = index + 1
-          layer_id  = layer["id"]
-          print(f"{row_index}: {layer_id}")
-          # print("  Description:", layer.get("description", "N/A"))
-          # print("  Min zoom:", layer.get("minzoom", "N/A"))
-          # print("  Max zoom:", layer.get("maxzoom", "N/A"))
-          # print("  Fields:", layer.get("fields", "N/A"))
+    row = cursor.fetchone()
+    if row is not None:
+        json_content = row[1]
+        layers_json = json.loads(json_content)
+        if "vector_layers" in layers_json:
+            vector_layers = layers_json["vector_layers"]
+            print("Vector layers:")
+            for index, layer in enumerate(vector_layers):
+                row_index = index + 1
+                layer_id = layer["id"]
+                print(f"{row_index}: {layer_id}")
+                # Additional information printing here if needed
+        else:
+            print("No 'vector_layers' found in metadata.")
     else:
-      print("No 'vector_layers' found in metadata.")
+        return
     # Write metadata to JSON content
     # metadata_json_path = os.path.join(os.path.dirname(input_filename), "tiles.json")
     # with open(metadata_json_path, "w") as metadata_file:
     #     json.dump(layers_json, metadata_file, indent=4)
     # print ("Writing tiles.json done!")
 
 def main():
```

### Comparing `mbtiles_util-1.0.3/mbtiles_util/osm2mbtiles.py` & `mbtiles_util-1.0.4/mbtiles_util/osm2mbtiles.py`

 * *Files identical despite different names*

### Comparing `mbtiles_util-1.0.3/mbtiles_util/tileserve.py` & `mbtiles_util-1.0.4/mbtiles_util/tileserve.py`

 * *Files identical despite different names*

### Comparing `mbtiles_util-1.0.3/mbtiles_util/util.py` & `mbtiles_util-1.0.4/mbtiles_util/util.py`

 * *Files identical despite different names*

