# Comparing `tmp/radiotray-ng-mpris-0.1.1.tar.gz` & `tmp/radiotray_ng_mpris-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiotray-ng-mpris-0.1.1.tar", last modified: Fri Nov  4 16:50:56 2022, max compression
+gzip compressed data, was "radiotray_ng_mpris-0.1.2.tar", last modified: Tue Apr 30 15:44:42 2024, max compression
```

## Comparing `radiotray-ng-mpris-0.1.1.tar` & `radiotray_ng_mpris-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 16:50:56.365885 radiotray-ng-mpris-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1050 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3581 2022-11-04 16:50:56.365885 radiotray-ng-mpris-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2609 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 16:50:56.363885 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/
--rw-rw-rw-   0 root         (0) root         (0)      294 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4177 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    15462 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 16:50:56.365885 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3581 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-11-04 16:50:56.000000 radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-04 16:50:56.366885 radiotray-ng-mpris-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3598 2022-11-04 16:50:46.000000 radiotray-ng-mpris-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 15:44:42.440792 radiotray_ng_mpris-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-04-30 15:44:42.439792 radiotray_ng_mpris-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 15:44:42.437792 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4177 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    15558 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 15:44:42.439792 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-30 15:44:42.000000 radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 15:44:42.440792 radiotray_ng_mpris-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2024-04-30 15:44:32.000000 radiotray_ng_mpris-0.1.2/setup.py
```

### Comparing `radiotray-ng-mpris-0.1.1/LICENSE` & `radiotray_ng_mpris-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `radiotray-ng-mpris-0.1.1/PKG-INFO` & `radiotray_ng_mpris-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiotray-ng-mpris
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper script for Radiotray-NG which provides an MPRIS2 interface.
 Home-page: https://github.com/IngoMeyer441/radiotray-ng-mpris
 Author: Ingo Meyer
 Author-email: IJ_M@gmx.de
 License: MIT
 Keywords: multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mpris-server
+Requires-Dist: pydbus
+Requires-Dist: yacl
 
 # Radiotray-NG MPRIS
 
 ## Overview
 
 Radiotray-NG MPRIS is a wrapper for [Radiotray-NG](https://github.com/ebruck/radiotray-ng) to add an [MPRIS2
 interface](https://specifications.freedesktop.org/mpris-spec/latest/) which integrates well with desktop environments
```

### Comparing `radiotray-ng-mpris-0.1.1/README.md` & `radiotray_ng_mpris-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/cli.py` & `radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,19 @@
     parser = get_argumentparser()
     args = parser.parse_args()
     if args.print_version:
         return args
     args.verbosity_level = (
         Verbosity.QUIET
         if args.quiet
-        else Verbosity.ERROR
-        if args.error
-        else Verbosity.VERBOSE
-        if args.verbose
-        else Verbosity.DEBUG
-        if args.debug
-        else Verbosity.WARN
+        else (
+            Verbosity.ERROR
+            if args.error
+            else Verbosity.VERBOSE if args.verbose else Verbosity.DEBUG if args.debug else Verbosity.WARN
+        )
     )
     return args
 
 
 def setup_stderr_logging(verbosity_level: Verbosity) -> None:
     if verbosity_level == Verbosity.QUIET:
         logging.getLogger().handlers = []
```

### Comparing `radiotray-ng-mpris-0.1.1/radiotray_ng_mpris/wrap.py` & `radiotray_ng_mpris-0.1.2/radiotray_ng_mpris/wrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,39 @@
 import time
 from pprint import pformat
 from types import FrameType
 from typing import Optional, cast
 
 import pydbus
 from gi.repository import GLib
-from mpris_server import Metadata, MetadataObj
-from mpris_server.adapters import (
+from mpris_server.adapters import ActivePlaylist, MprisAdapter
+from mpris_server.base import (
     DEFAULT_DESKTOP,
     DEFAULT_ORDERINGS,
     DEFAULT_PLAYLIST_COUNT,
     DEFAULT_RATE,
     MIME_TYPES,
     URI,
-    ActivePlaylist,
     DbusObj,
     Microseconds,
-    MprisAdapter,
     Paths,
     PlaylistEntry,
     PlayState,
-    RateDecimal,
     Track,
-    ValidMetadata,
-    VolumeDecimal,
 )
 from mpris_server.events import EventAdapter
-from mpris_server.mpris.metadata import DEFAULT_METADATA
+from mpris_server.mpris.metadata import DEFAULT_METADATA, Metadata, MetadataObj, ValidMetadata
 from mpris_server.server import Server
 
+try:
+    from mpris_server.base import Rate, Volume
+except ImportError:
+    from mpris_server.base import RateDecimal as Rate
+    from mpris_server.base import VolumeDecimal as Volume
+
 MAX_DBUS_GET_TRY_COUNT = 10
 RADIOTRAY_NG_DEFAULT_POLL_INTERVAL = 1000  # ms
 
 
 logger = logging.getLogger(__name__)
 radiotray_ng_process = None
 
@@ -236,45 +237,45 @@
 
     def set_repeating(self, val: bool) -> None:
         pass
 
     def set_loop_status(self, val: str) -> None:
         pass
 
-    def get_rate(self) -> RateDecimal:
+    def get_rate(self) -> Rate:
         return DEFAULT_RATE
 
-    def set_rate(self, val: RateDecimal) -> None:
+    def set_rate(self, val: Rate) -> None:
         pass
 
-    def set_minimum_rate(self, val: RateDecimal) -> None:
+    def set_minimum_rate(self, val: Rate) -> None:
         pass
 
-    def set_maximum_rate(self, val: RateDecimal) -> None:
+    def set_maximum_rate(self, val: Rate) -> None:
         pass
 
-    def get_minimum_rate(self) -> RateDecimal:
+    def get_minimum_rate(self) -> Rate:
         return DEFAULT_RATE
 
-    def get_maximum_rate(self) -> RateDecimal:
+    def get_maximum_rate(self) -> Rate:
         return DEFAULT_RATE
 
     def get_shuffle(self) -> bool:
         return False
 
     def set_shuffle(self, val: bool) -> None:
         pass
 
     def get_art_url(self, track: int) -> str:
         return ""
 
-    def get_volume(self) -> VolumeDecimal:
+    def get_volume(self) -> Volume:
         return float(self._radiotray_ng_api.get_player_state()["volume"]) / 100
 
-    def set_volume(self, val: VolumeDecimal) -> None:
+    def set_volume(self, val: Volume) -> None:
         self._radiotray_ng_api.set_volume(int(val * 100))
 
     def is_mute(self) -> bool:
         return bool(self._radiotray_ng_api.get_player_state()["mute"])
 
     def set_mute(self, val: bool) -> None:
         if val != self.is_mute():
@@ -308,15 +309,15 @@
         return Track("")
 
     def activate_playlist(self, id: DbusObj) -> None:
         pass
 
     def get_playlists(self, index: int, max_count: int, order: str, reverse: bool) -> list[PlaylistEntry]:
         # TODO
-        pass
+        return []
 
     def get_playlist_count(self) -> int:
         return cast(int, DEFAULT_PLAYLIST_COUNT)
 
     def get_orderings(self) -> list[str]:
         return cast(list[str], DEFAULT_ORDERINGS)
 
@@ -334,15 +335,15 @@
         pass
 
     def go_to(self, track_id: DbusObj) -> None:
         pass
 
     def get_tracks(self) -> list[DbusObj]:
         # TODO
-        pass
+        return []
 
     def can_edit_tracks(self) -> bool:
         return False
 
 
 class RadiotrayNgEventAdapter:
     def __init__(
```

### Comparing `radiotray-ng-mpris-0.1.1/radiotray_ng_mpris.egg-info/PKG-INFO` & `radiotray_ng_mpris-0.1.2/radiotray_ng_mpris.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiotray-ng-mpris
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper script for Radiotray-NG which provides an MPRIS2 interface.
 Home-page: https://github.com/IngoMeyer441/radiotray-ng-mpris
 Author: Ingo Meyer
 Author-email: IJ_M@gmx.de
 License: MIT
 Keywords: multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mpris-server
+Requires-Dist: pydbus
+Requires-Dist: yacl
 
 # Radiotray-NG MPRIS
 
 ## Overview
 
 Radiotray-NG MPRIS is a wrapper for [Radiotray-NG](https://github.com/ebruck/radiotray-ng) to add an [MPRIS2
 interface](https://specifications.freedesktop.org/mpris-spec/latest/) which integrates well with desktop environments
```

### Comparing `radiotray-ng-mpris-0.1.1/setup.py` & `radiotray_ng_mpris-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import runpy
 import subprocess
-from distutils.cmd import Command
 from tempfile import TemporaryDirectory
 from typing import List, Optional, Tuple, cast
 
-from setuptools import find_packages, setup
+from setuptools import Command, find_packages, setup
 
 
 class PyinstallerCommand(Command):
     description = "create a self-contained executable with PyInstaller"
-    user_options = []  # type: List[Tuple[str, Optional[str], str]]
+    user_options: List[Tuple[str, Optional[str], str]] = []
 
     def initialize_options(self) -> None:
         pass
 
     def finalize_options(self) -> None:
         pass
 
@@ -51,16 +50,16 @@
 
 
 def get_version_from_pyfile(version_file: str = "radiotray_ng_mpris/_version.py") -> str:
     file_globals = runpy.run_path(version_file)
     return cast(str, file_globals["__version__"])
 
 
-def get_long_description_from_readme(readme_filename: str = "README.md") -> Optional[str]:
-    long_description = None
+def get_long_description_from_readme(readme_filename: str = "README.md") -> str:
+    long_description = ""
     if os.path.isfile(readme_filename):
         with open(readme_filename, "r", encoding="utf-8") as readme_file:
             long_description = readme_file.read()
     return long_description
 
 
 version = get_version_from_pyfile()
```

