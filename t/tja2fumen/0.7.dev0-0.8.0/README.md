# Comparing `tmp/tja2fumen-0.7.dev0.tar.gz` & `tmp/tja2fumen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.7.dev0.tar", last modified: Sat Feb  3 22:43:29 2024, max compression
+gzip compressed data, was "tja2fumen-0.8.0.tar", last modified: Tue Apr 30 02:12:50 2024, max compression
```

## Comparing `tja2fumen-0.7.dev0.tar` & `tja2fumen-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-03 22:43:29.718546 tja2fumen-0.7.dev0/
--rw-rw-rw-   0        0        0     1085 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0    13070 2024-02-03 22:43:29.718546 tja2fumen-0.7.dev0/PKG-INFO
--rw-rw-rw-   0        0        0    10974 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/README.md
--rw-rw-rw-   0        0        0     1294 2024-02-03 22:43:21.000000 tja2fumen-0.7.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-03 22:43:29.718546 tja2fumen-0.7.dev0/setup.cfg
--rw-rw-rw-   0        0        0       98 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:43:29.702915 tja2fumen-0.7.dev0/src/
-drwxrwxrwx   0        0        0        0 2024-02-03 22:43:29.702915 tja2fumen-0.7.dev0/src/tja2fumen/
--rw-rw-rw-   0        0        0     3263 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0    15654 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/classes.py
--rw-rw-rw-   0        0        0     2883 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    26667 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0   307495 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/hp_values.csv
--rw-rw-rw-   0        0        0    22777 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/parsers.py
--rw-rw-rw-   0        0        0     2553 2024-02-03 22:42:38.000000 tja2fumen-0.7.dev0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:43:29.718546 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0    13070 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-03 22:43:29.000000 tja2fumen-0.7.dev0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/
+-rw-rw-rw-   0        0        0     1085 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15196 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13103 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/README.md
+-rw-rw-rw-   0        0        0     1382 2024-04-30 02:12:46.000000 tja2fumen-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     5856 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0    16022 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/classes.py
+-rw-rw-rw-   0        0        0     3263 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    27352 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0   307495 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/hp_values.csv
+-rw-rw-rw-   0        0        0    27085 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0     2806 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0    15196 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.7.dev0/LICENSE.txt` & `tja2fumen-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.7.dev0/PKG-INFO` & `tja2fumen-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,7 @@
-Metadata-Version: 2.1
-Name: tja2fumen
-Version: 0.7.dev0
-Summary: Convert TJA chart files into fumen (.bin) chart files
-License: MIT License
-        
-        Copyright (c) 2023 Vivaria
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/vivaria/tja2fumen/
-Project-URL: Bug Reports, https://github.com/vivaria/tja2fumen/issues/
-Project-URL: Source, https://github.com/vivaria/tja2fumen/
-Keywords: taiko,tatsujin,fumen,TJA
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pyinstaller; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: toml-cli; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pyproject-flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-
 &nbsp;
 <p align="center">
   <img
     width="400"
     src="https://user-images.githubusercontent.com/76574898/255353006-6c4504d0-c9a4-40d1-961f-db4cef7add0d.png"
     alt="tja2fumen – TJA chart converter"
   />
@@ -67,34 +23,82 @@
 
 </p>
 
 
 
 ----
 
+> [!IMPORTANT]
+> tja2fumen is a tool designed for mod developers. It allows modders to load TJA charts into official games by converting them into Taiko's official binary fumen file format (`.bin`).
+> 
+> If you are not a mod developer, and you just want to play TJAs on Taiko no Tatsujin PC, please install and run [TakoTako](https://github.com/fluto/takotako). (Alternatively, you can also run TakoTako's `TJAConvert.exe` [directly on your TJA files](#tja--audio-conversion).)
+
+
+> [!NOTE]
+> #### Replacing tja2bin (TakoTako 3.2.0 and below)
+> TakoTako 3.2.0 includes an older, flawed tool called `tja2bin.exe`. If you have downloaded TakoTako 3.2.0, you should replace the old `tja2bin.exe` with the latest version of `tja2fumen.exe`. This will ensure that your TJAs get converted accurately.
+>
+> You can do this by:
+> - Downloading `tja2fumen.exe` from the [releases page](https://github.com/vivaria/tja2fumen/releases).
+> - Renaming the file to `tja2bin.exe`.
+> - Copying and pasting it into the `{TDMX_INSTALLATION_DIR}/BepInEx/plugins/com.fluto.takotako/` directory, replacing the old `tja2bin.exe`.
+
 ## Features
 
 tja2fumen is designed to be an open source alternative to the closed source tja2bin tool that has been floating around various Discord servers. tja2fumen fixes several outstanding tja2bin issues, while providing an open source codebase to modify and learn from.
 
-- Converts `.tja` chart files to official fumen `.bin` files.
+- Command line tool to convert `.tja` chart files to official fumen `.bin` files.
 - Decodes official fumen `.bin` files (to inspect metadata and note data).
-- Uses strong development practices (thorough test suite with example charts, type checking)
+- Fix `.bin` files that were previously converted by `tja2bin` (WIP, see [#65](https://github.com/vivaria/tja2fumen/issues/65)).
+- Uses strong development practices (thorough test suite with example charts, type checking).
 - Provides an open source resource for the Taiko no Tatsujin fumen file format.
 
 ## Usage
 
-> [!NOTE]  
-> For older versions of TakoTako (3.2.0 and below), you can add tja2fumen by renaming `tja2fumen.exe` to `tja2bin.exe` and placing it inside TakoTako's plugin folder (`BepInEx/plugins/com.fluto.takotako/`).
+### TJA conversion
+
+To convert a `.tja` file to `.bin` files, simply download `tja2fumen.exe` and run:
+
+```bash
+tja2fumen.exe "file.tja"
+```
+
+### TJA + Audio conversion
+
+`tja2fumen.exe` only converts TJA files. If you want to convert both TJAs _and_ audio (.OGG or .WAV files) to `.bin` files, you can use the TakoTako plugin for the PC version of Taiko no Tatsujin. However, if you don't want to install and run Taiko no Tatsujin on PC, then you can use this simpler method instead:
 
-tja2fumen is included as part of several existing projects. So, you may be using tja2fumen already!
+1. Download the [latest release of TakoTako](https://github.com/Fluto/TakoTako/releases).
+2. Extract the `TJAConvert.exe` program into a separate folder.
+3. Download the newest version of `tja2fumen.exe`. Rename it `tja2bin.exe`, then place it in the same folder as `TJAConvert.exe`.
+4. Run the following command:
 
-- **XB1/TDMX**: [TakoTako](https://github.com/fluto/takotako) converts both chart and audio files for XB1/TDMX.
-- **Nijiro**: [TaikoSoundEditor](https://github.com/NotImplementedLife/TaikoSoundEditor) converts both chart and audio files for NIjiro.
+```bash
+TJAConvert.exe "path_to_folder_containing_both_tja_and_audio/"
+```
 
-You can also use tja2fumen directly on a `.tja` file by downloading `tja2fumen.exe` from the [Releases](https://github.com/vivaria/tja2fumen/releases) page and running `tja2fumen.exe file.tja` in a command prompt.
+`TJAConvert.exe` will convert the audio to CRIWARE HCA packed into ACB container, and then it will call `tja2fumen.exe` to convert the chart files. (This is the exact same conversion you would get by running TakoTako as a BepInEx plugin -- you just have more control.) Note that the output audio is unencrypted, and that ACB audio files are incompatible with any NUS3BANK-based games.
+
+### Decoding fumen charts in Python scripts
+
+If you want to explore the song structure of existing `.bin` files or `.tja` files using Python scripts, run:
+
+```
+pip install tja2fumen
+```
+
+Then, you can use tja2fumen's Python API as follows:
+
+```python
+from tja2fumen.parsers import parse_fumen, parse_tja
+
+fumen = parse_fumen("path/to/fumen_file.bin")
+tja = parse_tja("path/to/tja_file.tja")
+```
+
+Please refer to `src/__init__.py` for further example usage of the Python API.
 
 ## TJA Support
 
 If there is an unsupported feature that you would like support for, please make a request by [opening a new issue](https://github.com/vivaria/tja2fumen/issues/new).
 
 ### Supported file formats
 
@@ -120,15 +124,15 @@
 
 ### Supported notes/commands
 
 > **Legend**: `✅` = Fully supported, `⚪️` = Ignored, `⚠️` = Incorrect behavior, `❌` = Not supported
 
 |                                              | tja 2 fumen | tja 2 bin | Comment                                                                                                       |
 |----------------------------------------------|-------------|-----------|---------------------------------------------------------------------------------------------------------------|
-| `0`, `1`, `2`, `3`, `4`                      | `✅`         | `✅`       |                                                                                                               |
+| `0`, `1`, `2`, `3`, `4`                      | `✅`         | `⚠️`       | tja2fumen will write proper SENOTES (ド, コ, ドン, カ, カッ), see [#41](https://github.com/vivaria/tja2fumen/issues/41). |
 | `5008,`, `6008,`, `7008,`                    | `✅`         | `✅`       |                                                                                                               |
 | `9008,`                                      | `✅`         | `⚠️`      |                                                                                                               |
 | `9000,`<br>`9008,`                           | `⚪️`        | `⚠️`      | Double Kusudama note treated as 1 drumroll by tja2fumen, but 2 overlapping drumrolls by tja2bin.              |
 | `A`, `B`                                     | `✅`         | `❌`       | Multiplayer "hands" notes are valid in fumens, but unrecognized by tja2bin.                                   |
 | `C`, `D`, `E`, `F`, `G`, `H`, `I`            | `⚠️`        | `❌`       | Replaced by normal notes/rolls in tja2fumen.                                                                  |
 | `#START`, `#END`                             | `✅`         | `✅`       |                                                                                                               |
 | `#START P1`, `#START P2`                     | `✅`         | `❌`       |                                                                                                               |
@@ -146,16 +150,14 @@
 
 ## Reporting bugs
 
 If you've found a `.tja` file that tja2fumen converts incorrectly, please [open a new issue](https://github.com/vivaria/tja2fumen/issues/new) on the tja2fumen repo. 
 
 It is especially important that you attach the song files to the issue. You can do this by adding the song files to a `.zip` (Select files -> Right click -> "Send to" -> "Compressed (zipped) folder"), and then uploading the `.zip` to the issue. This greatly helps me to reproduce and fix any issues.
 
-You can also message me directly on Discord (`_vivaria`) if you don't have a GitHub account, and I will take care of making an issue for you. :)
-
 ## Building on top of tja2fumen
 
 If you are a developer looking to add tja2fumen to your project, you have two options:
 
 1. For non-Python projects, you can download `tja2fumen.exe` and call it via a system call.
 2. For Python projects, you can install tja2fumen via `pip install tja2fumen`.
```

#### html2text {}

```diff
@@ -1,79 +1,86 @@
-Metadata-Version: 2.1 Name: tja2fumen Version: 0.7.dev0 Summary: Convert TJA
-chart files into fumen (.bin) chart files License: MIT License Copyright (c)
-2023 Vivaria Permission is hereby granted, free of charge, to any person
-obtaining a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including without
-limitation the rights to use, copy, modify, merge, publish, distribute,
-sublicense, and/or sell copies of the Software, and to permit persons to whom
-the Software is furnished to do so, subject to the following conditions: The
-above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
-IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
-LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
-AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
-https://github.com/vivaria/tja2fumen/ Project-URL: Bug Reports, https://
-github.com/vivaria/tja2fumen/issues/ Project-URL: Source, https://github.com/
-vivaria/tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt Provides-
-Extra: dev Requires-Dist: pytest; extra == "dev" Requires-Dist: build; extra ==
-"dev" Requires-Dist: pyinstaller; extra == "dev" Requires-Dist: twine; extra ==
-"dev" Requires-Dist: toml-cli; extra == "dev" Requires-Dist: flake8; extra ==
-"dev" Requires-Dist: pyproject-flake8; extra == "dev" Requires-Dist: mypy;
-extra == "dev" Requires-Dist: pylint; extra == "dev"  
+ 
                       [tja2fumen â TJA chart converter]
    tja2fumen is a tool that allows you to convert TJA charts (.tja) to fumen
                                 charts (.bin).
 _[_T_e_s_t_ _s_t_a_t_u_s_ _(_m_a_i_n_ _b_r_a_n_c_h_)_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_w_i_t_h_ _f_i_l_t_e_r_)_]_[_M_I_T_ _L_i_c_e_n_s_e_]_[_L_i_n_t_i_n_g
                      _p_y_l_i_n_t_]_[_L_i_n_t_i_n_g_ _f_l_a_k_e_8_]_[_L_i_n_t_i_n_g_ _m_y_p_y_]
----- ## Features tja2fumen is designed to be an open source alternative to the
-closed source tja2bin tool that has been floating around various Discord
-servers. tja2fumen fixes several outstanding tja2bin issues, while providing an
-open source codebase to modify and learn from. - Converts `.tja` chart files to
-official fumen `.bin` files. - Decodes official fumen `.bin` files (to inspect
-metadata and note data). - Uses strong development practices (thorough test
-suite with example charts, type checking) - Provides an open source resource
-for the Taiko no Tatsujin fumen file format. ## Usage > [!NOTE] > For older
-versions of TakoTako (3.2.0 and below), you can add tja2fumen by renaming
-`tja2fumen.exe` to `tja2bin.exe` and placing it inside TakoTako's plugin folder
-(`BepInEx/plugins/com.fluto.takotako/`). tja2fumen is included as part of
-several existing projects. So, you may be using tja2fumen already! - **XB1/
-TDMX**: [TakoTako](https://github.com/fluto/takotako) converts both chart and
-audio files for XB1/TDMX. - **Nijiro**: [TaikoSoundEditor](https://github.com/
-NotImplementedLife/TaikoSoundEditor) converts both chart and audio files for
-NIjiro. You can also use tja2fumen directly on a `.tja` file by downloading
-`tja2fumen.exe` from the [Releases](https://github.com/vivaria/tja2fumen/
-releases) page and running `tja2fumen.exe file.tja` in a command prompt. ## TJA
-Support If there is an unsupported feature that you would like support for,
-please make a request by [opening a new issue](https://github.com/vivaria/
-tja2fumen/issues/new). ### Supported file formats > **Legend**: `â` = Fully
-supported, `â` = Not supported | | tja 2 fumen | tja 2 bin | Comment | |-----
-----------------|-------------|-----------|----------| | UTF-8 (with BOM) |
-`â` | `â` | â | | UTF-8 (without BOM) | `âï¸` | `â` | â | | Shift-
-JIS | `â` | `â` | â | ### Supported metadata > **Legend**: `â` = Fully
-supported, `âªï¸` = Ignored, `â ï¸` = Incorrect behavior, `â` = Not
-supported | | tja 2 fumen | tja 2 bin | Comment | |----------------------------
--------------------------------------|-------------|-----------|---------------
-----------------------------------------------------------| | `BPM:`, `OFFSET:
-` | `â` | `â` | â | | `TITLE:`, `SUBTITLE:`, `WAVE:`,
+---- > [!IMPORTANT] > tja2fumen is a tool designed for mod developers. It
+allows modders to load TJA charts into official games by converting them into
+Taiko's official binary fumen file format (`.bin`). > > If you are not a mod
+developer, and you just want to play TJAs on Taiko no Tatsujin PC, please
+install and run [TakoTako](https://github.com/fluto/takotako). (Alternatively,
+you can also run TakoTako's `TJAConvert.exe` [directly on your TJA files](#tja-
+-audio-conversion).) > [!NOTE] > #### Replacing tja2bin (TakoTako 3.2.0 and
+below) > TakoTako 3.2.0 includes an older, flawed tool called `tja2bin.exe`. If
+you have downloaded TakoTako 3.2.0, you should replace the old `tja2bin.exe`
+with the latest version of `tja2fumen.exe`. This will ensure that your TJAs get
+converted accurately. > > You can do this by: > - Downloading `tja2fumen.exe`
+from the [releases page](https://github.com/vivaria/tja2fumen/releases). > -
+Renaming the file to `tja2bin.exe`. > - Copying and pasting it into the `
+{TDMX_INSTALLATION_DIR}/BepInEx/plugins/com.fluto.takotako/` directory,
+replacing the old `tja2bin.exe`. ## Features tja2fumen is designed to be an
+open source alternative to the closed source tja2bin tool that has been
+floating around various Discord servers. tja2fumen fixes several outstanding
+tja2bin issues, while providing an open source codebase to modify and learn
+from. - Command line tool to convert `.tja` chart files to official fumen
+`.bin` files. - Decodes official fumen `.bin` files (to inspect metadata and
+note data). - Fix `.bin` files that were previously converted by `tja2bin`
+(WIP, see [#65](https://github.com/vivaria/tja2fumen/issues/65)). - Uses strong
+development practices (thorough test suite with example charts, type checking).
+- Provides an open source resource for the Taiko no Tatsujin fumen file format.
+## Usage ### TJA conversion To convert a `.tja` file to `.bin` files, simply
+download `tja2fumen.exe` and run: ```bash tja2fumen.exe "file.tja" ``` ### TJA
++ Audio conversion `tja2fumen.exe` only converts TJA files. If you want to
+convert both TJAs _and_ audio (.OGG or .WAV files) to `.bin` files, you can use
+the TakoTako plugin for the PC version of Taiko no Tatsujin. However, if you
+don't want to install and run Taiko no Tatsujin on PC, then you can use this
+simpler method instead: 1. Download the [latest release of TakoTako](https://
+github.com/Fluto/TakoTako/releases). 2. Extract the `TJAConvert.exe` program
+into a separate folder. 3. Download the newest version of `tja2fumen.exe`.
+Rename it `tja2bin.exe`, then place it in the same folder as `TJAConvert.exe`.
+4. Run the following command: ```bash TJAConvert.exe
+"path_to_folder_containing_both_tja_and_audio/" ``` `TJAConvert.exe` will
+convert the audio to CRIWARE HCA packed into ACB container, and then it will
+call `tja2fumen.exe` to convert the chart files. (This is the exact same
+conversion you would get by running TakoTako as a BepInEx plugin -- you just
+have more control.) Note that the output audio is unencrypted, and that ACB
+audio files are incompatible with any NUS3BANK-based games. ### Decoding fumen
+charts in Python scripts If you want to explore the song structure of existing
+`.bin` files or `.tja` files using Python scripts, run: ``` pip install
+tja2fumen ``` Then, you can use tja2fumen's Python API as follows: ```python
+from tja2fumen.parsers import parse_fumen, parse_tja fumen = parse_fumen("path/
+to/fumen_file.bin") tja = parse_tja("path/to/tja_file.tja") ``` Please refer to
+`src/__init__.py` for further example usage of the Python API. ## TJA Support
+If there is an unsupported feature that you would like support for, please make
+a request by [opening a new issue](https://github.com/vivaria/tja2fumen/issues/
+new). ### Supported file formats > **Legend**: `â` = Fully supported, `â` =
+Not supported | | tja 2 fumen | tja 2 bin | Comment | |---------------------|--
+-----------|-----------|----------| | UTF-8 (with BOM) | `â` | `â` | â |
+| UTF-8 (without BOM) | `âï¸` | `â` | â | | Shift-JIS | `â` | `â` |
+â | ### Supported metadata > **Legend**: `â` = Fully supported, `âªï¸` =
+Ignored, `â ï¸` = Incorrect behavior, `â` = Not supported | | tja 2 fumen |
+tja 2 bin | Comment | |--------------------------------------------------------
+---------|-------------|-----------|-------------------------------------------
+------------------------------| | `BPM:`, `OFFSET:` | `â` | `â` | â | |
+`TITLE:`, `SUBTITLE:`, `WAVE:`,
 `DEMOSTART:`, etc. | `âªï¸` | `âªï¸` | The only global metadata needed are
 `BPM:` and `OFFSET:`. â | | `COURSE:`, `LEVEL:`, `BALLOON:`,
 `SCOREINIT:`, `SCOREDIFF:` | `â` | `â` | â | | `STYLE:` (`Single`,
 `Double`) | `â` | `â` | â | | `EXAM1:`, `GAUGEINCR:`, `TOTAL:`, etc. |
 `âªï¸` | `âªï¸` | Other simulator-specific metadata fields are currently
 ignored.â | ### Supported notes/commands > **Legend**: `â` = Fully
 supported, `âªï¸` = Ignored, `â ï¸` = Incorrect behavior, `â` = Not
 supported | | tja 2 fumen | tja 2 bin | Comment | |----------------------------
 ------------------|-------------|-----------|----------------------------------
 -----------------------------------------------------------------------------
-| | `0`, `1`, `2`, `3`, `4` | `â` | `â` | | | `5008,`, `6008,`, `7008,` |
-`â` | `â` | | | `9008,` | `â` | `â ï¸` | | | `9000,`
+| | `0`, `1`, `2`, `3`, `4` | `â` | `â ï¸` | tja2fumen will write proper
+SENOTES (ã, ã³, ãã³, ã«, ã«ã), see [#41](https://github.com/vivaria/
+tja2fumen/issues/41). | | `5008,`, `6008,`, `7008,` | `â` | `â` | | |
+`9008,` | `â` | `â ï¸` | | | `9000,`
 `9008,` | `âªï¸` | `â ï¸` | Double Kusudama note treated as 1 drumroll by
 tja2fumen, but 2 overlapping drumrolls by tja2bin. | | `A`, `B` | `â` | `â`
 | Multiplayer "hands" notes are valid in fumens, but unrecognized by tja2bin. |
 | `C`, `D`, `E`, `F`, `G`, `H`, `I` | `â ï¸` | `â` | Replaced by normal
 notes/rolls in tja2fumen. | | `#START`, `#END` | `â` | `â` | | | `#START
 P1`, `#START P2` | `â` | `â` | | | `#BPMCHANGE` | `â` | `â ï¸` | See
 [#16](https://github.com/Fluto/TakoTako/issues/16) | | `#MEASURE` | `â` |
@@ -87,25 +94,23 @@
 `#DIRECTION`, etc. | `âªï¸` | `â` | Other simulator-specific chart commands
 are currently ignored. | ## Reporting bugs If you've found a `.tja` file that
 tja2fumen converts incorrectly, please [open a new issue](https://github.com/
 vivaria/tja2fumen/issues/new) on the tja2fumen repo. It is especially important
 that you attach the song files to the issue. You can do this by adding the song
 files to a `.zip` (Select files -> Right click -> "Send to" -> "Compressed
 (zipped) folder"), and then uploading the `.zip` to the issue. This greatly
-helps me to reproduce and fix any issues. You can also message me directly on
-Discord (`_vivaria`) if you don't have a GitHub account, and I will take care
-of making an issue for you. :) ## Building on top of tja2fumen If you are a
-developer looking to add tja2fumen to your project, you have two options: 1.
-For non-Python projects, you can download `tja2fumen.exe` and call it via a
-system call. 2. For Python projects, you can install tja2fumen via `pip install
-tja2fumen`. tja2fumen uses a very permissable license ([MIT License](https://
-choosealicense.com/licenses/mit/)). You are free to distribute and modify
-tja2fumen, but please include a copy of the MIT License alongside the
-`tja2fumen.exe` executable if you copy it into your project. ## Attribution -
-The fumen-parsing code in this project is based off of a modified copy of the
+helps me to reproduce and fix any issues. ## Building on top of tja2fumen If
+you are a developer looking to add tja2fumen to your project, you have two
+options: 1. For non-Python projects, you can download `tja2fumen.exe` and call
+it via a system call. 2. For Python projects, you can install tja2fumen via
+`pip install tja2fumen`. tja2fumen uses a very permissable license ([MIT
+License](https://choosealicense.com/licenses/mit/)). You are free to distribute
+and modify tja2fumen, but please include a copy of the MIT License alongside
+the `tja2fumen.exe` executable if you copy it into your project. ## Attribution
+- The fumen-parsing code in this project is based off of a modified copy of the
 [`readFumen()`](https://github.com/KatieFrogs/fumen-tools/blob/
 6ff3a2f7f53687f3dd49c5c57fcfc5ccbe3e5a10/fumen2osu/fumen2osu.py#L7-L152)
 function from the [`fumen2osu.py`](https://github.com/KatieFrogs/fumen-tools/
 blob/main/fumen2osu/fumen2osu.py) found in @KatieFrogs' [`fumen-tools`](https:/
 /github.com/KatieFrogs/fumen-tools) project. - The TJA-parsing code in this
 project is a Python translation of the [`parseTJA.js`](https://github.com/
 WHMHammer/tja-tools/blob/master/src/js/parseTJA.js) file from @WHMHammer's
```

### Comparing `tja2fumen-0.7.dev0/pyproject.toml` & `tja2fumen-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.7.dev0"
+version = "0.8.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
@@ -21,16 +21,17 @@
 dev = ["pytest", "build", "pyinstaller", "twine", "toml-cli",
        "flake8", "pyproject-flake8", "mypy", "pylint"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
-addopts = "-vv --tb=short"
+addopts = "-vv --tb=short --color=yes"
 console_output_style = "count"
+disable_test_id_escaping_and_forfeit_all_rights_to_community_support = "True"
 
 [tool.flake8]
 exclude = "venv/"
 per-file-ignores = """
     ./src/tja2fumen/classes.py: E221
     ./testing/test_conversion.py: E221, E272
 """
```

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/classes.py` & `tja2fumen-0.8.0/src/tja2fumen/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import csv
 import os
 import struct
 from typing import Any, List, Dict, Tuple
 
 from dataclasses import dataclass, field, fields
 
-from tja2fumen.constants import BRANCH_NAMES
+from tja2fumen.constants import BRANCH_NAMES, TIMING_WINDOWS
 
 
 @dataclass()
 class TJAData:
     """Contains the information for a single note or single command."""
     name: str
     value: str
@@ -220,15 +220,15 @@
                 self.branch_info[4:6] = vals
 
 
 @dataclass()
 class FumenHeader:
     """Contains all the byte values for a Fumen chart file's header."""
     order: str = "<"
-    b000_b431_timing_windows: Tuple[float, ...] = (25.025, 75.075, 108.422)*36
+    b000_b431_timing_windows: Tuple[float, ...] = (0.0, 0.0, 0.0)*36
     b432_b435_has_branches:                 int = 0
     b436_b439_hp_max:                       int = 10000
     b440_b443_hp_clear:                     int = 8000
     b444_b447_hp_gain_good:                 int = 10
     b448_b451_hp_gain_ok:                   int = 5
     b452_b455_hp_loss_bad:                  int = -20
     b456_b459_normal_normal_ratio:          int = 65536
@@ -288,14 +288,20 @@
         # both little and big endian, then compare to see which is correct.
         if (self.unp(raw_bytes, ">I", 512, 515) <
                 self.unp(raw_bytes, "<I", 512, 515)):
             self.order = ">"
         else:
             self.order = "<"
 
+    def set_timing_windows(self, difficulty: str) -> None:
+        """Set the timing window header bytes depending on the difficulty."""
+        # Note: Ura Oni is equivalent to Oni for timing window behavior
+        difficulty = 'Oni' if difficulty in ['Ura', 'Edit'] else difficulty
+        self.b000_b431_timing_windows = TIMING_WINDOWS[difficulty]*36
+
     def set_hp_bytes(self, n_notes: int, difficulty: str, stars: int) -> None:
         """Compute header bytes related to the soul gauge (HP) behavior."""
         # Note: Ura Oni is equivalent to Oni for soul gauge behavior
         difficulty = 'Oni' if difficulty in ['Ura', 'Edit'] else difficulty
         self._get_hp_from_lookup_tables(n_notes, difficulty, stars)
         self.b440_b443_hp_clear = {'Easy': 6000, 'Normal': 7000,
                                    'Hard': 7000, 'Oni': 8000}[difficulty]
```

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/constants.py` & `tja2fumen-0.8.0/src/tja2fumen/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,7 +90,15 @@
 COURSE_IDS = {
     'Easy': 'e',
     'Normal': 'n',
     'Hard': 'h',
     'Oni': 'm',
     'Ura': 'x',
 }
+
+TIMING_WINDOWS = {
+    #            "GOOD" timing      "OK" timing       "BAD" timing
+    'Easy':   (041.7083358764648, 108.441665649414, 125.125000000000),
+    'Normal': (041.7083358764648, 108.441665649414, 125.125000000000),
+    'Hard':   (025.0250015258789, 075.075004577637, 108.441665649414),
+    'Oni':    (025.0250015258789, 075.075004577637, 108.441665649414)
+}
```

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/converters.py` & `tja2fumen-0.8.0/src/tja2fumen/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Functions for converting TJA song data to Fumen song data.
 """
 
 import re
+import warnings
 from typing import List, Dict, Tuple, Union
 
 from tja2fumen.classes import (TJACourse, TJAMeasure, TJAMeasureProcessed,
                                FumenCourse, FumenHeader, FumenMeasure,
                                FumenNote)
 from tja2fumen.constants import BRANCH_NAMES
 
@@ -54,18 +55,23 @@
                     measure_tja_processed.notes.append(data)
 
                 # Handle commands that can only be placed between measures
                 # (i.e. no mid-measure variations)
                 elif data.name == 'delay':
                     measure_tja_processed.delay = float(data.value) * 1000
                 elif data.name == 'branch_start':
-                    branch_type, val1, val2 = data.value.split(',')
-                    if branch_type == 'r':  # r = drumRoll
+                    branch_parts = data.value.split(',')
+                    if len(branch_parts) != 3:
+                        raise ValueError(f"#BRANCHSTART must have 3 comma-"
+                                         f"separated values, but got "
+                                         f"'{data.value}' instead.")
+                    branch_type, val1, val2 = branch_parts
+                    if branch_type.lower() == 'r':  # r = drumRoll
                         branch_cond = (float(val1), float(val2))
-                    elif branch_type == 'p':  # p = Percentage
+                    elif branch_type.lower() == 'p':  # p = Percentage
                         branch_cond = (float(val1)/100, float(val2)/100)
                     else:
                         raise ValueError(f"Invalid #BRANCHSTART type: "
                                          f"'{branch_type}'.")
                     measure_tja_processed.branch_type = branch_type
                     measure_tja_processed.branch_cond = branch_cond
                 elif data.name == 'section':
@@ -117,27 +123,27 @@
                             barline=current_barline,
                             time_sig=[current_dividend, current_divisor],
                             subdivisions=len(measure_tja.notes),
                             pos_start=data.pos
                         )
 
                 else:
-                    print(f"Unexpected event type: {data.name}")
+                    warnings.warn(f"Unexpected event type: {data.name}")
 
             measure_tja_processed.pos_end = len(measure_tja.notes)
             tja_branches_processed[branch_name].append(measure_tja_processed)
 
     has_branches = all(len(b) for b in tja_branches_processed.values())
     if has_branches:
         if len({len(b) for b in tja_branches_processed.values()}) != 1:
             raise ValueError(
                 "Branches do not have the same number of measures. (This "
                 "check was performed after splitting up the measures due "
                 "to mid-measure commands. Please check any GOGO, BPMCHANGE, "
-                "and SCROLL commands you have in your branches, and make sure"
+                "and SCROLL commands you have in your branches, and make sure "
                 "that each branch has the same number of commands.)"
             )
 
     return tja_branches_processed
 
 
 def convert_tja_to_fumen(tja: TJACourse) -> FumenCourse:
@@ -283,18 +289,20 @@
                 pos_ratio = ((note_tja.pos - measure_tja.pos_start) /
                              (measure_tja.pos_end - measure_tja.pos_start))
                 note_pos = measure_fumen.duration * pos_ratio
 
                 # Handle '8' notes (end of a drumroll/balloon)
                 if note_tja.value == "EndDRB":
                     if not current_drumroll.note_type:
-                        raise ValueError(
+                        warnings.warn(
                             "'8' note encountered without matching "
-                            "drumroll/balloon/kusudama note."
+                            "drumroll/balloon/kusudama note. Ignoring to "
+                            "avoid crash. Check TJA and re-run."
                         )
+                        continue
                     # If a drumroll spans a single measure, then add the
                     # difference between start/end position
                     if not current_drumroll.multimeasure:
                         current_drumroll.duration += (note_pos -
                                                       current_drumroll.pos)
                     # Otherwise, if a drumroll spans multiple measures,
                     # then we want to add the duration between the start
@@ -323,17 +331,19 @@
 
                 # Handle drumroll-specific note metadata
                 if note.note_type in ["Drumroll", "DRUMROLL"]:
                     current_drumroll = note
                 elif note.note_type in ["Balloon", "Kusudama"]:
                     try:
                         note.hits = course_balloons.pop(0)
-                    except IndexError as exc:
-                        raise ValueError(f"Not enough values for 'BALLOON: "
-                                         f"{course_balloons}'") from exc
+                    except IndexError:
+                        warnings.warn(f"Not enough values for 'BALLOON:' "
+                                      f"({tja.balloon}). Using value=1 to "
+                                      f"avoid crashing. Check TJA and re-run.")
+                        note.hits = 1
                     current_drumroll = note
 
                 # Track Don/Ka notes (to later compute header values)
                 elif (note.note_type.lower().startswith('don')
                         or note.note_type.lower().startswith('ka')):
                     total_notes[current_branch] += 1
 
@@ -363,14 +373,16 @@
                 else:
                     current_drumroll.multimeasure = True
                     current_drumroll.duration += (measure_fumen.duration -
                                                   current_drumroll.pos)
 
     # Compute the header bytes that dictate the soul gauge bar behavior
     fumen.header.set_hp_bytes(total_notes['normal'], tja.course, tja.level)
+    # Compute the timing windows based on the course
+    fumen.header.set_timing_windows(tja.course)
 
     # If song has only drumroll branching conditions (also allowing percentage
     # conditions that force a level up/level down), then set the header bytes
     # so that only drumrolls contribute to branching.
     drumroll_only = (
         branch_types           # noqa: branch_types will always be set
         and branch_conditions  # noqa: branch_conditions will always be set
```

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/hp_values.csv` & `tja2fumen-0.8.0/src/tja2fumen/hp_values.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/parsers.py` & `tja2fumen-0.8.0/src/tja2fumen/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Functions for parsing TJA files (.tja) and Fumen files (.bin)
 """
 
 import os
 import re
 import struct
+import warnings
 from copy import deepcopy
 from typing import BinaryIO, Any, List, Dict, Tuple
 
 from tja2fumen.classes import (TJASong, TJACourse, TJAMeasure, TJAData,
                                FumenCourse, FumenMeasure, FumenBranch,
                                FumenNote, FumenHeader)
 from tja2fumen.constants import (NORMALIZE_COURSE, COURSE_NAMES, BRANCH_NAMES,
@@ -64,48 +65,57 @@
     `parse_tja_course_data()` function.
     """
     # Strip leading/trailing whitespace and comments ('// Comment')
     lines = [line.split("//")[0].strip() for line in lines
              if line.split("//")[0].strip()]
 
     # Initialize song with BPM and OFFSET global metadata
-    bpm = float([line.split(":")[1] for line in lines
-                if line.startswith("BPM")][0])
-    offset = float([line.split(":")[1] for line in lines
-                   if line.startswith("OFFSET")][0])
+    tja_metadata = {}
+    for required_metadata in ["BPM", "OFFSET"]:
+        for line in lines:
+            if line.startswith(required_metadata):
+                tja_metadata[required_metadata] = float(line.split(":")[1])
+                break
+        else:
+            raise ValueError(f"TJA does not contain required "
+                             f"'{required_metadata}' metadata.")
     parsed_tja = TJASong(
-        bpm=bpm,
-        offset=offset,
-        courses={course: TJACourse(bpm=bpm, offset=offset, course=course)
+        bpm=tja_metadata['BPM'],
+        offset=tja_metadata['OFFSET'],
+        courses={course: TJACourse(bpm=tja_metadata['BPM'],
+                                   offset=tja_metadata['OFFSET'],
+                                   course=course)
                  for course in TJA_COURSE_NAMES}
     )
 
     current_course = ''
     current_course_basename = ''
     for line in lines:
         # Only metadata and #START commands are relevant for this function
-        match_metadata = re.match(r"^([A-Z0-9]+):(.*)", line)
+        match_metadata = re.match(r"^([a-zA-Z0-9]+):(.*)", line)
         match_start = re.match(r"^#START(?:\s+(.+))?", line)
 
         # Case 1: Metadata lines
         if match_metadata:
             name_upper = match_metadata.group(1).upper()
             value = match_metadata.group(2).strip()
 
             # Course-specific metadata fields
             if name_upper == 'COURSE':
+                value = value.lower().capitalize()  # coerce hard/HARD -> Hard
                 if value not in NORMALIZE_COURSE:
                     raise ValueError(f"Invalid COURSE value: '{value}'")
                 current_course = NORMALIZE_COURSE[value]
                 current_course_basename = current_course
             elif name_upper == 'LEVEL':
-                if value not in ['1', '2', '3', '4', '5',
-                                 '6', '7', '8', '9', '10']:
-                    raise ValueError(f"Invalid LEVEL value: '{value}")
-                parsed_tja.courses[current_course].level = int(value)
+                if not value.isdigit():
+                    raise ValueError(f"Invalid LEVEL value: '{value}'")
+                # restrict to 1 <= level <= 10
+                parsed_level = min(max(int(value), 1), 10)
+                parsed_tja.courses[current_course].level = parsed_level
             elif name_upper == 'SCOREINIT':
                 parsed_tja.courses[current_course].score_init = \
                     int(value.split(",")[-1]) if value else 0
             elif name_upper == 'SCOREDIFF':
                 parsed_tja.courses[current_course].score_diff = \
                     int(value.split(",")[-1]) if value else 0
             elif name_upper == 'BALLOON':
@@ -123,28 +133,34 @@
         # Case 2: #START commands
         elif match_start:
             value = match_start.group(1) if match_start.group(1) else ''
             # For STYLE:Double, #START P1/P2 indicates the start of a new
             # chart. But, we want multiplayer charts to inherit the
             # metadata from the course as a whole, so we deepcopy the
             # existing course for that difficulty.
+            if value in ["1P", "2P"]:
+                value = value[1] + value[0]  # Fix user typo (e.g. 1P -> P1)
             if value in ["P1", "P2"]:
                 current_course = current_course_basename + value
                 parsed_tja.courses[current_course] = \
                     deepcopy(parsed_tja.courses[current_course_basename])
                 parsed_tja.courses[current_course].data = []
             elif value:
                 raise ValueError(f"Invalid value '{value}' for #START.")
 
             # Since P1/P2 has been handled, we can just use a normal '#START'
             parsed_tja.courses[current_course].data.append("#START")
 
         # Case 3: For other commands and data, simply copy as-is (parse later)
         else:
-            parsed_tja.courses[current_course].data.append(line)
+            if current_course:
+                parsed_tja.courses[current_course].data.append(line)
+            else:
+                warnings.warn(f"Data encountered before first COURSE: "
+                              f"'{line}' (Check for typos in TJA)")
 
     # If a .tja has "STYLE: Double" but no "STYLE: Single", then it will be
     # missing data for the "single player" chart. To fix this, we copy over
     # the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
     for course_name in COURSE_NAMES:
         course_single_player = parsed_tja.courses[course_name]
         course_player_one = parsed_tja.courses[course_name+"P1"]
@@ -195,29 +211,31 @@
 
     # Process course lines
     idx_m = 0
     idx_m_branchstart = 0
     for idx_l, line in enumerate(data):
         # 0. Check to see whether line is a command or note data
         command, name, value, note_data = '', '', '', ''
-        match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
+        match_command = re.match(r"^#([a-zA-Z0-9]+)(?:\s+(.+))?", line)
         if match_command:
-            command = match_command.group(1)
+            command = match_command.group(1).upper()
             if match_command.group(2):
                 value = match_command.group(2)
         else:
             note_data = line  # If not a command, then line must be note data
 
         # 1. Parse measure notes
         if note_data:
             # If measure has ended, then add notes to the current measure,
             # then start a new measure by incrementing idx_m
             if note_data.endswith(','):
                 for branch_name in (BRANCH_NAMES if current_branch == 'all'
                                     else [current_branch]):
+                    check_branch_length(parsed_branches, branch_name,
+                                        expected_len=idx_m+1)
                     parsed_branches[branch_name][idx_m].notes += note_data[:-1]
                     parsed_branches[branch_name].append(TJAMeasure())
                 idx_m += 1
             # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
                 for branch_name in (BRANCH_NAMES if current_branch == 'all'
                                     else [current_branch]):
@@ -227,14 +245,16 @@
         elif command in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF',
                          'DELAY', 'SCROLL', 'BPMCHANGE', 'MEASURE',
                          'LEVELHOLD', 'SECTION', 'BRANCHSTART']:
             # Get position of the event
             pos = 0
             for branch_name in (BRANCH_NAMES if current_branch == 'all'
                                 else [current_branch]):
+                check_branch_length(parsed_branches, branch_name,
+                                    expected_len=idx_m+1)
                 pos = len(parsed_branches[branch_name][idx_m].notes)
 
             # Parse event type
             if command == 'GOGOSTART':
                 name, value = 'gogo', '1'
             elif command == 'GOGOEND':
                 name, value = 'gogo', '0'
@@ -256,29 +276,38 @@
                 # If #SECTION occurs before a #BRANCHSTART, then ensure that
                 # it's present on every branch. Otherwise, #SECTION will only
                 # be present on the current branch, and so the `branch_info`
                 # values won't be correctly set for the other two branches.
                 if data[idx_l+1].startswith('#BRANCHSTART'):
                     name = 'section'
                     current_branch = 'all'
+                elif not branch_condition:
+                    name = 'section'
+                    current_branch = 'all'
                 # Otherwise, #SECTION exists in isolation. In this case, to
                 # reset the accuracy, we just repeat the previous #BRANCHSTART.
                 else:
                     name, value = 'branch_start', branch_condition
             elif command == 'BRANCHSTART':
                 # Ensure that the #BRANCHSTART command is added to all branches
                 current_branch = 'all'
                 name = 'branch_start'
                 branch_condition = value
+                # If a branch was intentionally excluded by the charter,
+                # make sure to copy measures from the longest branch.
+                for branch_name in BRANCH_NAMES:
+                    check_branch_length(parsed_branches, branch_name)
                 # Preserve the index of the BRANCHSTART command to re-use
                 idx_m_branchstart = idx_m
 
             # Append event to the current measure's events
             for branch_name in (BRANCH_NAMES if current_branch == 'all'
                                 else [current_branch]):
+                check_branch_length(parsed_branches, branch_name,
+                                    expected_len=idx_m+1)
                 parsed_branches[branch_name][idx_m].events.append(
                     TJAData(name=name, value=value, pos=pos)
                 )
 
         # 3. Parse commands that don't create an event
         #    (e.g. simply changing the current branch)
         else:
@@ -293,27 +322,45 @@
             elif command == 'M':
                 current_branch = 'master'
                 idx_m = idx_m_branchstart
             elif command == 'BRANCHEND':
                 current_branch = 'all'
 
             else:
-                print(f"Ignoring unsupported command '{command}'")
+                warnings.warn(f"Ignoring unsupported command '{command}'")
 
     # Delete the last measure in the branch if no notes or events
     # were added to it (due to preallocating empty measures)
+    deleted_branches = False
     for branch in parsed_branches.values():
         if not branch[-1].notes and not branch[-1].events:
             del branch[-1]
+            deleted_branches = True
+    if deleted_branches:
+        idx_m -= 1
+
+    # Equalize branch lengths to account for missing branches
+    for branch_name, branch in parsed_branches.items():
+        if branch:
+            check_branch_length(parsed_branches, branch_name)
 
     # Merge measure data and measure events in chronological order
     for branch_name, branch in parsed_branches.items():
         for measure in branch:
+            # warn the user if their measure have typos
+            valid_notes = []
+            for note in measure.notes:
+                if note not in TJA_NOTE_TYPES:
+                    warnings.warn(f"Ignoring invalid note '{note}' in measure "
+                                  f"'{''.join(measure.notes)}' (check for "
+                                  f"typos in TJA)")
+                else:
+                    valid_notes.append(note)
             notes = [TJAData(name='note', value=TJA_NOTE_TYPES[note], pos=i)
-                     for i, note in enumerate(measure.notes) if
+                     for i, note in enumerate(valid_notes) if
                      TJA_NOTE_TYPES[note] != 'Blank']
             events = measure.events
             while notes or events:
                 if events and notes:
                     if notes[0].pos >= events[0].pos:
                         measure.combined.append(events.pop(0))
                     else:
@@ -322,24 +369,66 @@
                     measure.combined.append(events.pop(0))
                 elif notes:
                     measure.combined.append(notes.pop(0))
 
     # Ensure all branches have the same number of measures
     if has_branches:
         if len({len(b) for b in parsed_branches.values()}) != 1:
+            # If `check_branch_length` works, this should never be reached
             raise ValueError(
                 "Branches do not have the same number of measures. (This "
                 "check was performed prior to splitting up the measures due "
-                "to mid-measure commands. Please check the number of ',' you"
+                "to mid-measure commands. Please check the number of ',' you "
                 "have in each branch.)"
             )
 
     return parsed_branches
 
 
+def check_branch_length(parsed_branches: Dict[str, List[TJAMeasure]],
+                        branch_name: str, expected_len: int = 0) -> None:
+    """
+    Ensure that a given branch ('branch_name') matches either an expected
+    integer length, or the max length of all branches if length not given.
+
+    Note: Modifies branch in-place.
+    """
+    branch_len = len(parsed_branches[branch_name])
+    # If no length is provided, then we assume we're comparing branches,
+    # then copying any missing measures from the largest branch.
+    if expected_len == 0:
+        max_branch_name = branch_name
+        expected_len = branch_len
+        for name, branch in parsed_branches.items():
+            if len(branch) > expected_len:
+                expected_len = len(branch)
+                max_branch_name = name
+        warning_msg = (f"To fix this, measures will be copied from the "
+                       f"'{max_branch_name}' branch to equalize branch "
+                       f"lengths.")
+        for idx_m in range(branch_len, expected_len):
+            parsed_branches[branch_name].append(
+                parsed_branches[max_branch_name][idx_m]
+            )
+    # Otherwise, if length was provided, then simply pad with empty measures
+    else:
+        warning_msg = ("To fix this, empty measures will be added to "
+                       "equalize branch lengths.")
+        for idx_m in range(branch_len, expected_len):
+            parsed_branches[branch_name].append(TJAMeasure())
+
+    if branch_len < expected_len:
+        warnings.warn(
+            f"While parsing the TJA's branches, tja2fumen expected "
+            f"{expected_len} measure(s) from the '{branch_name}' branch, but "
+            f"it only had {branch_len} measure(s). {warning_msg} (Hint: Do "
+            f"#N, #E, and #M all have the same number of measures?)"
+        )
+
+
 ###############################################################################
 #                          Fumen-parsing functions                            #
 ###############################################################################
 
 def parse_fumen(fumen_file: str,
                 exclude_empty_measures: bool = False) -> FumenCourse:
     """
```

### Comparing `tja2fumen-0.7.dev0/src/tja2fumen/writers.py` & `tja2fumen-0.8.0/src/tja2fumen/writers.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
                 for note in branch.notes:
                     note_struct = [FUMEN_TYPE_NOTES[note.note_type], note.pos,
                                    note.item, note.padding]
                     if note.hits:
                         extra_vals = [note.hits, note.hits_padding]
                     else:
-                        extra_vals = [note.score_init, note.score_diff * 4]
+                        # Max value for H -> 0xffff -> 65535
+                        extra_vals = [min(65535, note.score_init),
+                                      min(65535, note.score_diff * 4)]
                     note_struct.extend(extra_vals)
                     note_struct.append(note.duration)
                     write_struct(file, song.header.order,
                                  format_string="ififHHf",
                                  value_list=note_struct)
 
                     if note.note_type.lower() == "drumroll":
@@ -53,9 +55,12 @@
 
 
 def write_struct(file: BinaryIO,
                  order: str,
                  format_string: str,
                  value_list: List[Any]) -> None:
     """Pack (int, float, etc.) values into a string of bytes, then write."""
-    packed_bytes = struct.pack(order + format_string, *value_list)
+    try:
+        packed_bytes = struct.pack(order + format_string, *value_list)
+    except struct.error as err:
+        raise ValueError(f"Can't fmt {value_list} as {format_string}") from err
     file.write(packed_bytes)
```

