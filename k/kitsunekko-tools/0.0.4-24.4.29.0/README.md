# Comparing `tmp/kitsunekko_tools-0.0.4.tar.gz` & `tmp/kitsunekko_tools-24.4.29.0.tar.gz`

## Comparing `kitsunekko_tools-0.0.4.tar` & `kitsunekko_tools-24.4.29.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.github/workflows/black.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/__init__.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/__version__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/common.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/config.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/consts.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/download.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/ignore.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/kitsunekko_tools/mega_upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    41751 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/format.sh
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/__main__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/__version__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/common.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/config.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/consts.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/ignore.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/kitsu_download.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/kitsu_parse.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/kitsu_types.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/kitsunekko_tools/mega_upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/tests/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/tests/test_parser.py
+-rw-r--r--   0        0        0   663796 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/tests/data/main_dir_page.html
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/tests/data/subs_page.html
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/LICENSE
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/pyproject.toml
+-rw-r--r--   0        0        0    42071 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.29.0/PKG-INFO
```

### Comparing `kitsunekko_tools-0.0.4/.github/ISSUE_TEMPLATE/config.yml` & `kitsunekko_tools-24.4.29.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.4/.github/workflows/ci-cd.yml` & `kitsunekko_tools-24.4.29.0/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.4/kitsunekko_tools/__main__.py` & `kitsunekko_tools-24.4.29.0/kitsunekko_tools/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
+import sys
 
 import fire
 
+from kitsunekko_tools.__version__ import __version__
 from kitsunekko_tools.common import KitsuException
-from kitsunekko_tools.config import ConfigFileNotFoundError, KitsuConfig, get_config
-from kitsunekko_tools.download import Sync
+from kitsunekko_tools.config import ConfigFileNotFoundError, Config
+from kitsunekko_tools.consts import PROG_NAME
 from kitsunekko_tools.ignore import IgnoreList, IgnoreListException
+from kitsunekko_tools.kitsu_download import Sync
 from kitsunekko_tools.mega_upload import mega_upload
 
 
 class ConfigCli:
     """
-    Manage config file.
+    Manage config.
     """
 
-    @staticmethod
-    def create() -> None:
+    _config: Config
+
+    def __init__(self, config: Config):
+        self._config = config
+
+    def create(self) -> None:
         """
-        Create an example config file in the default location, if it does not exist.
+        Create an example config file in the default or user-specified location, if it does not exist.
         """
         try:
-            data, location = get_config()
+            location = self._config.file_path()
         except ConfigFileNotFoundError:
-            config_file_path = KitsuConfig.default_location()
-            config_file_path.parent.mkdir(exist_ok=True, parents=True)
-            config_file_path.write_text(KitsuConfig().as_toml_str())
-            print(f"Created config file: {config_file_path}")
+            location = self._config.create_config_file()
+            print(f"Created config file: {location}")
         else:
             print(f"File already exists: {location}")
 
-    @staticmethod
-    def locate() -> None:
+    def locate(self) -> None:
         """
         Print path to the config file, if it exists.
         """
         try:
-            data, location = get_config()
+            location = self._config.file_path()
         except ConfigFileNotFoundError as ex:
             print(ex.what)
         else:
             print(location)
 
-    @staticmethod
-    def show() -> None:
+    def show(self) -> None:
         """
         Show the content of the config file, if it exists.
         """
         try:
-            data, location = get_config()
+            data = self._config.data()
         except ConfigFileNotFoundError as ex:
             print(ex.what)
         else:
             print(data.as_toml_str())
 
 
 class IgnoreCli:
@@ -77,79 +80,98 @@
 
     def add(self, pattern: str) -> None:
         """
         Add a new ignore rule.
         """
         if pattern:
             self._ignore_list.add(str(pattern))
+            self._ignore_list.commit()
             print(f"File written: {self._ignore_list.path()}")
         else:
             print("Nothing to add.")
 
 
 class Application:
     """
     A set of scripts for creating a local kitsunekko mirror.
+
+    :param version: Print version and exit.
+    :param config_path: Alternative path to the config file.
     """
 
+    def __init__(self, version: bool = False, config_path: str | None = None):
+        self._config = Config(config_path)
+        if version:
+            # handle ktools --version
+            sys.exit(self.version())
+
     @staticmethod
-    def config() -> ConfigCli:
+    def version() -> None:
         """
-        Manage config file.
+        Print version and exit.
         """
-        return ConfigCli()
+        print(f"{PROG_NAME} version: {__version__}")
 
-    @staticmethod
-    def destination() -> None:
+    def config(self) -> ConfigCli:
+        """
+        Manage config.
+        """
+        try:
+            return ConfigCli(self._config)
+        except IgnoreListException as ex:
+            print(ex.what)
+
+    def destination(self) -> None:
         """
         Print path to destination directory.
         """
         try:
-            data, location = get_config()
+            data = self._config.data()
         except ConfigFileNotFoundError as ex:
             print(ex.what)
         else:
             print(data.destination)
 
-    @staticmethod
-    def ignore():
+    def ignore(self) -> IgnoreCli:
         """
         Manage the list of ignore patterns.
         """
         try:
-            return IgnoreCli(IgnoreList())
+            return IgnoreCli(IgnoreList(self._config.data()))
         except IgnoreListException as ex:
             print(ex.what)
 
-    @staticmethod
-    async def sync():
+    async def sync(self, full: bool = False) -> None:
         """
         Download everything from Kitsunekko to a local folder.
+
+        :param full: Do a full sync. Ignore the 'skip_older' setting.
         """
         try:
-            s = Sync()
+            s = Sync(config=self._config.data(), full_sync=full)
         except KitsuException as ex:
             print(ex.what)
         else:
             await s.sync_all()
 
-    @staticmethod
-    def upload():
+    def upload(self):
         """
         Upload the local folder to mega.nz.
         The ~/.megarc file must exist.
         """
         try:
-            mega_upload(get_config().data)
+            mega_upload(self._config.data())
         except KitsuException as ex:
             print(ex.what)
 
 
 def main() -> None:
     try:
         fire.Fire(Application)
+    except KitsuException as ex:
+        print(ex.what)
     except KeyboardInterrupt:
-        print("Aborted by the user.")
+        print("\nAborted by the user.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `kitsunekko_tools-0.0.4/kitsunekko_tools/download.py` & `kitsunekko_tools-24.4.29.0/kitsunekko_tools/kitsu_download.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
 
 import asyncio
 import dataclasses
+import datetime
 import enum
-import os.path
 import pathlib
 import re
 import typing
-from datetime import datetime
-from urllib.parse import unquote
+from collections.abc import Sequence
 
 import httpx
 
 from kitsunekko_tools.common import KitsuException
-from kitsunekko_tools.config import get_config
-from kitsunekko_tools.consts import *
+from kitsunekko_tools.config import KitsuConfig
 from kitsunekko_tools.ignore import IgnoreList
+from kitsunekko_tools.kitsu_parse import find_all_subtitle_dirs, find_all_subtitle_files
+from kitsunekko_tools.kitsu_types import AnimeDir, SubtitleFile
 
 
 def is_file_non_empty(file_path: pathlib.Path) -> bool:
     """
     Returns True if file exists and is not empty.
     """
     return file_path.is_file() and file_path.stat().st_size > 0
 
 
-@dataclasses.dataclass(frozen=True)
-class AnimeSubtitleUrl:
-    url: str
-    title: str
-
-    @property
-    def file_name(self) -> str:
-        return unquote(self.url).split("/")[-1]
-
+class PageCrawlResult(typing.NamedTuple):
+    visited_dir: AnimeDir
+    found_dirs: list[AnimeDir]
+    found_files: list[SubtitleFile]
 
-AnimeDirUrl = typing.NewType("AnimeDirUrl", str)
+    def __str__(self) -> str:
+        return str(
+            f"visited page {self.visited_dir.url}. "
+            f"found {len(self.found_files)} files. "
+            f"found {len(self.found_dirs)} directories."
+        )
 
 
-@dataclasses.dataclass(frozen=True)
-class FetchResult:
-    to_visit: set[AnimeDirUrl]
-    to_download: set[AnimeSubtitleUrl]
+@dataclasses.dataclass
+class LocalSubtitleFile:
+    remote: SubtitleFile  # remote URL
+    file_path: pathlib.Path  # path to the file on the hard drive
+
+    def __init__(self, remote: SubtitleFile, config: KitsuConfig):
+        self.remote = remote
+        self.file_path = config.destination / remote.show_name / remote.file_name
 
-    @classmethod
-    def new(cls):
-        return cls(to_visit=set(), to_download=set())
+    def ensure_subtitle_dir(self) -> None:
+        """
+        Create directory to store the subtitle file.
+        """
+        return self.file_path.parent.mkdir(exist_ok=True)
 
-    def update(self, other: "FetchResult"):
-        self.to_visit.update(other.to_visit)
-        self.to_download.update(other.to_download)
+    def is_already_downloaded(self) -> bool:
+        return is_file_non_empty(self.file_path)
 
 
 class DownloadStatus(enum.Enum):
     already_exists = enum.auto()
     explicitly_ignored = enum.auto()
     download_failed = enum.auto()
     saved = enum.auto()
@@ -62,30 +67,63 @@
     def __str__(self) -> str:
         return self.name.replace("_", " ")
 
 
 @dataclasses.dataclass(frozen=True)
 class DownloadResult:
     reason: DownloadStatus
-    file_path: pathlib.Path
+    subtitle: LocalSubtitleFile
+    status_code: int = 0
 
     def __repr__(self):
-        return f"{self.reason}: {self.file_path}"
+        if self.reason == DownloadStatus.download_failed:
+            return f"{self.reason} with status {self.status_code}: {self.subtitle.remote.url}"
+        return f"{self.reason}: {self.subtitle.remote.url}"
+
+    def is_successful(self) -> bool:
+        return self.reason == DownloadStatus.already_exists or self.reason == DownloadStatus.saved
+
+
+@dataclasses.dataclass(frozen=True)
+class FetchResult:
+    to_visit: set[AnimeDir]
+    to_download: set[SubtitleFile]
+    visited: set[AnimeDir]
+    saved: set[LocalSubtitleFile]
+    failed: set[LocalSubtitleFile]
+
+    @classmethod
+    def new(cls):
+        return cls(to_visit=set(), to_download=set(), visited=set(), saved=set(), failed=set())
+
+    def update(self, dir_result: PageCrawlResult, downloads: Sequence[DownloadResult]):
+        self.to_visit.update(dir_result.found_dirs)
+        self.to_download.update(dir_result.found_files)
+        self.visited.add(dir_result.visited_dir)
+        self.saved.update(f.subtitle for f in downloads if f.reason == DownloadStatus.saved)
+        self.failed.update(f.subtitle for f in downloads if f.reason == DownloadStatus.download_failed)
+
+    def __str__(self) -> str:
+        return str(
+            f"visited {len(self.visited)} pages. "
+            f"saved {len(self.saved)} files. "
+            f"failed {len(self.failed)} files."
+        )
 
 
 @dataclasses.dataclass(frozen=True)
 class FetchState:
-    to_visit: set[AnimeDirUrl]
-    visited: set[AnimeDirUrl]
+    to_visit: set[AnimeDir]
+    visited: set[AnimeDir]
 
     @classmethod
-    def new(cls, download_root: AnimeDirUrl) -> typing.Self:
+    def new(cls, download_root_url: str) -> typing.Self:
         return cls(
             to_visit={
-                download_root,
+                AnimeDir(download_root_url, "subtitles", datetime.datetime.now()),
             },
             visited=set(),
         )
 
     def balance(self, prev_result: FetchResult) -> None:
         self.visited.update(self.to_visit)
         self.to_visit.clear()
@@ -106,108 +144,111 @@
 
 def get_anime_title(page_text: str) -> str:
     title = re.search(r"<title>([^<>]+)</title>", page_text, flags=re.IGNORECASE | re.MULTILINE).group(1)
     title = title.replace(" - Japanese subtitles - kitsunekko.net", "").replace("/", " ").replace("\\", " ")
     return title.strip()
 
 
-def find_all_subtitle_dir_urls(html_text: str) -> list[str]:
-    return re.findall(r'(?<="/)dirlist.php\?[^"\']+(?=")', html_text)
-
-
-def find_all_subtitle_file_urls(html_text: str) -> list[str]:
-    return re.findall(r'(?<=href=")subtitles/[^"\']+\.(?:zip|rar|ass|srt)(?=")', html_text)
-
-
-async def crawl_page(client: httpx.AsyncClient, url: str) -> FetchResult:
-    try:
-        r = await client.get(url)
-    except Exception as e:
-        raise DownloadError(url) from e
-
-    return FetchResult(
-        to_visit={
-            AnimeDirUrl(f"{KITSUNEKKO_DOMAIN_URL}/{anime_dir}") for anime_dir in find_all_subtitle_dir_urls(r.text)
-        },
-        to_download={
-            AnimeSubtitleUrl(f"{KITSUNEKKO_DOMAIN_URL}/{subtitle}", get_anime_title(r.text))
-            for subtitle in find_all_subtitle_file_urls(r.text)
-        },
+def get_http_client(config: KitsuConfig):
+    return httpx.AsyncClient(
+        proxies=config.proxy,
+        headers=config.headers,
+        timeout=config.timeout,
+        follow_redirects=False,
     )
 
 
-async def find_subs_all(client: httpx.AsyncClient, to_visit: set[str]) -> FetchResult:
-    result = FetchResult.new()
-    for fut in asyncio.as_completed([crawl_page(client, page) for page in to_visit]):
-        try:
-            result.update(await fut)
-        except DownloadError as e:
-            print(f"got {e.what} while trying to download {e.url}")
-    return result
-
-
-class AnimeSubtitleFile:
-    def __init__(self, remote: AnimeSubtitleUrl, root_dir_path: pathlib.Path):
-        self.dir_path = root_dir_path / remote.title
-        self.file_path = self.dir_path / remote.file_name
-        self.remote_url = remote.url
-
-    def ensure_subtitle_dir(self) -> None:
-        """
-        Create directory to store the subtitle file.
-        """
-        return self.dir_path.mkdir(exist_ok=True)
-
-    def is_already_downloaded(self) -> bool:
-        return is_file_non_empty(self.file_path)
-
-
 class Sync:
-    def __init__(self):
-        self._config = get_config().data
-        self._ignore = IgnoreList(self._config)
-        self._config.raise_for_destination()
+    _config: KitsuConfig
+    _ignore: IgnoreList
+    _now: datetime
+    _full_sync: bool
 
-    async def download_sub(self, client: httpx.AsyncClient, subtitle: AnimeSubtitleFile) -> DownloadResult:
-        subtitle.ensure_subtitle_dir()
+    def __init__(self, config: KitsuConfig, full_sync: bool = False):
+        self._config = config
+        self._config.raise_for_destination()
+        self._ignore = IgnoreList(self._config)
+        self._now = datetime.datetime.now()
+        self._full_sync = full_sync
 
+    async def download_sub(self, client: httpx.AsyncClient, subtitle: LocalSubtitleFile) -> DownloadResult:
         if subtitle.is_already_downloaded():
-            return DownloadResult(DownloadStatus.already_exists, subtitle.file_path)
+            return DownloadResult(DownloadStatus.already_exists, subtitle)
 
         if self._ignore.is_matching(subtitle.file_path):
-            return DownloadResult(DownloadStatus.explicitly_ignored, subtitle.file_path)
+            return DownloadResult(DownloadStatus.explicitly_ignored, subtitle)
 
         try:
-            r = await client.get(subtitle.remote_url)
+            r = await client.get(subtitle.remote.url)
         except Exception as e:
-            raise DownloadError(subtitle.remote_url) from e
+            raise DownloadError(subtitle.remote.url) from e
+
         if r.status_code != httpx.codes.OK:
-            return DownloadResult(DownloadStatus.download_failed, subtitle.file_path)
+            return DownloadResult(DownloadStatus.download_failed, subtitle, r.status_code)
+
+        subtitle.ensure_subtitle_dir()
+        print(f"downloading file: {subtitle.remote.url}")
         with open(subtitle.file_path, "wb") as f:
             f.write(r.content)
-        return DownloadResult(DownloadStatus.saved, subtitle.file_path)
+        return DownloadResult(DownloadStatus.saved, subtitle, r.status_code)
+
+    async def download_subs(
+        self, client: httpx.AsyncClient, to_download: Sequence[SubtitleFile]
+    ) -> Sequence[DownloadResult]:
+        tasks = tuple(self.download_sub(client, LocalSubtitleFile(sub, self._config)) for sub in to_download)
+        results = []
+        for fut in asyncio.as_completed(tasks):
+            try:
+                result = await fut
+            except DownloadError as ex:
+                print(f"got {ex.what} while trying to download {ex.url}")
+            else:
+                print(result)
+                if result.is_successful():
+                    # this file will not be downloaded again even if it is moved later.
+                    self._ignore.add_file(result.subtitle.file_path)
+                self._ignore.maybe_commit_midway()
+                results.append(result)
+        return results
+
+    def _should_visit(self, location: AnimeDir | SubtitleFile) -> bool:
+        """
+        The page is visited if it was modified recently enough.
+        On full sync, visit and download everything.
+        """
+        if self._full_sync:
+            return True
+        return location.mod_timestamp >= (self._now - self._config.skip_older)
+
+    async def crawl_page(self, client: httpx.AsyncClient, anime_dir: AnimeDir) -> PageCrawlResult:
+        try:
+            r = await client.get(anime_dir.url)
+        except Exception as e:
+            raise DownloadError(anime_dir.url) from e
+
+        return PageCrawlResult(
+            visited_dir=anime_dir,
+            found_dirs=[*filter(self._should_visit, find_all_subtitle_dirs(r.text))],
+            found_files=[*filter(self._should_visit, find_all_subtitle_files(r.text))],
+        )
 
-    async def download_subs(self, client: httpx.AsyncClient, to_download: typing.Iterable[AnimeSubtitleFile]) -> None:
-        for fut in asyncio.as_completed(tuple(self.download_sub(client, subtitle) for subtitle in to_download)):
+    async def find_subs_all(self, client: httpx.AsyncClient, to_visit: set[AnimeDir]) -> FetchResult:
+        results = FetchResult.new()
+        for fut in asyncio.as_completed([self.crawl_page(client, page) for page in to_visit]):
             try:
-                print(await fut)
-            except DownloadError as e:
-                print(f"got {e.what} while trying to download {e.url}")
+                page_visit: PageCrawlResult = await fut
+            except DownloadError as ex:
+                print(f"got {ex.what} while trying to download {ex.url}")
+            else:
+                print(page_visit)
+                downloads = await self.download_subs(client, page_visit.found_files)
+                results.update(page_visit, downloads)
+        return results
 
     async def sync_all(self) -> None:
-        async with httpx.AsyncClient(
-            proxies=self._config.proxy,
-            headers=self._config.headers,
-            timeout=self._config.timeout,
-        ) as client:
-            state = FetchState.new(AnimeDirUrl(self._config.download_root))
+        async with get_http_client(self._config) as client:
+            state = FetchState.new(self._config.download_root)
             while state.has_unvisited():
-                task: FetchResult = await find_subs_all(client, state.to_visit)
-                print(f"visited {len(state.to_visit)} pages, found {len(task.to_download)} files.")
-                await self.download_subs(
-                    client,
-                    (AnimeSubtitleFile(url, self._config.destination) for url in task.to_download),
-                )
+                task: FetchResult = await self.find_subs_all(client, state.to_visit)
+                print(task)
                 state.balance(task)
-
-        with open(os.path.join(self._config.destination, UPDATED_FILENAME), "w") as of:
-            of.write(datetime.utcnow().strftime("%c"))
+        self._ignore.commit()
```

### Comparing `kitsunekko_tools-0.0.4/kitsunekko_tools/ignore.py` & `kitsunekko_tools-24.4.29.0/kitsunekko_tools/ignore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,96 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
 
 import dataclasses
 import fnmatch
-import os.path
 import pathlib
-import sys
 import typing
 
 from kitsunekko_tools.common import KitsuException
-from kitsunekko_tools.config import get_config, KitsuConfig
+from kitsunekko_tools.config import KitsuConfig, get_config
 from kitsunekko_tools.consts import *
 
 
 @dataclasses.dataclass
 class IgnoreListException(KitsuException):
     what: str
 
 
 class IgnoreList:
+    """
+    Holds a list of files that should not be downloaded even if they're not present in expected locations.
+    """
+
     _config: KitsuConfig
     _ignore_filepath: pathlib.Path
-    _patterns: set[str]
+    _patterns: dict[str, None]
+    _dirty_level: int  # counts additions
+    _autocommit_threshold: int
 
-    def __init__(self, config: KitsuConfig | None = None):
-        self._config = config or get_config().data
+    def __init__(self, config: KitsuConfig, autocommit_threshold: int = 20):
+        self._config = config
         self._ignore_filepath = pathlib.Path(self._config.destination) / IGNORE_FILENAME
-        self._patterns = set()
+        self._patterns = {}
+        self._dirty_level = 0
+        self._autocommit_threshold = autocommit_threshold
         self._config.raise_for_destination()
         try:
             with open(self._ignore_filepath, encoding="utf8") as f:
-                self._patterns.update(filter(bool, map(str.strip, f.read().splitlines())))
+                self._patterns.update(dict.fromkeys(filter(bool, map(str.strip, f.read().splitlines()))))
         except FileNotFoundError:
             pass
 
     @property
     def ignore_filepath(self) -> pathlib.Path:
         return self._ignore_filepath
 
+    def _pattern_from_path(self, file_path: pathlib.Path) -> str:
+        return str(file_path.relative_to(self._config.destination))
+
     def is_matching(self, file_path: pathlib.Path) -> bool:
-        path_dest_stripped = str(file_path.relative_to(self._config.destination))
+        path_dest_stripped = self._pattern_from_path(file_path)
         if path_dest_stripped in self._patterns:
             # try without wildcards first.
             return True
         return any(fnmatch.fnmatch(path_dest_stripped, pattern) for pattern in self._patterns)
 
-    def patterns(self) -> set[str]:
+    def patterns(self) -> typing.Iterable[str]:
         """
         Return all known ignore patterns.
         """
-        return self._patterns
+        return self._patterns.keys()
 
-    def add(self, pattern: str):
+    def add(self, pattern: str) -> None:
         """
         Add a new ignore pattern to the list.
         """
-        self._patterns.add(pattern)
-        self._ignore_filepath.write_text("\n".join(sorted(self._patterns)))
+        self._patterns[pattern] = None
+        self._dirty_level += 1
+
+    def add_file(self, file_path: pathlib.Path) -> None:
+        """
+        Add file to the list, as relative path.
+        """
+        return self.add(self._pattern_from_path(file_path))
 
     def path(self) -> pathlib.Path:
         """
         Return path to ignore file.
         """
         return self._ignore_filepath
+
+    def commit(self) -> None:
+        """
+        Save ignore file to disk.
+        """
+        if self._dirty_level == 0:
+            return
+        self._ignore_filepath.write_text("\n".join(self._patterns) + "\n")  # newline at the end of file
+        self._dirty_level = 0
+
+    def maybe_commit_midway(self) -> None:
+        """
+        Save file to disk if its dirty level exceeds the set limit.
+        """
+        if self._dirty_level >= self._autocommit_threshold:
+            self.commit()
```

### Comparing `kitsunekko_tools-0.0.4/kitsunekko_tools/mega_upload.py` & `kitsunekko_tools-24.4.29.0/kitsunekko_tools/mega_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     remote_destination = f"/Root/{config.destination.name}"
     print(f"Remote destination: {remote_destination}")
 
     subprocess.run(  # will return 1 if directory already exists.
         args=("megamkdir", remote_destination),
         stdout=sys.stdout,
         stderr=sys.stderr,
+        check=False,
     )
 
     out = subprocess.run(
         args=("megacopy", "--local", config.destination, "--remote", remote_destination, "--no-follow"),
         stdout=sys.stdout,
         stderr=sys.stderr,
+        check=False,
     )
     raise_for_status(out)
```

### Comparing `kitsunekko_tools-0.0.4/LICENSE` & `kitsunekko_tools-24.4.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.4/README.md` & `kitsunekko_tools-24.4.29.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,27 +24,38 @@
 ktools config create
 ```
 
 Edit the config file.
 
  * `destination` - the local folder where the files should be downloaded.
  * `proxy` - Your proxy settings.
-   Set to `null` if you don't use proxies.
+   Set to `""` (empty string) if you don't use proxies.
    By default, it is set to the default Tor address.
 
 Everything else usually doesn't need to be changed.
 
 ## Usage
 
+The first time, run full sync.
+It will download everything.
+
+``` bash
+ktools sync --full
+```
+
 Run sync.
+If you already have downloaded everything once,
+this command will skip files that have not been modified recently.
 
 ``` bash
 ktools sync
 ```
 
+The `skip_older` config parameter controls what files should be skipped during regular runs.
+
 ## Upload your mirror to Mega
 
 1) Install [megatools](https://archlinux.org/packages/extra/x86_64/megatools/).
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
 
 ## Ignoring certain files
```

### Comparing `kitsunekko_tools-0.0.4/pyproject.toml` & `kitsunekko_tools-24.4.29.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 readme = "README.md"
 dynamic = ["version"]
 authors = [
   { name = "Ren Tatsumoto", email = "tatsu@autistici.org" },
 ]
 dependencies = [
   "httpx[socks]>=0.27",
-  "fire>=0.6.0"
+  "fire>=0.6.0",
 ]
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 
 [project.scripts]
 ktools = "kitsunekko_tools.__main__:main"
 
@@ -30,10 +30,15 @@
 [tool.hatch.version]
 source = "vcs"
 path = "kitsunekko_tools/__version__.py"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "kitsunekko_tools/__version__.py"
 
+[tool.hatch.envs.test]
+dependencies = [
+  "pytest", # run as `hatch run test:pytest`
+]
+
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `kitsunekko_tools-0.0.4/PKG-INFO` & `kitsunekko_tools-24.4.29.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitsunekko-tools
-Version: 0.0.4
+Version: 24.4.29.0
 Summary: A set of scripts for creating a local kitsunekko mirror.
 Author-email: Ren Tatsumoto <tatsu@autistici.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,27 +696,38 @@
 ktools config create
 ```
 
 Edit the config file.
 
  * `destination` - the local folder where the files should be downloaded.
  * `proxy` - Your proxy settings.
-   Set to `null` if you don't use proxies.
+   Set to `""` (empty string) if you don't use proxies.
    By default, it is set to the default Tor address.
 
 Everything else usually doesn't need to be changed.
 
 ## Usage
 
+The first time, run full sync.
+It will download everything.
+
+``` bash
+ktools sync --full
+```
+
 Run sync.
+If you already have downloaded everything once,
+this command will skip files that have not been modified recently.
 
 ``` bash
 ktools sync
 ```
 
+The `skip_older` config parameter controls what files should be skipped during regular runs.
+
 ## Upload your mirror to Mega
 
 1) Install [megatools](https://archlinux.org/packages/extra/x86_64/megatools/).
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
 
 ## Ignoring certain files
```

