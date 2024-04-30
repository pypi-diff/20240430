# Comparing `tmp/simple-extract-0.3.1.tar.gz` & `tmp/simple_extract-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-extract-0.3.1.tar", last modified: Fri Feb 16 20:58:17 2024, max compression
+gzip compressed data, was "simple_extract-0.3.2.tar", last modified: Tue Apr 30 18:58:39 2024, max compression
```

## Comparing `simple-extract-0.3.1.tar` & `simple_extract-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-16 20:58:17.200433 simple-extract-0.3.1/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1057 2024-01-25 22:41:29.000000 simple-extract-0.3.1/LICENSE
--rw-r--r--   0 berrym    (1000) berrym    (1000)     2450 2024-02-16 20:58:17.200433 simple-extract-0.3.1/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1964 2024-02-16 20:55:32.000000 simple-extract-0.3.1/README.md
--rw-r--r--   0 berrym    (1000) berrym    (1000)      722 2024-02-16 20:58:08.000000 simple-extract-0.3.1/pyproject.toml
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-02-16 20:58:17.200433 simple-extract-0.3.1/setup.cfg
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-01-25 22:41:29.000000 simple-extract-0.3.1/setup.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-16 20:58:17.199433 simple-extract-0.3.1/src/
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-16 20:58:17.199433 simple-extract-0.3.1/src/simple_extract/
--rw-r--r--   0 berrym    (1000) berrym    (1000)       22 2024-02-16 20:54:40.000000 simple-extract-0.3.1/src/simple_extract/__init__.py
--rwxr-xr-x   0 berrym    (1000) berrym    (1000)    15701 2024-02-16 20:39:37.000000 simple-extract-0.3.1/src/simple_extract/simple_extract.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-16 20:58:17.200433 simple-extract-0.3.1/src/simple_extract.egg-info/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     2450 2024-02-16 20:58:17.000000 simple-extract-0.3.1/src/simple_extract.egg-info/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)      322 2024-02-16 20:58:17.000000 simple-extract-0.3.1/src/simple_extract.egg-info/SOURCES.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-02-16 20:58:17.000000 simple-extract-0.3.1/src/simple_extract.egg-info/dependency_links.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       70 2024-02-16 20:58:17.000000 simple-extract-0.3.1/src/simple_extract.egg-info/entry_points.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       15 2024-02-16 20:58:17.000000 simple-extract-0.3.1/src/simple_extract.egg-info/top_level.txt
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-30 18:58:39.948155 simple_extract-0.3.2/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1057 2024-02-29 00:20:52.000000 simple_extract-0.3.2/LICENSE
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     2450 2024-04-30 18:58:39.948155 simple_extract-0.3.2/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1964 2024-02-29 00:20:52.000000 simple_extract-0.3.2/README.md
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      722 2024-04-30 18:56:40.000000 simple_extract-0.3.2/pyproject.toml
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-04-30 18:58:39.948155 simple_extract-0.3.2/setup.cfg
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-02-29 00:20:52.000000 simple_extract-0.3.2/setup.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-30 18:58:39.946155 simple_extract-0.3.2/src/
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-30 18:58:39.947155 simple_extract-0.3.2/src/simple_extract/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       22 2024-04-30 18:56:52.000000 simple_extract-0.3.2/src/simple_extract/__init__.py
+-rwxr-xr-x   0 berrym    (1000) berrym    (1000)    15562 2024-04-30 18:57:55.000000 simple_extract-0.3.2/src/simple_extract/simple_extract.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-30 18:58:39.947155 simple_extract-0.3.2/src/simple_extract.egg-info/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     2450 2024-04-30 18:58:39.000000 simple_extract-0.3.2/src/simple_extract.egg-info/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      322 2024-04-30 18:58:39.000000 simple_extract-0.3.2/src/simple_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-04-30 18:58:39.000000 simple_extract-0.3.2/src/simple_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       70 2024-04-30 18:58:39.000000 simple_extract-0.3.2/src/simple_extract.egg-info/entry_points.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       15 2024-04-30 18:58:39.000000 simple_extract-0.3.2/src/simple_extract.egg-info/top_level.txt
```

### Comparing `simple-extract-0.3.1/LICENSE` & `simple_extract-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-extract-0.3.1/PKG-INFO` & `simple_extract-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-extract
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small command line utility to help extract compressed archives.
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/simple_extract
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simple-extract-0.3.1/README.md` & `simple_extract-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `simple-extract-0.3.1/pyproject.toml` & `simple_extract-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "simple-extract"
-version = "0.3.1"
+version = "0.3.2"
 description = "A small command line utility to help extract compressed archives."
 authors = [
     {name = "Michael Berry", email = "trismegustis@gmail.com"},
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `simple-extract-0.3.1/src/simple_extract/simple_extract.py` & `simple_extract-0.3.2/src/simple_extract/simple_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 import urllib.parse
 import urllib.request
 
 from . import __version__
 
 
 # Enable logging
-logging.basicConfig(
-    level=logging.DEBUG, format="[%(levelname)-8s]  %(message)s"
-)
+logging.basicConfig(level=logging.DEBUG, format="[%(levelname)-8s]  %(message)s")
 
 
 class ArchiveCommand:
     """Object for storing information needed to extract archives."""
 
     def __init__(
         self, extract_cmd="", pipe_cmd="", uses_stdin=False, uses_stdout=False
@@ -90,17 +88,18 @@
 
     @param cmd: external command to check for existence
 
     @return: boolean value True if cmd exists, False otherwise
     """
 
     try:
-        subprocess.Popen(
+        with subprocess.Popen(
             [cmd], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-        )
+        ) as cmd:
+            pass
     except OSError as e:
         if e.errno == errno.ENOENT:
             return False
 
     return True
 
 
@@ -156,54 +155,55 @@
     logging.info("Target: %s", target)
 
     if os.path.exists(target) and no_clobber:
         logging.warning("Target: %s already exists not overwriting...", target)
         return
 
     # Extract archive
-    with open(archive) as infile:
+    with open(archive, encoding="utf8") as infile:
         if not pipe_cmd:
             if uses_stdin and not uses_stdout:
                 try:
                     subprocess.run(extract_cmd, stdin=infile, check=True)
                 except OSError as e:
                     logging.warning(
                         "Errno %d: %s - %s", e.errno, e.strerror, extract_cmd
                     )
-            elif uses_stdin and uses_stdout:
-                with open(target, "w+") as outfile:
+                return
+
+            if uses_stdin and uses_stdout:
+                with open(target, "w+", encoding="utf8") as outfile:
                     try:
                         subprocess.run(
                             extract_cmd,
                             stdin=infile,
                             stdout=outfile,
                             check=True,
                         )
                     except OSError as e:
                         logging.warning(
                             "Errno %d: %s - %s", e.errno, e.strerror, extract_cmd
                         )
                         os.remove(target)
+                    return
             else:
                 try:
                     subprocess.run(extract_cmd, check=True)
                 except OSError as e:
                     logging.warning(
                         "Errno %d: %s - %s", e.errno, e.strerror, extract_cmd
                     )
-        else:
-            with subprocess.Popen(
-                extract_cmd, stdin=infile, stdout=subprocess.PIPE
-            ) as cmd:
-                try:
-                    subprocess.run(pipe_cmd, stdin=cmd.stdout, check=True)
-                except OSError as e:
-                    logging.warning(
-                        "Errno %d: %s - %s", e.errno, e.strerror, extract_cmd
-                    )
+                return
+
+        # Piped command
+        with subprocess.Popen(extract_cmd, stdin=infile, stdout=subprocess.PIPE) as cmd:
+            try:
+                subprocess.run(pipe_cmd, stdin=cmd.stdout, check=True)
+            except OSError as e:
+                logging.warning("Errno %d: %s -> %s", e.errno, e.strerror, extract_cmd)
 
 
 def should_fetch_url(archive_url, local_archive):
     """Check if an archive should be fetched by comparing
     remote and local file sizes.
 
     @param archive_url: url of archive to be downloaded
@@ -219,16 +219,16 @@
     try:
         with urllib.request.urlopen(req) as f:
             if not f.headers["content-length"]:
                 logging.warning(
                     "Error: invalid archive content-length, skipping download"
                 )
                 return False
-            else:
-                remote_size = f.headers["content-length"]
+
+            remote_size = f.headers["content-length"]
     except urllib.error.HTTPError as e:
         logging.warning("Error: The server couldn't fulfil the request")
         logging.warning("Error Code: %d", e.code)
         return False
     except urllib.error.URLError as e:
         logging.warning("Error: failed to reach the server")
         logging.warning("Reason: %s", e.reason)
@@ -244,16 +244,16 @@
     logging.info("Comparing remote and local archives")
     logging.info("remote size: %d, local size: %d", remote_size, local_size)
 
     # compare remote and local sizes, if equal return False
     if int(remote_size) == int(local_size):
         logging.warning("Archive sizes are the same. Skipping download...")
         return False
-    else:
-        logging.info("Archives differ in size, downloading...")
+
+    logging.info("Archives differ in size, downloading...")
 
     return True
 
 
 def fetch_archive(url, silent_download=False, force_download=False):
     """Download an archive for extraction.
 
@@ -290,23 +290,19 @@
     if not force_download:
         logging.info("Checking if archive should be downloaded")
         if not should_fetch_url(url, target):
             return False
 
     logging.info("Fetching archive %s", target)
 
-    with open(target, "w+") as outfile:
+    with open(target, "w+", encoding="utf8") as outfile:
         try:
-            subprocess.run(
-                fetch_cmd, stdin=subprocess.PIPE, stdout=outfile, check=True
-            )
+            subprocess.run(fetch_cmd, stdin=subprocess.PIPE, stdout=outfile, check=True)
         except OSError as e:
-            logging.warning(
-                "Errno %d: %s - %s", e.errno, e.strerror, fetch_cmd
-            )
+            logging.warning("Errno %d: %s - %s", e.errno, e.strerror, fetch_cmd)
             os.remove(target)
             return False
 
     return target
 
 
 def extract_urls(args):
@@ -314,17 +310,15 @@
 
     @param args: list of possible valid urls to download
 
     @return: list of valid urls to download
     """
 
     possibles = [urllib.parse.urlsplit(x) for x in args]
-    unfiltered = [
-        x if x.scheme and x.netloc and x.path else None for x in possibles
-    ]
+    unfiltered = [x if x.scheme and x.netloc and x.path else None for x in possibles]
     processed_urls = list(filter(lambda x: x is not None, unfiltered))
 
     return [x.scheme + "://" + x.netloc + x.path for x in processed_urls]
 
 
 def main():
     """Main function.
@@ -362,45 +356,37 @@
         help="Don't show archive download progress",
         dest="silent_download",
     )
     parser.add_argument("ARCHIVES", nargs="*")
     parsed = parser.parse_args()
 
     start_time = datetime.datetime.now()
-    logging.info("Starting simple-extract @ %s, start_time")
+    logging.info("Starting simple-extract @ %s", start_time)
 
     working_dir = os.getcwd()
-    args = [x for x in parsed.ARCHIVES]
+    args = list(parsed.ARCHIVES)
     glob_files = []
     commands = []
     command_map = {
-        "*.tar.bz2": ArchiveCommand(
-            extract_cmd="tar -xvjf -", uses_stdin=True
-        ),
+        "*.tar.bz2": ArchiveCommand(extract_cmd="tar -xvjf -", uses_stdin=True),
         "*.tbz2": ArchiveCommand(extract_cmd="tar -xvjf -", uses_stdin=True),
         "*.tbz": ArchiveCommand(extract_cmd="tar -xvjf -", uses_stdin=True),
         "*.tar.gz": ArchiveCommand(extract_cmd="tar -xvzf -", uses_stdin=True),
         "*.tgz": ArchiveCommand(extract_cmd="tar -xvzf -", uses_stdin=True),
         "*.tar.xz": ArchiveCommand(extract_cmd="tar -xvJf -", uses_stdin=True),
         "*.txz": ArchiveCommand(extract_cmd="tar -xvJf -", uses_stdin=True),
-        "*.tar.lzma": ArchiveCommand(
-            extract_cmd="tar -xvJf -", uses_stdin=True
-        ),
-        "*.tar.zst": ArchiveCommand(
-            extract_cmd="tar --zstd -xvf -", uses_stdin=True
-        ),
+        "*.tar.lzma": ArchiveCommand(extract_cmd="tar -xvJf -", uses_stdin=True),
+        "*.tar.zst": ArchiveCommand(extract_cmd="tar --zstd -xvf -", uses_stdin=True),
         "*.tar": ArchiveCommand(extract_cmd="tar -xvf -", uses_stdin=True),
         "*.rar": ArchiveCommand(extract_cmd="unrar x"),
         "*.lzh": ArchiveCommand(extract_cmd="lha x"),
         "*.7z": ArchiveCommand(extract_cmd="7z x"),
         "*.zip": ArchiveCommand(extract_cmd="unzip"),
         "*.jar": ArchiveCommand(extract_cmd="unzip"),
-        "*.rpm": ArchiveCommand(
-            extract_cmd="rpm2cpio -", pipe_cmd="cpio -idvm"
-        ),
+        "*.rpm": ArchiveCommand(extract_cmd="rpm2cpio -", pipe_cmd="cpio -idvm"),
         "*.deb": ArchiveCommand(extract_cmd="ar -x"),
         "*.bz2": ArchiveCommand(
             extract_cmd="bzip2 -d -c -", uses_stdin=True, uses_stdout=True
         ),
         "*.gz": ArchiveCommand(
             extract_cmd="gzip -d -c -", uses_stdin=True, uses_stdout=True
         ),
@@ -462,15 +448,15 @@
     os.chdir(working_dir)
 
     # pass archives and their ArchiveCommand's to simple_extract
     for archive, archive_cmd in zip(glob_files, commands):
         root_cmd = archive_cmd.extract_cmd.split()[0]
         if not command_exists(root_cmd):
             logging.warning(
-                "Error: %s does not exist...not extracting %s.",root_cmd, archive
+                "Error: %s does not exist...not extracting %s.", root_cmd, archive
             )
             continue
         logging.info("Extracting archive %s", archive)
         simple_extract(archive, archive_cmd, no_clobber=parsed.no_clobber)
 
     end_time = datetime.datetime.now()
     logging.info("simple-extract finished @ %s", end_time)
```

### Comparing `simple-extract-0.3.1/src/simple_extract.egg-info/PKG-INFO` & `simple_extract-0.3.2/src/simple_extract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-extract
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small command line utility to help extract compressed archives.
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/simple_extract
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
```

