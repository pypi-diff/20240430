# Comparing `tmp/snapmap_archiver-2.2.0.tar.gz` & `tmp/snapmap_archiver-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapmap_archiver-2.2.0.tar", max compression
+gzip compressed data, was "snapmap_archiver-2.3.0.tar", max compression
```

## Comparing `snapmap_archiver-2.2.0.tar` & `snapmap_archiver-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35823 2024-04-26 12:55:26.451161 snapmap_archiver-2.2.0/LICENSE
--rw-r--r--   0        0        0      554 2024-04-26 14:12:41.918031 snapmap_archiver-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2262 2024-04-26 12:55:26.451161 snapmap_archiver-2.2.0/README.md
--rw-r--r--   0        0        0     2179 2024-04-26 13:35:15.422379 snapmap_archiver-2.2.0/snapmap_archiver/__init__.py
--rw-r--r--   0        0        0       84 2024-04-26 12:55:26.455162 snapmap_archiver-2.2.0/snapmap_archiver/__main__.py
--rw-r--r--   0        0        0      599 2024-04-26 13:31:54.392135 snapmap_archiver-2.2.0/snapmap_archiver/coordinates.py
--rw-r--r--   0        0        0      283 2024-04-26 13:31:54.393136 snapmap_archiver-2.2.0/snapmap_archiver/snap.py
--rw-r--r--   0        0        0     9360 2024-04-26 13:57:40.865489 snapmap_archiver-2.2.0/snapmap_archiver/SnapmapArchiver.py
--rw-r--r--   0        0        0      520 2024-04-26 13:53:40.404385 snapmap_archiver-2.2.0/snapmap_archiver/time.py
--rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 snapmap_archiver-2.2.0/setup.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 snapmap_archiver-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-04-26 12:55:26.451161 snapmap_archiver-2.3.0/LICENSE
+-rw-r--r--   0        0        0      650 2024-04-30 09:49:54.846102 snapmap_archiver-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3275 2024-04-30 09:49:54.845102 snapmap_archiver-2.3.0/README.md
+-rw-r--r--   0        0        0      564 2024-04-30 09:49:54.847103 snapmap_archiver-2.3.0/snapmap_archiver/__init__.py
+-rw-r--r--   0        0        0     4032 2024-04-30 09:49:54.847103 snapmap_archiver-2.3.0/snapmap_archiver/__main__.py
+-rw-r--r--   0        0        0      597 2024-04-30 09:49:54.847103 snapmap_archiver-2.3.0/snapmap_archiver/coordinates.py
+-rw-r--r--   0        0        0      283 2024-04-26 13:31:54.393136 snapmap_archiver-2.3.0/snapmap_archiver/snap.py
+-rw-r--r--   0        0        0    10323 2024-04-30 09:49:54.846102 snapmap_archiver-2.3.0/snapmap_archiver/SnapmapArchiver.py
+-rw-r--r--   0        0        0      523 2024-04-30 09:49:54.848103 snapmap_archiver-2.3.0/snapmap_archiver/time.py
+-rw-r--r--   0        0        0     4200 1970-01-01 00:00:00.000000 snapmap_archiver-2.3.0/setup.py
+-rw-r--r--   0        0        0     3886 1970-01-01 00:00:00.000000 snapmap_archiver-2.3.0/PKG-INFO
```

### Comparing `snapmap_archiver-2.2.0/LICENSE` & `snapmap_archiver-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snapmap_archiver-2.2.0/README.md` & `snapmap_archiver-2.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 # snapmap-archiver
 
-A tool written in Python **3.10** to download all Snapmaps content from a specific location.
+Download all Snap Map content from a specific location.
 
-## Install Python 3.10+
+![snapmap-archiver splash](/.github/img/Splash.png)
 
-Be sure to check that you're using a version of Python that is 3.10 or above. **This project will not work on Python 3.9 or below!**
+[View on PyPI](https://pypi.org/project/snapmap-archiver/)
 
-![snapmap-archiver splash](/.github/img/Splash.png)
+## Installation (for general usage)
 
-`pip install snapmap-archiver`
+Install with `pip` or `pipx` or whatever trendy Python package manager you use:
 
-[View on PyPI](https://pypi.org/project/snapmap-archiver/)
+```sh
+pip install snapmap-archiver
+```
+
+## Local Development Setup
 
-## Setup (for working in a Python environment)
+Install Poetry with `pip` or `pipx`:
+
+```sh
+pip install poetry
+```
+
+Install the project dependencies:
+
+```sh
+poetry install
+```
 
-Install dependencies with `pip`.
+Run the app with Poetry:
 
 ```sh
-pip install -r requirements.txt
+poetry run python3 main.py [...args]
 ```
 
 ## Usage
 
 ```sh
 snapmap-archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"
 ```
 
-Unfortunately you have to use the arbitrary `-l="lat,lon"` rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.
+Unfortunately you have to use the arbitrary `-l="lat,lon"` (with the equals sign) rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.
 
 ### Optional Arguments
 
 #### Location
 
 `-l` is not required if an input file or Snap URL is provided. It can also be used multiple times to download Snaps from multiple locations in one command.
 
@@ -63,16 +77,42 @@
 
 You can also just pass 1 or more normal Snap URLs or IDs to the package to download it individually like this:
 
 ```sh
 snapmap-archiver -o ~/Desktop/snap 'https://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z' 'Example'
 ```
 
+#### Time Filter
+
+Use the `-t` flag with a Unix timestamp or day, hour, or minute interval to skip the download of any snaps older than that point.
+
+Example with a Unix timestamp:
+
+```sh
+snapmap-archiver -t 1714392291 -l '-123,123'
+```
+
+Examples with a dynamic time filter:
+
+```sh
+snapmap-archiver -t 3d -l='-123,123'  # Removes anything older than 3 days
+snapmap-archiver -t 5h -l='-123,123'  # Removes anything older than 5 hours
+snapmap-archiver -t 30m -l='-123,123'  # Removes anything older than 30 minutes
+```
+
 #### Export JSON
 
 You can export a JSON file with info about downloaded snaps with the `--write-json` argument, which will contain information like the time the Snap was posted, and the Snap location.
 
 It will write `archive.json` to the specified output directory.
 
 #### Snap Radius
 
 The radius from the coordinates you provide that will be included for downloads. `-r 20000` will download all Snaps within a 20km radius of your coordinates.
+
+#### Zoom Depth
+
+You can input a custom zoom depth value (`-z`) that correlates to a zoom level in the GUI. ArcGIS has documentation about this [here](https://developers.arcgis.com/documentation/glossary/zoom-level/), but essentially the lower the number, the further zoomed-out you are. `5` is the default and shouldn't cause any issues.
+
+#### Debug Mode
+
+Enable debug logs with `-d`/`--debug`.
```

### Comparing `snapmap_archiver-2.2.0/snapmap_archiver/coordinates.py` & `snapmap_archiver-2.3.0/snapmap_archiver/coordinates.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     def __init__(self, coord_str: str):
         try:
             lat, long = coord_str.split(",", 1)
             self.lat = float(lat)
             self.long = float(long)
         except Exception:
             raise ValueError(
-                f'Provided coordinates [{coord_str}] could not be split to lat/long points. Use comma seperated values for latitude/longitude, e.g: -l="35.0,67.0".'
+                f'Provided coordinates [{coord_str}] could not be split to lat/long points. Use comma seperated values for latitude/longitude, e.g: "35.0,67.0".'
             )
 
     def __str__(self) -> str:
         return f"Lat: {self.lat}, Lon: {self.long}"
 
     def __repr__(self) -> str:
-        return f"({self.lat},{self.long})"
+        return f"({self.lat}, {self.long})"
```

### Comparing `snapmap_archiver-2.2.0/snapmap_archiver/SnapmapArchiver.py` & `snapmap_archiver-2.3.0/snapmap_archiver/SnapmapArchiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,255 +1,280 @@
+import asyncio
 import json
 import os
-import re
 import sys
 import typing as t
 from datetime import datetime
 from time import sleep
 
+import aiofiles
+import httpx
 import requests
+from alive_progress import alive_bar
+from loguru._logger import Logger
 
+from snapmap_archiver import (
+    DEFAULT_API_HOST,
+    DEFAULT_RADIUS,
+    DEFAULT_WRITE_JSON,
+    DEFAULT_ZOOM_DEPTH,
+    ISSUES_URL,
+    default_output_dir,
+)
 from snapmap_archiver.coordinates import Coordinates
 from snapmap_archiver.snap import Snap, SnapJSONEncoder
 from snapmap_archiver.time import since_epoch
 
-DEFAULT_RADIUS = 10_000
 MAX_RADIUS = 85_000
-ISSUES_URL = "https://github.com/king-millez/snapmap-archiver/issues/new/choose"
-SNAP_PATTERN = re.compile(
-    r"(?:https?:\/\/map\.snapchat\.com\/ttp\/snap\/)?(W7_(?:[a-zA-Z0-9\-_\+]{56})(?:\/?@-?[0-9]{1,3}\.?[0-9]{0,},-?[0-9]{1,3}\.?[0-9]{0,}(?:,[0-9]{1,3}\.?[0-9]{0,}z))?)"
-)
 
 
 class SnapmapArchiver:
     def __init__(
         self,
-        *args: str,
-        output_dir: str,
-        input_file: t.Optional[str] = None,
+        logger: Logger,
+        output_dir: str = default_output_dir,
         since_time: t.Optional[str] = None,
-        locations: list[str] = [],
-        radius: int = DEFAULT_RADIUS,
-        write_json: bool = False,
-        zoom_depth: int = 5,
+        write_json: bool = DEFAULT_WRITE_JSON,
+        api_host: str = DEFAULT_API_HOST,
     ) -> None:
         if sys.version_info < (3, 10):
             raise RuntimeError(
                 "Python 3.10 or above is required to use snapmap-archiver!"
             )
 
+        self.logger = logger
+        self.api_host = api_host
+        self.output_dir = os.path.expanduser(output_dir)
+        self.write_json = write_json
+
         self.since_time = None
         if since_time:
             self.since_time = since_epoch(since_time.lower())
-            print(f"Skipping Snaps older than [{self.since_time}].")
-
-        self.input_file = input_file
-        self.arg_snaps = args
+            self.logger.info(f"Skipping Snaps older than [{self.since_time}].")
 
-        self.write_json = write_json
-        self.zoom_depth = zoom_depth
-        self.all_snaps: dict[str, Snap] = {}
-
-        if not locations and not args and not input_file:
-            raise ValueError(
-                "Some sort of input is required. Run snapmap-archiver with [-h] to see a list of options."
-            )
+        self.snap_cache: dict[str, Snap] = {}
 
-        self.output_dir = os.path.expanduser(output_dir)
         if not os.path.isdir(self.output_dir):
             os.makedirs(self.output_dir, exist_ok=True)
 
-        self.radius = MAX_RADIUS if radius > MAX_RADIUS else radius
-        self.coords_list = [Coordinates(latlon) for latlon in locations]
-
-    def download_snaps(self, group: t.Iterable[Snap]):
-        for snap in group:
-            fpath = os.path.join(self.output_dir, f"{snap.snap_id}.{snap.file_type}")
-
-            if os.path.isfile(fpath):
-                print(f" - [{fpath}] already exists.")
-                continue
+    def _is_cached(self, snap_id: str) -> bool:
+        return snap_id in self.snap_cache
 
-            with open(fpath, "wb") as f:
-                f.write(requests.get(snap.url).content)
+    async def _batched_download(
+        self, snap_url: str, output_path: str, bar: t.Any, client: httpx.AsyncClient
+    ):
+        if os.path.isfile(output_path):
+            self.logger.debug(f" - [{output_path}] already exists.")
+            bar()
+            return
+
+        async with aiofiles.open(output_path, "wb") as f:
+            await f.write((await client.get(snap_url)).content)
+
+        self.logger.debug(f" - Downloaded [{output_path}].")
+        bar()
+
+    def download_cached_snaps(self):
+        with alive_bar(
+            len(self.snap_cache), title=f"Downloading to [{self.output_dir}]..."
+        ) as bar:
+            all_snaps = list(self.snap_cache.values())
+            client = httpx.AsyncClient()
+            for snap_chunk in [
+                all_snaps[i : i + 20]
+                for i in range(
+                    0, len(all_snaps), 20
+                )  # 20 connections seems to be ok with rate limits.
+            ]:
+                asyncio.get_event_loop().run_until_complete(
+                    asyncio.gather(
+                        *[
+                            self._batched_download(
+                                snap.url,
+                                os.path.join(
+                                    self.output_dir, f"{snap.snap_id}.{snap.file_type}"
+                                ),
+                                bar,
+                                client,
+                            )
+                            for snap in snap_chunk
+                        ]
+                    )
+                )
 
-            print(f" - Downloaded [{fpath}].")
+        if self.write_json:
+            with open(
+                os.path.join(
+                    self.output_dir, f"archive_{int(datetime.now().timestamp())}.json"
+                ),
+                "w",
+            ) as f:
+                json.dump(
+                    list(self.snap_cache.values()),
+                    f,
+                    indent=2,
+                    cls=SnapJSONEncoder,
+                )
 
     def query_snaps(self, snaps: t.Iterable[str]) -> list[Snap]:
-        to_query: list[str] = []
-        for snap_id in snaps:
-            rgx_match = re.search(
-                SNAP_PATTERN,
-                snap_id,
-            )
-            if not rgx_match:
-                print(f" - [{snap_id}] is not a valid Snap URL or ID.")
-                continue
-            to_query.append(rgx_match.group(1))
-
+        to_query = [snap_id for snap_id in snaps if not self._is_cached(snap_id)]
         if not to_query:
             return []
 
         api_response = requests.post(
-            "https://ms.sc-jpl.com/web/getStoryElements",
+            f"{self.api_host}/web/getStoryElements",
             json={"snapIds": to_query},
         )
+
         try:
-            retl: list[Snap] = []
+            parsed_snaps: list[Snap] = []
             for snap in api_response.json().get("elements", []):
                 s = self._parse_snap(snap)
                 if s:
-                    retl.append(s)
-            return retl
+                    parsed_snaps.append(s)
+            return parsed_snaps
         except requests.exceptions.JSONDecodeError as e:
-            print(
+            self.logger.warning(
                 f"Encountered error while querying Snap IDs:\n[{e}]. API Response: [{api_response.text}]."
             )
             return []
 
-    def query_coords(self, coords: Coordinates):
-        to_download: dict[str, Snap] = {}
-        current_iteration = self.radius
+    def query_coords(
+        self,
+        coords: Coordinates,
+        zoom_depth: int = DEFAULT_ZOOM_DEPTH,
+        requested_radius: int = DEFAULT_RADIUS,
+    ) -> list[Snap]:
+        if requested_radius > MAX_RADIUS:
+            radius = MAX_RADIUS
+            self.logger.info(
+                f"Radius cannot be larger than [{MAX_RADIUS}]. Using [{MAX_RADIUS}] as the radius value."
+            )
+        else:
+            radius = requested_radius
+
+        current_iteration = radius
         epoch = self._get_epoch()
-        while current_iteration != 1:
-            print(f"Querying with radius [{current_iteration}]...")
-            json_data = None
-            while not json_data:
-                api_data = requests.post(
-                    "https://ms.sc-jpl.com/web/getPlaylist",
-                    headers={
-                        "Content-Type": "application/json",
-                    },
-                    json={
-                        "requestGeoPoint": {"lat": coords.lat, "lon": coords.long},
-                        "zoomLevel": self.zoom_depth,
-                        "tileSetId": {"flavor": "default", "epoch": epoch, "type": 1},
-                        "radiusMeters": current_iteration,
-                        "maximumFuzzRadius": 0,
-                    },
-                ).text
-
-                if api_data:
-                    if api_data.strip() == "Too many requests":
-                        print("You have been rate limited. Sleeping for 1 minute.")
-                        sleep(60)
+        found_snaps = []
+        with alive_bar(
+            radius, manual=True, title=f"Location: {coords.__repr__()}"
+        ) as bar:
+            while current_iteration != 1:
+                snaps_from_coords = None
+                while not snaps_from_coords:
+                    api_response = requests.post(
+                        f"{self.api_host}/web/getPlaylist",
+                        headers={
+                            "Content-Type": "application/json",
+                        },
+                        json={
+                            "requestGeoPoint": {"lat": coords.lat, "lon": coords.long},
+                            "zoomLevel": zoom_depth,
+                            "tileSetId": {
+                                "flavor": "default",
+                                "epoch": epoch,
+                                "type": 1,
+                            },
+                            "radiusMeters": current_iteration,
+                            "maximumFuzzRadius": 0,
+                        },
+                    ).text
+
+                    if not api_response:
+                        self._coordinate_query_failure("No response received.")
+                    elif api_response.strip() == "Too many requests":
+                        self._coordinate_query_failure("You have been rate limited.")
                     else:
                         try:
-                            json_data = json.loads(api_data)["manifest"]["elements"]
-                        except requests.exceptions.JSONDecodeError:
-                            print(
-                                f"Unable to decode API response (likely a rate limit): [{api_data}] Sleeping for 1 minute."
+                            snaps_from_coords = json.loads(api_response)["manifest"][
+                                "elements"
+                            ]
+                        except json.JSONDecodeError:
+                            self._coordinate_query_failure(
+                                f"Unable to decode API response (likely a rate limit): [{api_response}]."
                             )
-                            sleep(60)
 
-            for snap in json_data:
-                if to_download.get(
-                    snap["id"]
-                ):  # Avoids downloading duplicates. Faster than a list because the Snap ID is indexed
-                    continue
-
-                parsed = self._parse_snap(snap)
-
-                if not parsed:
-                    continue
-
-                to_download[snap["id"]] = parsed
-
-            if current_iteration > 2000:
-                current_iteration -= 2000
-            elif current_iteration > 1000:
-                current_iteration -= 100
-            else:
-                current_iteration = 1
-
-        print(f"Found [{len(list(to_download.keys()))}] Snaps.")
-        return to_download.values()
-
-    def main(self):
-        # Query provided coordinates
-        for coords in self.coords_list:
-            self.download_snaps(self.query_coords(coords))
-
-        snap_ids = []
-
-        # Download Snaps from input file
-        if self.input_file:
-            if os.path.isfile(self.input_file):
-                with open(self.input_file, "r") as f:
-                    snap_ids = [ln for ln in f.read().split("\n") if ln.strip()]
-            else:
-                raise FileNotFoundError(
-                    f"Input file [{self.input_file}] does not exist."
+                for snap in snaps_from_coords:
+                    if self._is_cached(snap["id"]):
+                        found_snaps.append(self.snap_cache[snap["id"]])
+                        continue
+
+                    parsed = self._parse_snap(snap)
+                    if not parsed:
+                        continue
+
+                    self.snap_cache[snap["id"]] = parsed
+                    found_snaps.append(parsed)
+
+                if current_iteration > 2000:
+                    current_iteration -= 2000
+                elif current_iteration > 1000:
+                    current_iteration -= 100
+                else:
+                    current_iteration = 1
+                bar(
+                    (radius - current_iteration) / radius
+                    if current_iteration != 1
+                    else 1
                 )
 
-        snap_ids.extend(self.arg_snaps)
+        return found_snaps
 
-        # Download Snaps provided from the command line
-        self.download_snaps(self.query_snaps(snap_ids))
-
-        if self.write_json:
-            with open(
-                os.path.join(
-                    self.output_dir, f"archive_{int(datetime.now().timestamp())}.json"
-                ),
-                "w",
-            ) as f:
-                json.dump(
-                    list(self.all_snaps.values()),
-                    f,
-                    indent=2,
-                    cls=SnapJSONEncoder,
-                )
+    def _coordinate_query_failure(self, msg: str, sleep_seconds: int = 60):
+        self.logger.warning(f"{msg} Sleeping for [{sleep_seconds}] seconds...")
+        sleep(sleep_seconds)
 
     def _parse_snap(
         self,
         snap: dict[
             str, t.Any
         ],  # I don't like the Any type but this dict is so dynamic there isn't much point hinting it accurately.
     ) -> Snap | None:
-        if self.all_snaps.get(snap["id"]):
-            return self.all_snaps[snap["id"]]
+        if self.snap_cache.get(snap["id"]):
+            return self.snap_cache[snap["id"]]
 
         file_type = (
             "mp4"
             if snap["snapInfo"].get("snapMediaType")
             else "jpg"
             if snap["snapInfo"].get("streamingMediaInfo")
             else "UNKNOWN"
         )
 
         url: str | None = snap["snapInfo"]["streamingMediaInfo"].get("mediaUrl")
         if not url:
-            print(f'Media URL for snap [{snap["id"]}] could not be determined.')
+            self.logger.warning(
+                f'Media URL for snap [{snap["id"]}] could not be determined.'
+            )
             return None
 
         create_time = round(int(snap["timestamp"]) * 10**-3, 3)
 
         if (self.since_time) and (create_time < self.since_time):
-            print(
+            self.logger.debug(
                 f" - [{snap['id']}] is older than the specified time of [{self.since_time}]. Snap timestamp: [{int(create_time)}]. Skipping."
             )
             return None
 
-        s = Snap(
+        parsed_snap = Snap(
             create_time=create_time,  # type: ignore
             snap_id=snap["id"],
             url=url,
             file_type=file_type,
             location=snap["snapInfo"]
             .get("title", {})
             .get(
                 "fallback",
                 snap["snapInfo"].get("localitySubtitle", {}).get("fallback", "UNKNOWN"),
             ),
         )
 
-        self.all_snaps[snap["id"]] = s
+        self.snap_cache[snap["id"]] = parsed_snap
 
-        return s
+        return parsed_snap
 
     def _get_epoch(self):
         epoch_endpoint = requests.post(
             "https://ms.sc-jpl.com/web/getLatestTileSet",
             headers={"Content-Type": "application/json"},
             json={},
         ).json()
```

### Comparing `snapmap_archiver-2.2.0/snapmap_archiver/time.py` & `snapmap_archiver-2.3.0/snapmap_archiver/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 def since_epoch(since_time: str) -> int:
     if since_time.isdigit():
         return int(since_time)
 
     num = int(since_time[:-1])
-    if since_time[-1] == "m":
-        return int(datetime.now().timestamp()) - num * 60
-    if since_time[-1] == "h":
-        return int(datetime.now().timestamp()) - num * 60 * 60
-    if since_time[-1] == "d":
-        return int(datetime.now().timestamp()) - num * 60 * 60 * 24
+    match since_time[-1]:
+        case "m":
+            return int(datetime.now().timestamp()) - num * 60
+        case "h":
+            return int(datetime.now().timestamp()) - num * 60 * 60
+        case "d":
+            return int(datetime.now().timestamp()) - num * 60 * 60 * 24
     raise ValueError(f"Invalid time filter: [{since_time}]")
```

### Comparing `snapmap_archiver-2.2.0/setup.py` & `snapmap_archiver-2.3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 packages = \
 ['snapmap_archiver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.25.1,<3.0.0']
+['aiofiles>=23.2.1,<24.0.0',
+ 'alive-progress>=3.1.5,<4.0.0',
+ 'httpx>=0.27.0,<0.28.0',
+ 'loguru>=0.7.2,<0.8.0',
+ 'requests>=2.25.1,<3.0.0']
 
 entry_points = \
-{'console_scripts': ['snapmap-archiver = snapmap_archiver:main']}
+{'console_scripts': ['snapmap-archiver = snapmap_archiver.__main__:main']}
 
 setup_kwargs = {
     'name': 'snapmap-archiver',
-    'version': '2.2.0',
+    'version': '2.3.0',
     'description': 'Download all Snap Map content from a specific location.',
-    'long_description': '# snapmap-archiver\n\nA tool written in Python **3.10** to download all Snapmaps content from a specific location.\n\n## Install Python 3.10+\n\nBe sure to check that you\'re using a version of Python that is 3.10 or above. **This project will not work on Python 3.9 or below!**\n\n![snapmap-archiver splash](/.github/img/Splash.png)\n\n`pip install snapmap-archiver`\n\n[View on PyPI](https://pypi.org/project/snapmap-archiver/)\n\n## Setup (for working in a Python environment)\n\nInstall dependencies with `pip`.\n\n```sh\npip install -r requirements.txt\n```\n\n## Usage\n\n```sh\nsnapmap-archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"\n```\n\nUnfortunately you have to use the arbitrary `-l="lat,lon"` rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.\n\n### Optional Arguments\n\n#### Location\n\n`-l` is not required if an input file or Snap URL is provided. It can also be used multiple times to download Snaps from multiple locations in one command.\n\nE.g\n\n```sh\nsnapmap-archiver -o ~/Desktop/snap -l=\'123.123,123.123\' -l \'445.445,445.445\'\n```\n\n#### Input File\n\nWith `-f` or `--file`, you can specify a file containing a list of line-separated Snap URLs or IDs.\n\nE.g\n\n```sh\nsnapmap-archiver -o ~/Desktop/snaps -f ~/Desktop/snaps.txt\n```\n\nInside `snaps.txt`:\n\n```\nhttps://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z\nExample\nhttps://map.snapchat.com/ttp/snap/Example/\nhttps://map.snapchat.com/ttp/snap/Example/\n```\n\n#### Snap URL\n\nYou can also just pass 1 or more normal Snap URLs or IDs to the package to download it individually like this:\n\n```sh\nsnapmap-archiver -o ~/Desktop/snap \'https://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z\' \'Example\'\n```\n\n#### Export JSON\n\nYou can export a JSON file with info about downloaded snaps with the `--write-json` argument, which will contain information like the time the Snap was posted, and the Snap location.\n\nIt will write `archive.json` to the specified output directory.\n\n#### Snap Radius\n\nThe radius from the coordinates you provide that will be included for downloads. `-r 20000` will download all Snaps within a 20km radius of your coordinates.\n',
+    'long_description': '# snapmap-archiver\n\nDownload all Snap Map content from a specific location.\n\n![snapmap-archiver splash](/.github/img/Splash.png)\n\n[View on PyPI](https://pypi.org/project/snapmap-archiver/)\n\n## Installation (for general usage)\n\nInstall with `pip` or `pipx` or whatever trendy Python package manager you use:\n\n```sh\npip install snapmap-archiver\n```\n\n## Local Development Setup\n\nInstall Poetry with `pip` or `pipx`:\n\n```sh\npip install poetry\n```\n\nInstall the project dependencies:\n\n```sh\npoetry install\n```\n\nRun the app with Poetry:\n\n```sh\npoetry run python3 main.py [...args]\n```\n\n## Usage\n\n```sh\nsnapmap-archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"\n```\n\nUnfortunately you have to use the arbitrary `-l="lat,lon"` (with the equals sign) rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.\n\n### Optional Arguments\n\n#### Location\n\n`-l` is not required if an input file or Snap URL is provided. It can also be used multiple times to download Snaps from multiple locations in one command.\n\nE.g\n\n```sh\nsnapmap-archiver -o ~/Desktop/snap -l=\'123.123,123.123\' -l \'445.445,445.445\'\n```\n\n#### Input File\n\nWith `-f` or `--file`, you can specify a file containing a list of line-separated Snap URLs or IDs.\n\nE.g\n\n```sh\nsnapmap-archiver -o ~/Desktop/snaps -f ~/Desktop/snaps.txt\n```\n\nInside `snaps.txt`:\n\n```\nhttps://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z\nExample\nhttps://map.snapchat.com/ttp/snap/Example/\nhttps://map.snapchat.com/ttp/snap/Example/\n```\n\n#### Snap URL\n\nYou can also just pass 1 or more normal Snap URLs or IDs to the package to download it individually like this:\n\n```sh\nsnapmap-archiver -o ~/Desktop/snap \'https://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z\' \'Example\'\n```\n\n#### Time Filter\n\nUse the `-t` flag with a Unix timestamp or day, hour, or minute interval to skip the download of any snaps older than that point.\n\nExample with a Unix timestamp:\n\n```sh\nsnapmap-archiver -t 1714392291 -l \'-123,123\'\n```\n\nExamples with a dynamic time filter:\n\n```sh\nsnapmap-archiver -t 3d -l=\'-123,123\'  # Removes anything older than 3 days\nsnapmap-archiver -t 5h -l=\'-123,123\'  # Removes anything older than 5 hours\nsnapmap-archiver -t 30m -l=\'-123,123\'  # Removes anything older than 30 minutes\n```\n\n#### Export JSON\n\nYou can export a JSON file with info about downloaded snaps with the `--write-json` argument, which will contain information like the time the Snap was posted, and the Snap location.\n\nIt will write `archive.json` to the specified output directory.\n\n#### Snap Radius\n\nThe radius from the coordinates you provide that will be included for downloads. `-r 20000` will download all Snaps within a 20km radius of your coordinates.\n\n#### Zoom Depth\n\nYou can input a custom zoom depth value (`-z`) that correlates to a zoom level in the GUI. ArcGIS has documentation about this [here](https://developers.arcgis.com/documentation/glossary/zoom-level/), but essentially the lower the number, the further zoomed-out you are. `5` is the default and shouldn\'t cause any issues.\n\n#### Debug Mode\n\nEnable debug logs with `-d`/`--debug`.\n',
     'author': 'Miles Greenwark',
     'author_email': 'Millez.Dev@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `snapmap_archiver-2.2.0/PKG-INFO` & `snapmap_archiver-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 Metadata-Version: 2.1
 Name: snapmap-archiver
-Version: 2.2.0
+Version: 2.3.0
 Summary: Download all Snap Map content from a specific location.
 License: GPL-3.0-or-later
 Author: Miles Greenwark
 Author-email: Millez.Dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # snapmap-archiver
 
-A tool written in Python **3.10** to download all Snapmaps content from a specific location.
+Download all Snap Map content from a specific location.
 
-## Install Python 3.10+
+![snapmap-archiver splash](/.github/img/Splash.png)
 
-Be sure to check that you're using a version of Python that is 3.10 or above. **This project will not work on Python 3.9 or below!**
+[View on PyPI](https://pypi.org/project/snapmap-archiver/)
 
-![snapmap-archiver splash](/.github/img/Splash.png)
+## Installation (for general usage)
 
-`pip install snapmap-archiver`
+Install with `pip` or `pipx` or whatever trendy Python package manager you use:
 
-[View on PyPI](https://pypi.org/project/snapmap-archiver/)
+```sh
+pip install snapmap-archiver
+```
+
+## Local Development Setup
 
-## Setup (for working in a Python environment)
+Install Poetry with `pip` or `pipx`:
+
+```sh
+pip install poetry
+```
+
+Install the project dependencies:
+
+```sh
+poetry install
+```
 
-Install dependencies with `pip`.
+Run the app with Poetry:
 
 ```sh
-pip install -r requirements.txt
+poetry run python3 main.py [...args]
 ```
 
 ## Usage
 
 ```sh
 snapmap-archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"
 ```
 
-Unfortunately you have to use the arbitrary `-l="lat,lon"` rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.
+Unfortunately you have to use the arbitrary `-l="lat,lon"` (with the equals sign) rather than just `-l "lat,lon"` when parsing negative numbers as `argsparse` interprets said numbers as extra arguments.
 
 ### Optional Arguments
 
 #### Location
 
 `-l` is not required if an input file or Snap URL is provided. It can also be used multiple times to download Snaps from multiple locations in one command.
 
@@ -78,17 +96,43 @@
 
 You can also just pass 1 or more normal Snap URLs or IDs to the package to download it individually like this:
 
 ```sh
 snapmap-archiver -o ~/Desktop/snap 'https://map.snapchat.com/ttp/snap/Example/@-33.643495,115.741281,11.86z' 'Example'
 ```
 
+#### Time Filter
+
+Use the `-t` flag with a Unix timestamp or day, hour, or minute interval to skip the download of any snaps older than that point.
+
+Example with a Unix timestamp:
+
+```sh
+snapmap-archiver -t 1714392291 -l '-123,123'
+```
+
+Examples with a dynamic time filter:
+
+```sh
+snapmap-archiver -t 3d -l='-123,123'  # Removes anything older than 3 days
+snapmap-archiver -t 5h -l='-123,123'  # Removes anything older than 5 hours
+snapmap-archiver -t 30m -l='-123,123'  # Removes anything older than 30 minutes
+```
+
 #### Export JSON
 
 You can export a JSON file with info about downloaded snaps with the `--write-json` argument, which will contain information like the time the Snap was posted, and the Snap location.
 
 It will write `archive.json` to the specified output directory.
 
 #### Snap Radius
 
 The radius from the coordinates you provide that will be included for downloads. `-r 20000` will download all Snaps within a 20km radius of your coordinates.
 
+#### Zoom Depth
+
+You can input a custom zoom depth value (`-z`) that correlates to a zoom level in the GUI. ArcGIS has documentation about this [here](https://developers.arcgis.com/documentation/glossary/zoom-level/), but essentially the lower the number, the further zoomed-out you are. `5` is the default and shouldn't cause any issues.
+
+#### Debug Mode
+
+Enable debug logs with `-d`/`--debug`.
+
```

