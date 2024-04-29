# Comparing `tmp/pycatfile-0.8.6.tar.gz` & `tmp/pycatfile-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatfile-0.8.6.tar", last modified: Fri Apr 26 23:59:29 2024, max compression
+gzip compressed data, was "pycatfile-0.9.0.tar", last modified: Mon Apr 29 22:46:32 2024, max compression
```

## Comparing `pycatfile-0.8.6.tar` & `pycatfile-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:59:29.516924 pycatfile-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 23:59:21.000000 pycatfile-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 23:59:29.516924 pycatfile-0.8.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:59:29.516924 pycatfile-0.8.6/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 23:59:21.000000 pycatfile-0.8.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    12671 2024-04-26 23:59:21.000000 pycatfile-0.8.6/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-26 23:59:21.000000 pycatfile-0.8.6/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   361778 2024-04-26 23:59:21.000000 pycatfile-0.8.6/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 23:59:29.516924 pycatfile-0.8.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-26 23:59:21.000000 pycatfile-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:46:32.446028 pycatfile-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-29 22:46:21.000000 pycatfile-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-29 22:46:32.446028 pycatfile-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:46:32.446028 pycatfile-0.9.0/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-29 22:46:32.000000 pycatfile-0.9.0/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 22:46:32.000000 pycatfile-0.9.0/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:46:32.000000 pycatfile-0.9.0/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 22:46:32.000000 pycatfile-0.9.0/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:46:32.000000 pycatfile-0.9.0/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 22:46:21.000000 pycatfile-0.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9711 2024-04-29 22:46:21.000000 pycatfile-0.9.0/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-29 22:46:21.000000 pycatfile-0.9.0/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   359212 2024-04-29 22:46:21.000000 pycatfile-0.9.0/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 22:46:32.446028 pycatfile-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-29 22:46:21.000000 pycatfile-0.9.0/setup.py
```

### Comparing `pycatfile-0.8.6/LICENSE` & `pycatfile-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatfile-0.8.6/PKG-INFO` & `pycatfile-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.8.6
+Version: 0.9.0
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.8.6/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.9.0/PyCatFile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.8.6
+Version: 0.9.0
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.8.6/catfile.py` & `pycatfile-0.9.0/catfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/29/2024 Ver. 0.9.0 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 py7zr_support = pycatfile.py7zr_support;
@@ -114,101 +114,71 @@
 should_repack = getargs.create and getargs.repack;
 should_validate = getargs.validate;
 
 # Execute the appropriate functions based on determined actions and arguments
 if should_create:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
-  if(checkcompressfile=="tarfile"):
-   pycatfile.PackArchiveFileFromTarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="zipfile"):
-   pycatfile.PackArchiveFileFromZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="catfile"):
-   pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
-  elif(rarfile_support and checkcompressfile=="rarfile"):
-   pycatfile.PackArchiveFileFromRarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(py7zr_support and checkcompressfile=="7zipfile"):
-   pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(checkcompressfile=="catfile"):
+   tmpout = pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   else:
+   tmpout = pycatfile.PackArchiveFileFromInFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(not tmpout):
    sys.exit(1);
  else:
   pycatfile.PackArchiveFile(getargs.input, getargs.output, getargs.text, getargs.compression, getargs.level, False, getargs.checksum, [], fnamelist, getargs.verbose, False);
 
 elif should_repack:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
-  if(checkcompressfile=="tarfile"):
-   pycatfile.PackArchiveFileFromTarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="zipfile"):
-   pycatfile.PackArchiveFileFromZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="catfile"):
+  if(checkcompressfile=="catfile"):
    pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
-  elif(rarfile_support and checkcompressfile=="rarfile"):
-   pycatfile.PackArchiveFileFromRarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(py7zr_support and checkcompressfile=="7zipfile"):
-   pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   else:
+   pycatfile.PackArchiveFileFromInFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(not tmpout):
    sys.exit(1);
  else:
   pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
 
 elif should_extract:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   tempout = BytesIO();
-  if(checkcompressfile=="tarfile"):
-   pycatfile.PackArchiveFileFromTarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="zipfile"):
-   pycatfile.PackArchiveFileFromZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="catfile"):
-   pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
-  elif(rarfile_support and checkcompressfile=="rarfile"):
-   pycatfile.PackArchiveFileFromRarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(py7zr_support and checkcompressfile=="7zipfile"):
-   pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(checkcompressfile=="catfile"):
+   tmpout = pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   else:
+   tmpout = pycatfile.PackArchiveFileFromInFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(not tmpout):
    sys.exit(1);
   getargs.input = tempout;
  pycatfile.UnPackArchiveFile(getargs.input, getargs.output, False, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, getargs.preserve, getargs.preserve, False);
 
 elif should_list:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
-  if(checkcompressfile=="tarfile"):
-   pycatfile.TarFileListFiles(getargs.input, getargs.verbose, False);
-  elif(checkcompressfile=="zipfile"):
-   pycatfile.ZipFileListFiles(getargs.input, getargs.verbose, False);
-  elif(checkcompressfile=="catfile"):
-   pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
-  elif(rarfile_support and checkcompressfile=="rarfile"):
-   pycatfile.RarFileListFiles(getargs.input, getargs.verbose, False);
-  elif(py7zr_support and checkcompressfile=="7zipfile"):
-   pycatfile.SevenZipFileListFiles(getargs.input, getargs.verbose, False);
+  if(checkcompressfile=="catfile"):
+   tmpout = pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
   else:
+   tmpout = pycatfile.InFileListFiles(getargs.input, getargs.verbose, fnamelist, False);
+  if(not tmpout):
    sys.exit(1);
  else:
   pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
 
 elif should_validate:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   tempout = BytesIO();
-  if(checkcompressfile=="tarfile"):
-   pycatfile.PackArchiveFileFromTarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="zipfile"):
-   pycatfile.PackArchiveFileFromZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(checkcompressfile=="catfile"):
-   pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
-  elif(rarfile_support and checkcompressfile=="rarfile"):
-   pycatfile.PackArchiveFileFromRarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
-  elif(py7zr_support and checkcompressfile=="7zipfile"):
-   pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
+  if(checkcompressfile=="catfile"):
+   tmpout = pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   else:
-   sys.exit(1);
+   tmpout = pycatfile.PackArchiveFileFromInFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   getargs.input = tempout;
+  if(not tmpout):
+   sys.exit(1);
  fvalid = pycatfile.ArchiveFileValidate(getargs.input, fnamelist, getargs.verbose, False);
  if(not getargs.verbose):
   import sys, logging;
   logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(fvalid):
   pycatfile.VerbosePrintOut("File is valid: \n" + str(getargs.input));
  else:
```

### Comparing `pycatfile-0.8.6/neocatfile.py` & `pycatfile-0.9.0/neocatfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/29/2024 Ver. 0.9.0 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `pycatfile-0.8.6/pycatfile.py` & `pycatfile-0.9.0/pycatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/29/2024 Ver. 0.9.0 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -167,19 +167,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 8, 6, "RC 1", 1);
-__version_date_info__ = (2024, 4, 26, "RC 1", 1);
+__version_info__ = (0, 9, 0, "RC 1", 1);
+__version_date_info__ = (2024, 4, 29, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: d45dc765c1f1cbdec9b8820a0e3bcda7bb6e3940 $";
+__revision_id__ = "$Id: 12ec091d1c25a5e892a36b4e662e5b9093ee2a61 $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -2611,14 +2611,16 @@
  def PackArchiveFileFunc(archive_name, source_dir, **kwargs):
   return PackArchiveFile(source_dir, archive_name, False, "auto", None, False, "crc32", [], __file_format_delimiter__, False, False);
  create_alias_function("Pack", __file_format_name__, "Func", PackArchiveFileFunc);
 
 def PackArchiveFileFromDirList(infiles, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  return PackArchiveFile(infiles, outfile, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, extradata, formatspecs, verbose, returnfp);
 
+create_alias_function("Pack", __file_format_name__, "FromDirList", PackArchiveFileFromDirList);
+
 def PackArchiveFileFromTarFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   outfile = RemoveWindowsPath(outfile);
  checksumtype = checksumtype.lower();
  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
   checksumtype="crc32";
  if(checksumtype=="none"):
@@ -3829,14 +3831,16 @@
    catfp.close()
    return True;
 
 create_alias_function("Pack", __file_format_name__, "FromSevenZipFile", PackArchiveFileFromSevenZipFile);
 
 def PackArchiveFileFromInFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  checkcompressfile = CheckCompressionSubType(infile, formatspecs, True);
+ if(verbose):
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(checkcompressfile=="tarfile"):
   return PackArchiveFileFromTarFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
  elif(checkcompressfile=="zipfile"):
   return PackArchiveFileFromZipFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
  elif(checkcompressfile=="catfile"):
   return RePackArchiveFile(infile, outfile, compression, compressionlevel, False, 0, 0, checksumtype, False, extradata, formatspecs, verbose, returnfp);
  elif(rarfile_support and checkcompressfile=="rarfile"):
@@ -7237,67 +7241,15 @@
 create_alias_function("", __file_format_name__, "ListFiles", ArchiveFileListFiles);
 
 def ArchiveFileStringListFiles(catstr, seekstart=0, seekend=0, skipchecksum=False, formatspecs=__file_format_list__, verbose=False, returnfp=False):
  catfp = BytesIO(catstr);
  listcatfiles = ArchiveFileListFiles(catstr, seekstart, seekend, skipchecksum, formatspecs, verbose, returnfp);
  return listcatfiles;
 
-create_alias_function("", __file_format_name__, "StringListFiles", ArchiveFileListFiles);
-
-def ArchiveFileListFilesAlt(infile, seekstart=0, seekend=0, skipchecksum=False, formatspecs=__file_format_list__, verbose=False, returnfp=False):
- logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
- if(isinstance(infile, dict)):
-  listcatfiles = infile;
- else:
-  if(infile!="-" and not hasattr(infile, "read") and not hasattr(infile, "write")):
-   infile = RemoveWindowsPath(infile);
-  listcatfiles = ArchiveFileToArray(infile, seekstart, seekend, True, skipchecksum, formatspecs, returnfp);
- if(not listcatfiles):
-  return False;
- lenlist = len(listcatfiles['ffilelist']);
- fnumfiles = int(listcatfiles['fnumfiles']);
- lcfi = 0;
- lcfx = int(listcatfiles['fnumfiles']);
- if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
-  lcfx = int(lenlist);
- else:
-  lcfx = int(listcatfiles['fnumfiles']);
- returnval = {};
- while(lcfi<lcfx):
-  returnval.update({lcfi: listcatfiles['ffilelist'][lcfi]['fname']});
-  if(not verbose):
-   VerbosePrintOut(listcatfiles['ffilelist'][lcfi]['fname']);
-  if(verbose):
-   permissions = { 'access': { '0': ('---'), '1': ('--x'), '2': ('-w-'), '3': ('-wx'), '4': ('r--'), '5': ('r-x'), '6': ('rw-'), '7': ('rwx') }, 'roles': { 0: 'owner', 1: 'group', 2: 'other' } };
-   printfname = listcatfiles['ffilelist'][lcfi]['fname'];
-   if(listcatfiles['ffilelist'][lcfi]['ftype']==1):
-    printfname = listcatfiles['ffilelist'][lcfi]['fname'] + " link to " + listcatfiles['ffilelist'][lcfi]['flinkname'];
-   if(listcatfiles['ffilelist'][lcfi]['ftype']==2):
-    printfname = listcatfiles['ffilelist'][lcfi]['fname'] + " -> " + listcatfiles['ffilelist'][lcfi]['flinkname'];
-   fuprint = listcatfiles['ffilelist'][lcfi]['funame'];
-   if(len(fuprint)<=0):
-    fuprint = listcatfiles['ffilelist'][lcfi]['fuid'];
-   fgprint = listcatfiles['ffilelist'][lcfi]['fgname'];
-   if(len(fgprint)<=0):
-    fgprint = listcatfiles['ffilelist'][lcfi]['fgid'];
-   VerbosePrintOut(PrintPermissionString(listcatfiles['ffilelist'][lcfi]['fmode'], listcatfiles['ffilelist'][lcfi]['ftype']) + " " + str(str(fuprint) + "/" + str(fgprint) + " " + str(listcatfiles['ffilelist'][lcfi]['fsize']).rjust(15) + " " + datetime.datetime.utcfromtimestamp(listcatfiles['ffilelist'][lcfi]['fmtime']).strftime('%Y-%m-%d %H:%M') + " " + printfname));
-  lcfi = lcfi + 1;
- if(returnfp):
-  return listcatfiles['catfp'];
- else:
-  return True;
-
-create_alias_function("", __file_format_name__, "ListFilesAlt", ArchiveFileListFilesAlt);
-
-def ArchiveFileStringListFilesAlt(catstr, seekstart=0, seekend=0, skipchecksum=False, formatspecs=__file_format_list__, verbose=False, returnfp=False):
- catfp = BytesIO(catstr);
- listcatfiles = ArchiveFileListFilesAlt(catstr, seekstart, seekend, skipchecksum, formatspecs, verbose, returnfp);
- return listcatfiles;
-
-create_alias_function("", __file_format_name__, "StringListFilesAlt", ArchiveFileListFilesAlt);
+create_alias_function("", __file_format_name__, "StringListFiles", ArchiveFileStringListFiles);
 
 def TarFileListFiles(infile, verbose=False, returnfp=False):
  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(infile=="-"):
   infile = BytesIO();
   if(hasattr(sys.stdin, "buffer")):
    shutil.copyfileobj(sys.stdin.buffer, infile);
@@ -7747,21 +7699,22 @@
    lcfi = lcfi + 1;
   if(returnfp):
    return listcatfiles['catfp'];
   else:
    return True;
 
 def InFileListFiles(infile, verbose=False, formatspecs=__file_format_list__, returnfp=False):
+ logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  checkcompressfile = CheckCompressionSubType(infile, formatspecs, True);
  if(checkcompressfile=="tarfile"):
   return TarFileListFiles(infile, verbose, returnfp);
  elif(checkcompressfile=="zipfile"):
   return ZipFileListFiles(infile, verbose, returnfp);
  elif(checkcompressfile=="catfile"):
-  return ArchiveFileListFiles(infile, verbose, returnfp);
+  return ArchiveFileListFiles(infile, 0, 0, False, formatspecs, verbose, returnfp);
  elif(rarfile_support and checkcompressfile=="rarfile"):
   return RarFileListFiles(infile, verbose, returnfp);
  elif(py7zr_support and checkcompressfile=="7zipfile"):
   return SevenZipFileListFiles(infile, verbose, returnfp);
  else:
   return False;
  return False;
```

### Comparing `pycatfile-0.8.6/setup.py` & `pycatfile-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/29/2024 Ver. 0.9.0 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

