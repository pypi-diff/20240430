# Comparing `tmp/mpflash-0.7.0.tar.gz` & `tmp/mpflash-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.7.0.tar", max compression
+gzip compressed data, was "mpflash-0.7.1.tar", max compression
```

## Comparing `mpflash-0.7.0.tar` & `mpflash-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.0/mpflash/__init__.py
--rw-r--r--   0        0        0     7793 2024-04-12 12:06:31.002240 mpflash-0.7.0/mpflash/ask_input.py
--rw-r--r--   0        0        0     3090 2024-04-12 12:06:31.002240 mpflash-0.7.0/mpflash/cli_download.py
--rw-r--r--   0        0        0     5760 2024-04-25 20:03:13.729881 mpflash-0.7.0/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1967 2024-04-25 18:45:27.705659 mpflash-0.7.0/mpflash/cli_group.py
--rw-r--r--   0        0        0     1005 2024-04-06 13:17:36.787587 mpflash-0.7.0/mpflash/cli_list.py
--rw-r--r--   0        0        0      632 2024-04-11 20:40:17.002612 mpflash-0.7.0/mpflash/cli_main.py
--rw-r--r--   0        0        0     1049 2024-04-12 12:22:07.242346 mpflash-0.7.0/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.0/mpflash/config.py
--rw-r--r--   0        0        0    10765 2024-04-06 16:22:42.858056 mpflash-0.7.0/mpflash/download.py
--rw-r--r--   0        0        0     3803 2024-04-09 22:57:44.547253 mpflash-0.7.0/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-11 22:01:44.716103 mpflash-0.7.0/mpflash/errors.py
--rw-r--r--   0        0        0     2490 2024-04-07 23:02:43.917516 mpflash-0.7.0/mpflash/flash.py
--rw-r--r--   0        0        0     2316 2024-04-12 12:21:11.617847 mpflash-0.7.0/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-13 19:41:37.773737 mpflash-0.7.0/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-13 19:41:45.110360 mpflash-0.7.0/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-11 22:23:28.005043 mpflash-0.7.0/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2093 2024-04-25 20:46:33.719715 mpflash-0.7.0/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.0/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4298 2024-04-05 19:52:32.898069 mpflash-0.7.0/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1072 2024-04-05 19:52:32.900154 mpflash-0.7.0/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     3186 2024-04-25 21:38:21.828236 mpflash-0.7.0/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.0/mpflash/logger.py
--rw-r--r--   0        0        0     3509 2024-04-11 22:02:26.573574 mpflash-0.7.0/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     2230 2024-04-11 22:02:45.348676 mpflash-0.7.0/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.0/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-04-05 19:52:32.903789 mpflash-0.7.0/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     7017 2024-04-25 19:59:34.679576 mpflash-0.7.0/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.0/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4783 2024-04-15 16:01:00.749925 mpflash-0.7.0/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-04-05 19:52:32.916470 mpflash-0.7.0/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-05 19:52:32.918984 mpflash-0.7.0/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-05 19:52:32.919979 mpflash-0.7.0/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3629 2024-04-12 10:48:05.417995 mpflash-0.7.0/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5299 2024-04-25 20:25:46.822847 mpflash-0.7.0/mpflash/worklist.py
--rw-r--r--   0        0        0     1628 2024-04-25 21:40:15.517575 mpflash-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    12253 2024-04-09 20:15:12.410633 mpflash-0.7.0/README.md
--rw-r--r--   0        0        0    13778 1970-01-01 00:00:00.000000 mpflash-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.1/mpflash/__init__.py
+-rw-r--r--   0        0        0     8442 2024-04-29 18:55:09.404909 mpflash-0.7.1/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3266 2024-04-29 18:55:09.406130 mpflash-0.7.1/mpflash/cli_download.py
+-rw-r--r--   0        0        0     5847 2024-04-29 18:55:09.407466 mpflash-0.7.1/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.1/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.1/mpflash/cli_list.py
+-rw-r--r--   0        0        0      656 2024-04-29 18:55:09.408806 mpflash-0.7.1/mpflash/cli_main.py
+-rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.1/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.1/mpflash/config.py
+-rw-r--r--   0        0        0    10991 2024-04-29 18:55:09.412110 mpflash-0.7.1/mpflash/download.py
+-rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.1/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.1/mpflash/errors.py
+-rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.1/mpflash/flash.py
+-rw-r--r--   0        0        0     2316 2024-04-29 18:55:09.415109 mpflash-0.7.1/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.1/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.1/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.1/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2093 2024-04-29 18:55:09.417421 mpflash-0.7.1/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.1/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4298 2024-04-05 19:52:32.898069 mpflash-0.7.1/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1072 2024-04-05 19:52:32.900154 mpflash-0.7.1/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     3252 2024-04-29 18:55:09.417421 mpflash-0.7.1/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.1/mpflash/logger.py
+-rw-r--r--   0        0        0     3509 2024-04-29 18:55:09.418429 mpflash-0.7.1/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     2230 2024-04-29 18:55:09.419434 mpflash-0.7.1/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.1/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-04-05 19:52:32.903789 mpflash-0.7.1/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     7017 2024-04-29 18:55:09.420429 mpflash-0.7.1/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.1/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.1/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.1/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.1/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.1/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3629 2024-04-29 18:55:09.425429 mpflash-0.7.1/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5299 2024-04-29 18:55:09.426431 mpflash-0.7.1/mpflash/worklist.py
+-rw-r--r--   0        0        0     1630 2024-04-29 20:59:33.897829 mpflash-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13153 2024-04-29 20:30:38.703519 mpflash-0.7.1/README.md
+-rw-r--r--   0        0        0    14627 1970-01-01 00:00:00.000000 mpflash-0.7.1/PKG-INFO
```

### Comparing `mpflash-0.7.0/LICENSE` & `mpflash-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/ask_input.py` & `mpflash-0.7.1/mpflash/ask_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List, Sequence, Tuple, Union
 
 from loguru import logger as log
 
 from mpflash.config import config
-from mpflash.mpboard_id import known_stored_boards, local_mp_ports
+from mpflash.mpboard_id import get_stored_boards_for_port, known_stored_boards, local_mp_ports
 from mpflash.mpremoteboard import MPRemoteBoard
 from mpflash.vendor.versions import micropython_versions
 
 
 @dataclass
 class Params:
     ports: List[str] = field(default_factory=list)
@@ -127,15 +127,15 @@
     if some_boards:
         # Create a dictionary where the keys are the second elements of the tuples
         # This will automatically remove duplicates because dictionaries cannot have duplicate keys
         unique_dict = {item[1]: item for item in some_boards}
         # Get the values of the dictionary, which are the unique items from the original list
         some_boards = list(unique_dict.values())
     else:
-        some_boards = [("No boards found", "")]
+        some_boards = [(f"No {answers['port']} boards found for version(s) {_versions}", "")]
     return some_boards
 
 
 def ask_port_board(questions: list, *, action: str):
     """
     Asks the user for the port and board selection.
 
@@ -182,30 +182,45 @@
         action (str): The action to be performed.
 
     Returns:
         None
     """
     # import only when needed to reduce load time
     import inquirer
+    import inquirer.errors
 
     input_ux = inquirer.Checkbox if action == "download" else inquirer.List
     mp_versions: List[str] = micropython_versions()
     mp_versions = [v for v in mp_versions if "preview" not in v]
+
+    # remove the versions for which there are no known boards in the board_info.json
+    # todo: this may be a little slow
+    mp_versions = [v for v in mp_versions if get_stored_boards_for_port("stm32", [v])]
+
     mp_versions.append("preview")
     mp_versions.reverse()  # newest first
+
+    def at_least_one_validation(answers, current) -> bool:
+        if not current:
+            raise inquirer.errors.ValidationError("", reason="Please select at least one version")
+        if isinstance(current, list):
+            if not any(current):
+                raise inquirer.errors.ValidationError("", reason="Please select at least one version")
+        return True
+
     questions.append(
         input_ux(
             # inquirer.List(
             "versions",
             message="Which version(s) do you want to {action} " + ("to {serial} ?" if action == "flash" else "?"),
             # Hints would be nice , but needs a hint for each and every option
             # hints=["Use space to select multiple options"],
             choices=mp_versions,
             autocomplete=True,
-            validate=lambda _, x: True if x else "Please select at least one version",  # type: ignore
+            validate=at_least_one_validation,
         )
     )
 
 
 def ask_serialport(questions: list, *, action: str):
     """
     Asks the user for the serial port selection.
```

### Comparing `mpflash-0.7.0/mpflash/cli_download.py` & `mpflash-0.7.1/mpflash/cli_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pathlib import Path
 from typing import List, Tuple
 
 import rich_click as click
 from loguru import logger as log
 
+from mpflash.errors import MPFlashError
 from mpflash.mpboard_id import find_stored_board
 from mpflash.vendor.versions import clean_version
 
 from .ask_input import DownloadParams, ask_missing_params
 from .cli_group import cli
 from .cli_list import list_mcus
 from .config import config
@@ -58,41 +59,44 @@
 @click.option(
     "--force",
     default=False,
     is_flag=True,
     show_default=True,
     help="""Force download of firmware even if it already exists.""",
 )
-def cli_download(
-    **kwargs,
-):
+def cli_download(**kwargs) -> int:
     params = DownloadParams(**kwargs)
     params.versions = list(params.versions)
     params.boards = list(params.boards)
     if params.boards:
         pass
         # TODO Clean board - same as in cli_flash.py
     else:
         # no boards specified - detect connected boards
         params.ports, params.boards = connected_ports_boards()
 
     params = ask_missing_params(params, action="download")
     if not params:  # Cancelled by user
-        exit(1)
+        return 2
     params.versions = [clean_version(v, drop_v=True) for v in params.versions]
     assert isinstance(params, DownloadParams)
 
-    download(
-        params.fw_folder,
-        params.ports,
-        params.boards,
-        params.versions,
-        params.force,
-        params.clean,
-    )
+    try:
+        download(
+            params.fw_folder,
+            params.ports,
+            params.boards,
+            params.versions,
+            params.force,
+            params.clean,
+        )
+        return 0
+    except MPFlashError as e:
+        log.error(f"{e}")
+        return 1
 
 
 def connected_ports_boards() -> Tuple[List[str], List[str]]:
     """
     Returns a tuple containing lists of unique ports and boards from the connected MCUs.
     Boards that are physically connected, but give no tangible response are ignored.
```

### Comparing `mpflash-0.7.0/mpflash/cli_flash.py` & `mpflash-0.7.1/mpflash/cli_flash.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "flash",
     short_help="Flash one or all connected MicroPython boards with a specific firmware and version.",
 )
 @click.option(
     "--firmware",
     "-f",
     "fw_folder",
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, path_type=Path),
+    type=click.Path(file_okay=False, dir_okay=True, path_type=Path),
     default=config.firmware_folder,
     show_default=True,
     help="The folder to retrieve the firmware from.",
 )
 @click.option(
     "--version",
     "-v",
@@ -87,15 +87,15 @@
 @click.option(
     "--bootloader/--no-bootloader",
     default=True,
     is_flag=True,
     show_default=True,
     help="""Enter micropython bootloader mode before flashing.""",
 )
-def cli_flash_board(**kwargs):
+def cli_flash_board(**kwargs) -> int:
     # version to versions, board to boards
     kwargs["versions"] = [kwargs.pop("version")] if kwargs["version"] != None else []
     if kwargs["board"] is None:
         kwargs["boards"] = []
         kwargs.pop("board")
     else:
         kwargs["boards"] = [kwargs.pop("board")]
@@ -123,15 +123,15 @@
                         params.boards.append(info["board"])
                 except Exception as e:
                     log.warning(f"unable to resolve board description: {e}")
 
     # Ask for missing input if needed
     params = ask_missing_params(params, action="flash")
     if not params:  # Cancelled by user
-        exit(1)
+        return 2
     # TODO: Just in time Download of firmware
 
     assert isinstance(params, FlashParams)
 
     if len(params.versions) > 1:
         log.error(f"Only one version can be flashed at a time, not {params.versions}")
         raise MPFlashError("Only one version can be flashed at a time")
@@ -164,7 +164,11 @@
         worklist,
         params.fw_folder,
         params.erase,
         params.bootloader,
     ):
         log.info(f"Flashed {len(flashed)} boards")
         show_mcus(flashed, title="Updated boards after flashing")
+        return 0
+    else:
+        log.error("No boards were flashed")
+        return 1
```

### Comparing `mpflash-0.7.0/mpflash/cli_group.py` & `mpflash-0.7.1/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/cli_list.py` & `mpflash-0.7.1/mpflash/cli_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     "--progress/--no-progress",
     "progress",
     is_flag=True,
     default=True,
     show_default=True,
     help="""Show progress""",
 )
-def cli_list_mcus(as_json: bool, progress: bool = True):
+def cli_list_mcus(as_json: bool, progress: bool = True) -> int:
     """List the connected MCU boards, and output in a nice table or json."""
     if as_json:
         # avoid noise in json output
         make_quiet()
 
     conn_mcus = list_mcus()
     if as_json:
         print(json.dumps([mcu.__dict__ for mcu in conn_mcus], indent=4))
         progress = False
     if progress:
         show_mcus(conn_mcus, refresh=False)
-    return conn_mcus
+    return 0 if conn_mcus else 1
```

### Comparing `mpflash-0.7.0/mpflash/cli_main.py` & `mpflash-0.7.1/mpflash/cli_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """mpflash is a CLI to download and flash MicroPython firmware to various boards."""
 
 # import rich_click as click
 
+import click
+
 from .cli_download import cli_download
 from .cli_flash import cli_flash_board
 from .cli_group import cli
 from .cli_list import cli_list_mcus
 
-# from loguru import logger as log
-
 
 def mpflash():
     cli.add_command(cli_flash_board)
     cli.add_command(cli_list_mcus)
     cli.add_command(cli_download)
     # cli(auto_envvar_prefix="MPFLASH")
     try:
-        exit(cli())
+        result = cli(standalone_mode=False)
+        exit(result)
     except AttributeError as e:
         print(f"Error: {e}")
         exit(-1)
 
 
 if __name__ == "__main__":
     mpflash()
```

### Comparing `mpflash-0.7.0/mpflash/common.py` & `mpflash-0.7.1/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/download.py` & `mpflash-0.7.1/mpflash/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import jsonlines
 import requests
 from bs4 import BeautifulSoup
 from loguru import logger as log
 from rich.progress import track
 
 from mpflash.common import PORT_FWTYPES
+from mpflash.errors import MPFlashError
 
 jsonlines.ujson = None  # type: ignore
 # #########################################################################################################
 
 
 MICROPYTHON_ORG_URL = "https://micropython.org/"
 
@@ -161,15 +162,15 @@
     firmware_folder: Path,
     ports: List[str],
     boards: List[str],
     versions: Optional[List[str]] = None,
     *,
     force: bool = False,
     clean: bool = True,
-):
+) -> int:
     skipped = downloaded = 0
     if versions is None:
         versions = []
     unique_boards = get_firmware_list(ports, boards, versions, clean)
 
     for b in unique_boards:
         log.debug(b["filename"])
@@ -196,14 +197,15 @@
                 board["filename"] = str(filename.relative_to(firmware_folder))
             except requests.RequestException as e:
                 log.exception(e)
                 continue
             writer.write(board)
             downloaded += 1
     log.info(f"Downloaded {downloaded} firmwares, skipped {skipped} existing files.")
+    return downloaded + skipped
 
 
 def get_firmware_list(ports: List[str], boards: List[str], versions: List[str], clean: bool):
     """
     Retrieves a list of unique firmware information based on the specified ports, boards, versions, and clean flag.
 
     Args:
@@ -242,36 +244,37 @@
 def download(
     destination: Path,
     ports: List[str],
     boards: List[str],
     versions: List[str],
     force: bool,
     clean: bool,
-):
+) -> int:
     """
     Downloads firmware files based on the specified destination, ports, boards, versions, force flag, and clean flag.
 
     Args:
         destination : The destination folder to save the downloaded firmware files.
         ports : The list of ports to check for firmware.
         boards : The list of boards to download firmware for.
         versions : The list of versions to download firmware for.
         force : A flag indicating whether to force the download even if the firmware file already exists.
         clean : A flag indicating whether to perform a clean download.
 
     Returns:
-        None
+        int: The number of downloaded firmware files.
 
     Raises:
-        SystemExit: If no boards are found or specified.
+        MPFlashError : If no boards are found or specified.
 
     """
     if not boards:
         log.critical("No boards found, please connect a board or specify boards to download firmware for.")
-        exit(1)
+        raise MPFlashError("No boards found")
     # versions = [clean_version(v, drop_v=True) for v in versions]  # remove leading v from version
     try:
         destination.mkdir(exist_ok=True, parents=True)
     except (PermissionError, FileNotFoundError) as e:
-        log.critical(f"Could not create folder {destination}\n{e}")
-        exit(1)
-    download_firmwares(destination, ports, boards, versions, force=force, clean=clean)
+        log.critical(f"Could not create folder {destination}")
+        raise MPFlashError(f"Could not create folder {destination}") from e
+
+    return download_firmwares(destination, ports, boards, versions, force=force, clean=clean)
```

### Comparing `mpflash-0.7.0/mpflash/downloaded.py` & `mpflash-0.7.1/mpflash/downloaded.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash.py` & `mpflash-0.7.1/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_esp.py` & `mpflash-0.7.1/mpflash/flash_esp.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_stm32.py` & `mpflash-0.7.1/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_stm32_cube.py` & `mpflash-0.7.1/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_stm32_dfu.py` & `mpflash-0.7.1/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_uf2.py` & `mpflash-0.7.1/mpflash/flash_uf2.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_uf2_linux.py` & `mpflash-0.7.1/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/flash_uf2_windows.py` & `mpflash-0.7.1/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/list.py` & `mpflash-0.7.1/mpflash/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List
 
 from rich import print
 from rich.progress import BarColumn, Progress, SpinnerColumn, TextColumn, TimeElapsedColumn, track
 from rich.table import Column, Table
 
 from mpflash.mpremoteboard import MPRemoteBoard
+from mpflash.vendor.versions import clean_version
 
 from .config import config
 from .logger import console
 
 rp_spinner = SpinnerColumn(finished_text="✅")
 rp_text = TextColumn("{task.description} {task.fields[device]}", table_column=Column())
 rp_bar = BarColumn(bar_width=None, table_column=Column())
@@ -78,11 +79,11 @@
         table.add_row(
             mcu.serialport.replace("/dev/", ""),
             mcu.family,
             mcu.port,
             f"{mcu.board}\n{description}".strip(),
             # mcu.variant,
             mcu.cpu,
-            mcu.version,
+            clean_version(mcu.version),
             mcu.build,
         )
     console.print(table)
```

### Comparing `mpflash-0.7.0/mpflash/logger.py` & `mpflash-0.7.1/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpboard_id/__init__.py` & `mpflash-0.7.1/mpflash/mpboard_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpboard_id/board_id.py` & `mpflash-0.7.1/mpflash/mpboard_id/board_id.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpboard_id/board_info.csv` & `mpflash-0.7.1/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpboard_id/board_info.json` & `mpflash-0.7.1/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpremoteboard/__init__.py` & `mpflash-0.7.1/mpflash/mpremoteboard/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.7.1/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/mpremoteboard/runner.py` & `mpflash-0.7.1/mpflash/mpremoteboard/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,25 @@
     reset_tags: LogTagList
     error_tags: LogTagList
     warning_tags: LogTagList
     success_tags: LogTagList
     ignore_tags: LogTagList
 
 
+DEFAULT_RESET_TAGS = [
+    # ESP32 reset causes
+    "rst cause:1, boot mode:",  # 1 -> hardware watch dog reset
+    "rst cause:2, boot mode:",  # 2 -> software watch dog reset (From an exception)
+    "rst cause:3, boot mode:",  # 3 -> software watch dog reset system_restart (Possibly unfed watchdog got angry)
+    "rst cause:4, boot mode:",  # 4 -> soft restart (Possibly with a restart command)
+    "boot.esp32: PRO CPU has been reset by WDT.",
+    "rst:0x10 (RTCWDT_RTC_RESET)",
+]
+
+
 def run(
     cmd: List[str],
     timeout: int = 60,
     log_errors: bool = True,
     no_info: bool = False,
     *,
     log_warnings: bool = False,
@@ -53,26 +64,15 @@
         A list of strings to look for in the output to log as warnings, by default None
     Returns
     -------
     Tuple[int, List[str]]
         The return code and the output as a list of strings
     """
     if not reset_tags:
-        reset_tags = [
-            "rst cause:1, boot mode:",
-            "rst cause:2, boot mode:",
-            "rst cause:3, boot mode:",
-            "rst cause:4, boot mode:",
-        ]
-        # 0 -> normal startup by power on
-        # 1 -> hardware watch dog reset
-        # 2 -> software watch dog reset (From an exception)
-        # 3 -> software watch dog reset system_restart (Possibly unfed watchdog got angry)
-        # 4 -> soft restart (Possibly with a restart command)
-        # 5 -> wake up from deep-sleep
+        reset_tags = DEFAULT_RESET_TAGS
     if not error_tags:
         error_tags = ["Traceback ", "Error: ", "Exception: ", "ERROR :", "CRIT  :"]
     if not warning_tags:
         warning_tags = ["WARN  :", "TRACE :"]
     if not success_tags:
         success_tags = []
     if not ignore_tags:
```

### Comparing `mpflash-0.7.0/mpflash/vendor/dfu.py` & `mpflash-0.7.1/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/vendor/pydfu.py` & `mpflash-0.7.1/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/vendor/versions.py` & `mpflash-0.7.1/mpflash/vendor/versions.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/mpflash/worklist.py` & `mpflash-0.7.1/mpflash/worklist.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.0/pyproject.toml` & `mpflash-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.7.0"
+version = "0.7.1"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
@@ -21,15 +21,15 @@
 python =  ">=3.8.1,<4.0"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
 loguru = "^0.7.2"
 esptool = "^4.7.0"
 jsonlines = "^4.0.0"
 bincopy = "^20.0.0"
-strip-ansi = "^0.1.1"
+# strip-ansi = "^0.1.1"
 rich-click = "^1.7.3"
 psutil = "^5.9.8"
 blkinfo = "^0.2.0"
 pygithub = "^2.1.1"
 platformdirs = "^4.2.0"
 pyusb = "^1.2.1"
 packaging = "23.2"
```

### Comparing `mpflash-0.7.0/README.md` & `mpflash-0.7.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# mpflash
-mpflash is a command-line tool for working with MicroPython firmware. It provides various features to help you develop, build, and manage your MicroPython projects.
+# MPFLASH
 
-This tool was created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it can also be used for manual flashing and development.
+`mpflash` is a command-line tool for working with MicroPython firmware. It provides features to help you flash and update Micropython on one or more .
 
-mpflash has been tested on Windows x64, Linux X64 and ARM64, but not (yet) macOS.
+This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to me be used for manual downloadig, flashing and development.
+
+`mpflash` has been tested on Windows x64, Linux X64, but not (yet) macOS.
+Tested ports: `rp2`, `samd`, `esp32`, `esp32s3`, `esp32c3`, `esp8266` and `stm32`
 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
- 2. Download MicroPython firmware for specific boards and versions.
- 3. Flash one or all connected MicroPython boards with a specific firmware or version.
-    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32
+ 2. Download MicroPython firmware for versions, and matching a specified board or matches your current attached board.
+ 3. Flash one or all connected MicroPython boards with a specific firmware or version.  
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
 
 ## Basic usage
 You can use mpflash to perform various operations on your MicroPython boards. Here is an example of basic usage:
 
@@ -26,61 +27,68 @@
 
 ## Linux permissions to access usb devices 
 In order to flash the firmware to the board, you need to have the correct permissions to access the USB devices.
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
 [See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
-## Advanced use
+## Detailed usage
 You can list the connected boards using the following command:
 ```bash
 $ mpflash list
 D:\MyPython\micropython-stubber> mpflash list
-Getting board info ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% 0:00:02
-                                       Connected boards
-┏━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━┓
-┃ Serial ┃ Family      ┃ Port    ┃ Board              ┃ CPU         ┃ Version        ┃ build ┃
-┡━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━┩
-│ COM11  │ micropython │ rp2     │ RPI_PICO_W         │ RP2040      │ 1.20.0         │       │
-│ COM12  │ micropython │ esp8266 │ ESP8266_GENERIC    │ ESP8266     │ 1.22.2         │       │
-│ COM18  │ micropython │ rp2     │ RPI_PICO_W         │ RP2040      │ 1.23.0-preview │ 155   │
-│ COM3   │ micropython │ samd    │ SEEED_WIO_TERMINAL │ SAMD51P19A  │ 1.23.0-preview │ 155   │
-│ COM5   │ micropython │ stm32   │ PYBV11             │ STM32F405RG │ 1.23.0-preview │ 166   │
-│ COM8   │ micropython │ esp32   │ ESP32_GENERIC_S3   │ ESP32S3     │ 1.23.0-preview │ 155   │
-└────────┴─────────────┴─────────┴────────────────────┴─────────────┴────────────────┴───────┘
+                                               Connected boards
+┏━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━┓
+┃ Serial  ┃Family       ┃Port  ┃Board                                      ┃CPU     ┃Version          ┃build ┃
+┡━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━┩
+│ COM21   │micropython  │rp2   │RPI_PICO                                   │RP2040  │v1.23.0-preview  │  236 │
+│         │             │      │Raspberry Pi Pico with RP2040              │        │                 │      │
+│ COM23   │micropython  │rp2   │RPI_PICO_W                                 │RP2040  │v1.23.0-preview  │  176 │
+│         │             │      │Raspberry Pi Pico W with RP2040            │        │                 │      │
+│ COM9    │micropython  │rp2   │ARDUINO_NANO_RP2040_CONNECT                │RP2040  │v1.23.0-preview  │  341 │
+│         │             │      │Arduino Nano RP2040 Connect with RP2040    │        │                 │      │
+└─────────┴─────────────┴──────┴───────────────────────────────────────────┴────────┴─────────────────┴──────┘
 ```
+## Download the firmware
 
-Suppose you want to download the MicroPython firmware for some boards, you can use the following command: 
+To download the MicroPython firmware for some boards, use the following command: 
+ - `mpflash download` download the latest stable firmware for all connected boards
+ - `mpflash download --version preview` download the current preview for all connected boards
+ - `mpflash download --board ESP8266_GENERIC --board SEEED_WIO_TERMINAL` download these specific boards
+ - `mpflash download --version ? --board ?` prompt to select a specific version and board to download
 
-```bash
-# download the firmware
-$ mpflash download --board ESP8266_GENERIC --board SEEED_WIO_TERMINAL
-```	
-This will download the latest stable version of the MicroPython firmware for the boards and save it in the `firmware` directory.
+These will try to download the prebuilt MicroPython firmware for the boards from https://micropython.org/download/ and save it in your downloads folder in the  `firmware` directory.
 The stable version (default) is determined based on the most recent published release,
-other optionse are `--version preview` and `--version x.y.z` to download the latest preview or version x.y.z respectively.
+other versions are `--version preview` and `--version x.y.z` to download the latest preview or version x.y.z respectively.
 
-by default the firmware will be downloaded to  Downloads  in a `firmware` folder in your, but you can specify a different directory using the `--dir` option.
+By default the firmware will be downloaded to your OS's preferred `Downloads/firmware` folder, but you can speciy a different directory using the `--dir` option.
 
-```bash
 The directory structure will be something like this:
-```
+
+``` text
 Downloads/firmware
 |   firmware.jsonl
 +---esp8266
 |       ESP8266_GENERIC-FLASH_1M-v1.22.2.bin
 |       ESP8266_GENERIC-FLASH_512K-v1.22.2.bin
 |       ESP8266_GENERIC-OTA-v1.22.2.bin
 |       ESP8266_GENERIC-v1.22.2.bin
 \---samd
         SEEED_WIO_TERMINAL-v1.22.2.uf2
 ```
-You can then flash the firmware to the board using the following command: `mpflash flash`
+
+## Flashing the firmware
+After you have downloaded a firmware you can  flash the firmware to a board using the following command: `mpflash flash`
 This will (try to) autodetect the connected boards, and determine the correct firmware to flash to each board.
 
+- `mpflash flash` will flash the latest stable firmware to all connected boards.
+- `mpflash flash --serial ? --board ?` will prompt to select a specific serial port and board to flash. (the firmware must be dowloaded earlier)
+
+
+### Flashing all connected boards with the latest stable firmware
 ```bash
 > mpflash flash
 22:15:55 | ℹ️  - Using latest stable version: v1.22.2
                                        Connected boards
 ┏━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━┓
 ┃ Serial ┃ Family      ┃ Port    ┃ Board              ┃ CPU         ┃ Version        ┃ build ┃
 ┡━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━┩
```

### Comparing `mpflash-0.7.0/PKG-INFO` & `mpflash-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.7.0
+Version: 0.7.1
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -28,31 +28,31 @@
 Requires-Dist: packaging (==23.2)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pygithub (>=2.1.1,<3.0.0)
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich-click (>=1.7.3,<2.0.0)
-Requires-Dist: strip-ansi (>=0.1.1,<0.2.0)
 Requires-Dist: tenacity (==8.2.3)
 Project-URL: Repository, https://github.com/Josverl/micropython-stubber
 Description-Content-Type: text/markdown
 
-# mpflash
-mpflash is a command-line tool for working with MicroPython firmware. It provides various features to help you develop, build, and manage your MicroPython projects.
+# MPFLASH
 
-This tool was created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it can also be used for manual flashing and development.
+`mpflash` is a command-line tool for working with MicroPython firmware. It provides features to help you flash and update Micropython on one or more .
 
-mpflash has been tested on Windows x64, Linux X64 and ARM64, but not (yet) macOS.
+This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to me be used for manual downloadig, flashing and development.
+
+`mpflash` has been tested on Windows x64, Linux X64, but not (yet) macOS.
+Tested ports: `rp2`, `samd`, `esp32`, `esp32s3`, `esp32c3`, `esp8266` and `stm32`
 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
- 2. Download MicroPython firmware for specific boards and versions.
- 3. Flash one or all connected MicroPython boards with a specific firmware or version.
-    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32
+ 2. Download MicroPython firmware for versions, and matching a specified board or matches your current attached board.
+ 3. Flash one or all connected MicroPython boards with a specific firmware or version.  
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
 
 ## Basic usage
 You can use mpflash to perform various operations on your MicroPython boards. Here is an example of basic usage:
 
@@ -65,61 +65,68 @@
 
 ## Linux permissions to access usb devices 
 In order to flash the firmware to the board, you need to have the correct permissions to access the USB devices.
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
 [See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
-## Advanced use
+## Detailed usage
 You can list the connected boards using the following command:
 ```bash
 $ mpflash list
 D:\MyPython\micropython-stubber> mpflash list
-Getting board info ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% 0:00:02
-                                       Connected boards
-┏━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━┓
-┃ Serial ┃ Family      ┃ Port    ┃ Board              ┃ CPU         ┃ Version        ┃ build ┃
-┡━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━┩
-│ COM11  │ micropython │ rp2     │ RPI_PICO_W         │ RP2040      │ 1.20.0         │       │
-│ COM12  │ micropython │ esp8266 │ ESP8266_GENERIC    │ ESP8266     │ 1.22.2         │       │
-│ COM18  │ micropython │ rp2     │ RPI_PICO_W         │ RP2040      │ 1.23.0-preview │ 155   │
-│ COM3   │ micropython │ samd    │ SEEED_WIO_TERMINAL │ SAMD51P19A  │ 1.23.0-preview │ 155   │
-│ COM5   │ micropython │ stm32   │ PYBV11             │ STM32F405RG │ 1.23.0-preview │ 166   │
-│ COM8   │ micropython │ esp32   │ ESP32_GENERIC_S3   │ ESP32S3     │ 1.23.0-preview │ 155   │
-└────────┴─────────────┴─────────┴────────────────────┴─────────────┴────────────────┴───────┘
+                                               Connected boards
+┏━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━┓
+┃ Serial  ┃Family       ┃Port  ┃Board                                      ┃CPU     ┃Version          ┃build ┃
+┡━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━┩
+│ COM21   │micropython  │rp2   │RPI_PICO                                   │RP2040  │v1.23.0-preview  │  236 │
+│         │             │      │Raspberry Pi Pico with RP2040              │        │                 │      │
+│ COM23   │micropython  │rp2   │RPI_PICO_W                                 │RP2040  │v1.23.0-preview  │  176 │
+│         │             │      │Raspberry Pi Pico W with RP2040            │        │                 │      │
+│ COM9    │micropython  │rp2   │ARDUINO_NANO_RP2040_CONNECT                │RP2040  │v1.23.0-preview  │  341 │
+│         │             │      │Arduino Nano RP2040 Connect with RP2040    │        │                 │      │
+└─────────┴─────────────┴──────┴───────────────────────────────────────────┴────────┴─────────────────┴──────┘
 ```
+## Download the firmware
 
-Suppose you want to download the MicroPython firmware for some boards, you can use the following command: 
+To download the MicroPython firmware for some boards, use the following command: 
+ - `mpflash download` download the latest stable firmware for all connected boards
+ - `mpflash download --version preview` download the current preview for all connected boards
+ - `mpflash download --board ESP8266_GENERIC --board SEEED_WIO_TERMINAL` download these specific boards
+ - `mpflash download --version ? --board ?` prompt to select a specific version and board to download
 
-```bash
-# download the firmware
-$ mpflash download --board ESP8266_GENERIC --board SEEED_WIO_TERMINAL
-```	
-This will download the latest stable version of the MicroPython firmware for the boards and save it in the `firmware` directory.
+These will try to download the prebuilt MicroPython firmware for the boards from https://micropython.org/download/ and save it in your downloads folder in the  `firmware` directory.
 The stable version (default) is determined based on the most recent published release,
-other optionse are `--version preview` and `--version x.y.z` to download the latest preview or version x.y.z respectively.
+other versions are `--version preview` and `--version x.y.z` to download the latest preview or version x.y.z respectively.
 
-by default the firmware will be downloaded to  Downloads  in a `firmware` folder in your, but you can specify a different directory using the `--dir` option.
+By default the firmware will be downloaded to your OS's preferred `Downloads/firmware` folder, but you can speciy a different directory using the `--dir` option.
 
-```bash
 The directory structure will be something like this:
-```
+
+``` text
 Downloads/firmware
 |   firmware.jsonl
 +---esp8266
 |       ESP8266_GENERIC-FLASH_1M-v1.22.2.bin
 |       ESP8266_GENERIC-FLASH_512K-v1.22.2.bin
 |       ESP8266_GENERIC-OTA-v1.22.2.bin
 |       ESP8266_GENERIC-v1.22.2.bin
 \---samd
         SEEED_WIO_TERMINAL-v1.22.2.uf2
 ```
-You can then flash the firmware to the board using the following command: `mpflash flash`
+
+## Flashing the firmware
+After you have downloaded a firmware you can  flash the firmware to a board using the following command: `mpflash flash`
 This will (try to) autodetect the connected boards, and determine the correct firmware to flash to each board.
 
+- `mpflash flash` will flash the latest stable firmware to all connected boards.
+- `mpflash flash --serial ? --board ?` will prompt to select a specific serial port and board to flash. (the firmware must be dowloaded earlier)
+
+
+### Flashing all connected boards with the latest stable firmware
 ```bash
 > mpflash flash
 22:15:55 | ℹ️  - Using latest stable version: v1.22.2
                                        Connected boards
 ┏━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━┓
 ┃ Serial ┃ Family      ┃ Port    ┃ Board              ┃ CPU         ┃ Version        ┃ build ┃
 ┡━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━┩
```

