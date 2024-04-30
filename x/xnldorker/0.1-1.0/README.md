# Comparing `tmp/xnldorker-0.1.tar.gz` & `tmp/xnldorker-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnldorker-0.1.tar", last modified: Tue Apr 23 22:24:39 2024, max compression
+gzip compressed data, was "xnldorker-1.0.tar", last modified: Tue Apr 30 20:51:35 2024, max compression
```

## Comparing `xnldorker-0.1.tar` & `xnldorker-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 22:24:39.651021 xnldorker-0.1/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     9303 2024-04-23 22:24:39.636972 xnldorker-0.1/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     9057 2024-04-23 22:06:13.000000 xnldorker-0.1/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-23 22:24:39.653611 xnldorker-0.1/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      670 2024-04-23 21:45:00.000000 xnldorker-0.1/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 22:24:39.331394 xnldorker-0.1/xnldorker/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       18 2024-04-23 21:51:14.000000 xnldorker-0.1/xnldorker/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    43575 2024-04-23 22:23:25.000000 xnldorker-0.1/xnldorker/xnldorker.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 22:24:39.615116 xnldorker-0.1/xnldorker.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     9303 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      295 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       55 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 20:02:25.000000 xnldorker-0.1/xnldorker.egg-info/not-zip-safe
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       10 2024-04-23 22:24:39.000000 xnldorker-0.1/xnldorker.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.955378 xnldorker-1.0/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11035 2024-04-30 20:51:35.941330 xnldorker-1.0/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    10801 2024-04-30 20:50:30.000000 xnldorker-1.0/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-30 20:51:35.957911 xnldorker-1.0/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      671 2024-04-30 20:50:36.000000 xnldorker-1.0/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.640299 xnldorker-1.0/xnldorker/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       18 2024-04-30 20:50:34.000000 xnldorker-1.0/xnldorker/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47493 2024-04-30 20:49:44.000000 xnldorker-1.0/xnldorker/xnldorker.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.920228 xnldorker-1.0/xnldorker.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11035 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      295 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       55 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 20:02:25.000000 xnldorker-1.0/xnldorker.egg-info/not-zip-safe
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       64 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       10 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/top_level.txt
```

### Comparing `xnldorker-0.1/PKG-INFO` & `xnldorker-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,129 @@
-Metadata-Version: 2.1
-Name: xnldorker
-Version: 0.1
-Summary: Run a dork on different search sites
-Home-page: https://github.com/xnl-h4ck3r/xnldorker
-Author: @xnl-h4ck3r
-Description-Content-Type: text/markdown
-Requires-Dist: termcolor
-Requires-Dist: urlparse3
-Requires-Dist: requests
-Requires-Dist: asyncio
-Requires-Dist: beautifulsoup4
-Requires-Dist: playwright
-
-<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
-
-## About - v0.1
-
-This is a tool used to run a dork on different search sites.
-The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
-
-**WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
-
-## Installation
-
-`xnldorker` supports **Python 3**.
-
-Install `xnldorker` in default (global) python environment.
-
-```bash
-pip install xnldorker
-```
-
-OR
-
-```bash
-pip install git+https://github.com/xnl-h4ck3r/xnldorker.git -v
-```
-
-You can upgrade with
-
-```bash
-pip install --upgrade xnldorker
-```
-
-### pipx
-
-Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
-
-```bash
-pipx install git+https://github.com/xnl-h4ck3r/xnldorker.git
-```
-
-## Usage
-
-| Argument | Long Argument        | Description                                                                                                                                                                                                                                       |
-| -------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i       | --input              | A dork to use on the search sources.                                                                                                                                                                                                              |
-| -o       | --output             | The output file that will contain the results (default: output.txt). If piped to another program, output will be written to STDOUT instead.                                                                                                       |
-| -ow      | --output-overwrite   | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                           |
-| -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
-| -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
-| -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
-| -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
-| -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
-| -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
-| -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
-| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
-|          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
-| -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
-|          | --version            | Show current version number.                                                                                                                                                                                                                      |
-| -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
-| -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
-
-## Examples
-
-### Basic use
-
-```
-urless -i target_urls.txt -v
-```
-
-or
-
-```
-echo "site:redbull.com" | xnldorker -v
-```
-
-### Capture output
-
-```
-xnldorker -i "site:redbull.com" > redbull_endpoints.txt
-```
-
-or
-
-```
-xnldorker -i "site:redbull.com" -v -o redbull_endpoints.txt
-```
-
-<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
-
-### Recommendations
-
-- Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
-- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
-- The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
-- You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
-
-## Issues
-
-If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
-Also, if you have problems, it can be useful to use the `-sb`/`--show-browser` option to see what `xnldorker` is doing.
-If you use the `--debug` option, then `xnldorker` will try to write a html file of the contents that it got stuck on, e.g. `xnldorker_Google_20240423_133700.html`. It would also be useful to include these in the github issue.
-
-## TODO
-
-- Add more sources.
-- Identify anti bot mechanism pages on other sources (it's only on a few at the moment) so that `xnldorker` can pause to manually respond if the browser is being viewed.
-- Maybe allow a file of dorks to be passed as input.
-
-## And finally...
-
-Good luck and good hunting!
-If you really love the tool (or any others), or they helped you find an awesome bounty, consider [BUYING ME A COFFEE!](https://ko-fi.com/xnlh4ck3r) ☕ (I could use the caffeine!)
-
-🤘 /XNL-h4ck3r
-
-<p>
-<a href='https://ko-fi.com/B0B3CZKR5' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
+<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
+
+## About - v1.0
+
+This is a tool used to run a dork on different search sites.
+The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
+
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+
+**WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
+
+## Installation
+
+`xnldorker` supports **Python 3**.
+
+Install `xnldorker` in default (global) python environment.
+
+```bash
+pip install xnldorker
+```
+
+OR
+
+```bash
+pip install git+https://github.com/xnl-h4ck3r/xnldorker.git -v
+```
+
+You can upgrade with
+
+```bash
+pip install --upgrade xnldorker
+```
+
+### pipx
+
+Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
+
+```bash
+pipx install git+https://github.com/xnl-h4ck3r/xnldorker.git
+```
+
+## Usage
+
+| Argument | Long Argument        | Description                                                                                                                                                                                                                                       |
+| -------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| -i       | --input              | A dork to use on the search sources. If no advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) are used in the input value, then it is assumed a domain only is passed, and will be prefixed with `site:`                        |
+| -o       | --output             | The output file that will contain the results (default: output.txt). If piped to another program, output will be written to STDOUT instead.                                                                                                       |
+| -ow      | --output-overwrite   | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                           |
+| -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
+| -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
+| -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
+| -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
+| -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
+| -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
+| -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
+| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
+|          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
+| -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
+|          | --version            | Show current version number.                                                                                                                                                                                                                      |
+| -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
+| -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
+
+## Examples
+
+### Basic use
+
+```
+xnldorker -i redbull.com -v
+```
+
+or
+
+```
+echo "redbull.com" | xnldorker -v
+```
+
+(without any advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) then a domain is assumed and prefied with `site:`. So in this case, `site:redbull.com` is searched for)
+
+### Capture output
+
+In this example, search `google` only and save any links for `redbull.com` that have an extension of `.php`
+
+```
+xnldorker -i "site:redbull.com ext:php" -s google -v -o redbull_endpoints.txt
+```
+
+The output can also be piped to another command.
+
+<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
+
+## Recommendations
+
+- Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
+- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
+- You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
+- Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
+- If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
+
+```sh
+xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+```
+
+- After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
+
+## Issues
+
+If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
+Also, if you have problems, it can be useful to use the `-sb`/`--show-browser` option to see what `xnldorker` is doing.
+If you use the `--debug` option, then `xnldorker` will try to write a html file of the contents that it got stuck on, e.g. `xnldorker_Google_20240423_133700.html`. It would also be useful to include these in the github issue.
+
+## TODO
+
+- Add more sources.
+- Identify anti bot mechanism pages on other sources (it's only on a few at the moment) so that `xnldorker` can pause to manually respond if the browser is being viewed.
+- Maybe allow a file of dorks to be passed as input.
+- Find our what search operators work on which sources and adjust the `--sources` automatically depending on which sources will get the expected results.
+- Add arguments that let you specify a certain time-frame for results which can often be specified with query parameters in the search engine request.
+- Add argument that let you specify a certain Region for results which can often be specified with query parameters in the search engine request.
+
+## And finally...
+
+Good luck and good hunting!
+If you really love the tool (or any others), or they helped you find an awesome bounty, consider [BUYING ME A COFFEE!](https://ko-fi.com/xnlh4ck3r) ☕ (I could use the caffeine!)
+
+🤘 /XNL-h4ck3r
+
+<p>
+<a href='https://ko-fi.com/B0B3CZKR5' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
```

### Comparing `xnldorker-0.1/README.md` & `xnldorker-1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,143 @@
-<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
-
-## About - v0.1
-
-This is a tool used to run a dork on different search sites.
-The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
-
-**WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
-
-## Installation
-
-`xnldorker` supports **Python 3**.
-
-Install `xnldorker` in default (global) python environment.
-
-```bash
-pip install xnldorker
-```
-
-OR
-
-```bash
-pip install git+https://github.com/xnl-h4ck3r/xnldorker.git -v
-```
-
-You can upgrade with
-
-```bash
-pip install --upgrade xnldorker
-```
-
-### pipx
-
-Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
-
-```bash
-pipx install git+https://github.com/xnl-h4ck3r/xnldorker.git
-```
-
-## Usage
-
-| Argument | Long Argument        | Description                                                                                                                                                                                                                                       |
-| -------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i       | --input              | A dork to use on the search sources.                                                                                                                                                                                                              |
-| -o       | --output             | The output file that will contain the results (default: output.txt). If piped to another program, output will be written to STDOUT instead.                                                                                                       |
-| -ow      | --output-overwrite   | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                           |
-| -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
-| -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
-| -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
-| -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
-| -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
-| -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
-| -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
-| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
-|          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
-| -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
-|          | --version            | Show current version number.                                                                                                                                                                                                                      |
-| -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
-| -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
-
-## Examples
-
-### Basic use
-
-```
-urless -i target_urls.txt -v
-```
-
-or
-
-```
-echo "site:redbull.com" | xnldorker -v
-```
-
-### Capture output
-
-```
-xnldorker -i "site:redbull.com" > redbull_endpoints.txt
-```
-
-or
-
-```
-xnldorker -i "site:redbull.com" -v -o redbull_endpoints.txt
-```
-
-<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
-
-### Recommendations
-
-- Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
-- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
-- The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
-- You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
-
-## Issues
-
-If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
-Also, if you have problems, it can be useful to use the `-sb`/`--show-browser` option to see what `xnldorker` is doing.
-If you use the `--debug` option, then `xnldorker` will try to write a html file of the contents that it got stuck on, e.g. `xnldorker_Google_20240423_133700.html`. It would also be useful to include these in the github issue.
-
-## TODO
-
-- Add more sources.
-- Identify anti bot mechanism pages on other sources (it's only on a few at the moment) so that `xnldorker` can pause to manually respond if the browser is being viewed.
-- Maybe allow a file of dorks to be passed as input.
-
-## And finally...
-
-Good luck and good hunting!
-If you really love the tool (or any others), or they helped you find an awesome bounty, consider [BUYING ME A COFFEE!](https://ko-fi.com/xnlh4ck3r) ☕ (I could use the caffeine!)
-
-🤘 /XNL-h4ck3r
-
-<p>
-<a href='https://ko-fi.com/B0B3CZKR5' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
+Metadata-Version: 2.1
+Name: xnldorker
+Version: 1.0
+Summary: Run a dork on different search sites
+Home-page: https://github.com/xnl-h4ck3r/xnldorker
+Author: @xnl-h4ck3r
+Description-Content-Type: text/markdown
+Requires-Dist: termcolor
+Requires-Dist: requests
+Requires-Dist: asyncio
+Requires-Dist: beautifulsoup4
+Requires-Dist: playwright
+Requires-Dist: tldextract
+
+<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
+
+## About - v1.0
+
+This is a tool used to run a dork on different search sites.
+The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
+
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+
+**WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
+
+## Installation
+
+`xnldorker` supports **Python 3**.
+
+Install `xnldorker` in default (global) python environment.
+
+```bash
+pip install xnldorker
+```
+
+OR
+
+```bash
+pip install git+https://github.com/xnl-h4ck3r/xnldorker.git -v
+```
+
+You can upgrade with
+
+```bash
+pip install --upgrade xnldorker
+```
+
+### pipx
+
+Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
+
+```bash
+pipx install git+https://github.com/xnl-h4ck3r/xnldorker.git
+```
+
+## Usage
+
+| Argument | Long Argument        | Description                                                                                                                                                                                                                                       |
+| -------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| -i       | --input              | A dork to use on the search sources. If no advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) are used in the input value, then it is assumed a domain only is passed, and will be prefixed with `site:`                        |
+| -o       | --output             | The output file that will contain the results (default: output.txt). If piped to another program, output will be written to STDOUT instead.                                                                                                       |
+| -ow      | --output-overwrite   | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                           |
+| -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
+| -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
+| -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
+| -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
+| -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
+| -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
+| -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
+| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
+|          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
+| -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
+|          | --version            | Show current version number.                                                                                                                                                                                                                      |
+| -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
+| -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
+
+## Examples
+
+### Basic use
+
+```
+xnldorker -i redbull.com -v
+```
+
+or
+
+```
+echo "redbull.com" | xnldorker -v
+```
+
+(without any advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) then a domain is assumed and prefied with `site:`. So in this case, `site:redbull.com` is searched for)
+
+### Capture output
+
+In this example, search `google` only and save any links for `redbull.com` that have an extension of `.php`
+
+```
+xnldorker -i "site:redbull.com ext:php" -s google -v -o redbull_endpoints.txt
+```
+
+The output can also be piped to another command.
+
+<center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
+
+## Recommendations
+
+- Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
+- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
+- You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
+- Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
+- If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
+
+```sh
+xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+```
+
+- After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
+
+## Issues
+
+If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
+Also, if you have problems, it can be useful to use the `-sb`/`--show-browser` option to see what `xnldorker` is doing.
+If you use the `--debug` option, then `xnldorker` will try to write a html file of the contents that it got stuck on, e.g. `xnldorker_Google_20240423_133700.html`. It would also be useful to include these in the github issue.
+
+## TODO
+
+- Add more sources.
+- Identify anti bot mechanism pages on other sources (it's only on a few at the moment) so that `xnldorker` can pause to manually respond if the browser is being viewed.
+- Maybe allow a file of dorks to be passed as input.
+- Find our what search operators work on which sources and adjust the `--sources` automatically depending on which sources will get the expected results.
+- Add arguments that let you specify a certain time-frame for results which can often be specified with query parameters in the search engine request.
+- Add argument that let you specify a certain Region for results which can often be specified with query parameters in the search engine request.
+
+## And finally...
+
+Good luck and good hunting!
+If you really love the tool (or any others), or they helped you find an awesome bounty, consider [BUYING ME A COFFEE!](https://ko-fi.com/xnlh4ck3r) ☕ (I could use the caffeine!)
+
+🤘 /XNL-h4ck3r
+
+<p>
+<a href='https://ko-fi.com/B0B3CZKR5' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
```

### Comparing `xnldorker-0.1/setup.py` & `xnldorker-1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     version=__import__('xnldorker').__version__,
     description="Run a dork on different search sites",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author="@xnl-h4ck3r",
     url="https://github.com/xnl-h4ck3r/xnldorker",
     zip_safe=False,
-    install_requires=["termcolor", "urlparse3", "requests", "asyncio", "beautifulsoup4", "playwright"],
+    install_requires=["termcolor", "requests", "asyncio", "beautifulsoup4", "playwright", "tldextract"],
     entry_points={
         'console_scripts': [
             'xnldorker = xnldorker.xnldorker:main',
         ],
     },
 )
```

### Comparing `xnldorker-0.1/xnldorker/xnldorker.py` & `xnldorker-1.0/xnldorker/xnldorker.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import datetime
 from signal import SIGINT, signal
 from termcolor import colored
 from pathlib import Path
 import asyncio
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup
+import tldextract
 try:
     from . import __version__
 except:
     pass
 
 # Available sources to search
 SOURCES = ['duckduckgo','bing','startpage','yahoo', 'google']
@@ -28,19 +29,21 @@
 DEFAULT_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36'
 
 # Global variables
 args = None
 browser = None
 stopProgram = False
 stopProgramCount = 0
+inputDork = ''
 duckduckgoEndpoints = set()
 bingEndpoints = set()
 yahooEndpoints = set()
 googleEndpoints = set()
 startpageEndpoints = set()
+allSubs = set()
 sourcesToProcess = []
 
 # Functions used when printing messages dependant on verbose options
 def verbose():
     return args.verbose or args.vverbose
 def vverbose():
     return args.vverbose
@@ -100,41 +103,55 @@
             writerr(colored('>>> Patience isn\'t your strong suit eh? ¯\_(ツ)_/¯','red'))
             sys.exit()
     else:
         stopProgram = True
         writerr(colored('>>> "Oh my God, they killed Kenny... and xnldorker!" - Kyle',"red"))
         writerr(colored('>>> Attempting to rescue any data gathered so far...', "red"))
 
+def getSubdomain(url):
+    try:
+        # Just get the hostname of the url 
+        tldExtract = tldextract.extract(url)
+        return tldExtract.subdomain
+    except Exception as e:
+        writerr(colored('ERROR getSubdomain 1: ' + str(e), 'red')) 
+        
 async def getResultsDuckDuckGo(page, endpoints):
+    global allSubs
     try:
         content = await page.content()
         soup = BeautifulSoup(content, 'html.parser')
         div_content = soup.find('div', id='web_content_wrapper')
         if div_content:
             a_tags = div_content.find_all('a')
             for a in a_tags:
                 href = a.get('href')
                 if href and href.startswith('http') and not re.match(r'^https?:\/\/([\w-]+\.)*duckduckgo\.[^\/\.]{2,}', href):
                     endpoints.append(href.strip())
+                    # If the same search is going to be resubmitted without subs, get the subdomain
+                    if args.resubmit_without_subs:
+                        allSubs.add(getSubdomain(href.strip()))
         return endpoints
     except Exception as e:
         writerr(colored('ERROR getResultsDuckDuckGo 1: ' + str(e), 'red')) 
         
 async def getDuckDuckGo(browser, dork, semaphore):
     global stopProgram
     try:
         endpoints = []
         page = None
         await semaphore.acquire()
         page = await browser.new_page(user_agent=DEFAULT_USER_AGENT)
         
         if verbose():
             writerr(colored('[ DuckDuckGo ] Starting...', 'green'))
-            
-        await page.goto(f'https://duckduckgo.com/?t=h_&ia=web&q={dork}', timeout=args.timeout*1000)
+        
+        # Call with parameters:
+        #  kc=-1 - Don't auto load images
+        await page.goto(f'https://duckduckgo.com/?kc=-1&ia=web&q={dork}', timeout=args.timeout*1000)
         pageNo = 1
         
         # If captcha is shown then allow time to submit it
         captcha = await page.query_selector('#anomaly-modal__modal.anomaly-modal__modal')
         if captcha:
             if args.show_browser:
                 writerr(colored(f'[ Google ] reCAPTCHA needs responding to. Process will resume in {arg.antibot_timeout} seconds...','yellow')) 
@@ -193,24 +210,28 @@
         try:
             await page.close()
             semaphore.release()
         except:
             pass
         
 def extractBingEndpoints(soup):
+    global allSubs
     try:
         endpoints = []
         div_content = soup.find('div', id='b_content')
         if div_content:
             a_tags = div_content.find_all('a')
             for a in a_tags:
                 href = a.get('href')
                 recommendations = a.find_parent('div', class_='pageRecoContainer')
                 if href and href.startswith('http') and not recommendations and not re.match(r'^https?:\/\/([\w-]+\.)*bing\.[^\/\.]{2,}', href) and not re.match(r'^https?:\/\/go\.microsoft\.com', href):
-                    endpoints.append(href)
+                    endpoints.append(href.strip())
+                    # If the same search is going to be resubmitted without subs, get the subdomain
+                    if args.resubmit_without_subs:
+                        allSubs.add(getSubdomain(href.strip()))
         return endpoints
     except Exception as e:
         writerr(colored('ERROR extractBingEndpoints 1: ' + str(e), 'red')) 
         
 async def getBing(browser, dork, semaphore):
     try:
         endpoints = [] 
@@ -279,21 +300,25 @@
         try:
             await page.close()
             semaphore.release()
         except:
             pass
         
 def extractStartpageEndpoints(soup):
+    global allSubs
     try:
         endpoints = []
         result_links = soup.find_all('a', class_=re.compile('.*result-link.*'))
         for link in result_links:
             href = link.get('href')
             if href and href.startswith('http') and not re.match(r'^https?:\/\/([\w-]+\.)*startpage\.[^\/\.]{2,}', href):
-                endpoints.append(href)
+                endpoints.append(href.strip())
+                # If the same search is going to be resubmitted without subs, get the subdomain
+                if args.resubmit_without_subs:
+                    allSubs.add(getSubdomain(href.strip()))
         return endpoints
     except Exception as e:
         writerr(colored('ERROR extractStartpageEndpoints 1: ' + str(e), 'red')) 
         
 async def getStartpage(browser, dork, semaphore):
     try:
         endpoints = []
@@ -412,25 +437,29 @@
         try:
             await page.close()
             semaphore.release()
         except:
             pass
         
 def extractYahooEndpoints(soup):
+    global allSubs
     try:
         endpoints = []
         div_content = soup.find('div', id='results')
         if div_content:
             a_tags = div_content.find_all('a')
             for a in a_tags:
                 # Don't add links from Ads
                 if not a.find_parent(class_="searchCenterTopAds") and not a.find_parent(class_="searchCenterBottomAds"):
                     href = a.get('href')
                     if href and href.startswith('http') and not re.match(r'^https?:\/\/([\w-]+\.)*yahoo\.[^\/\.]{2,}', href) and not re.match(r'^https?:\/\/([\w-]+\.)*bingj\.com', href):
-                        endpoints.append(href)
+                        endpoints.append(href.strip())
+                        # If the same search is going to be resubmitted without subs, get the subdomain
+                        if args.resubmit_without_subs:
+                            allSubs.add(getSubdomain(href.strip()))
         return endpoints
     except Exception as e:
         writerr(colored('ERROR extractYahooEndpoints 1: ' + str(e), 'red')) 
         
 def extractYahooResultNumber(url):
     try:
         match = re.search(r'\b(?:b=)([^&]+)', url)
@@ -527,37 +556,45 @@
         try:
             await page.close()
             semaphore.release()
         except:
             pass
         
 async def getResultsGoogle(page, endpoints):
+    global allSubs
     try:
         content = await page.content()
         soup = BeautifulSoup(content, 'html.parser')
         a_tags = soup.find_all('a')
         for a in a_tags:
             href = a.get('href')
             if href and href.startswith('http') and not re.match(r'^https?:\/\/([\w-]+\.)*google\.[^\/\.]{2,}', href):
                 endpoints.append(href.strip())
+                # If the same search is going to be resubmitted without subs, get the subdomain
+                if args.resubmit_without_subs:
+                    allSubs.add(getSubdomain(href.strip()))
         return endpoints
     except Exception as e:
         writerr(colored('ERROR getResultsGoogle 1: ' + str(e), 'red')) 
         
 async def getGoogle(browser, dork, semaphore):
     try:
         endpoints = []
         page = None
         await semaphore.acquire()
         page = await browser.new_page(user_agent=DEFAULT_USER_AGENT)
         
         if verbose():
             writerr(colored('[ Google ] Starting...', 'green'))
         
-        await page.goto(f'https://www.google.com/search?hl=en&filter=0&q={dork}', timeout=args.timeout*1000)
+        # Use the parameters:
+        #  tbs=li:1 - Verbatim search
+        #  hl=en - English language
+        #  filter=0 - Show near duplicate content
+        await page.goto(f'https://www.google.com/search?tbs=li:1&hl=en&filter=0&q={dork}', timeout=args.timeout*1000)
         await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
         
         pageNo = 1
         
         # If captcha is shown then allow time to submit it
         captcha = await page.query_selector('form#captcha-form')
         if captcha:
@@ -568,15 +605,15 @@
                 writerr(colored('[ Google ] reCAPTCHA needed responding to. Consider using option -vb / --view-browser','red'))
                 return set(endpoints)
         
         # If the cookies notice is shown, accept it
         cookieAccept = await page.query_selector('button:has-text("Accept all")')
         if cookieAccept:
             await cookieAccept.click()
-            
+        
         # If the dialog box asking if you want location specific search, say Not now
         locationSpecific = await page.query_selector('g-raised-button:has-text("Not now")')
         if locationSpecific:
             await locationSpecific.click()
             
         # Scroll to the bottom of the page
         attempts = 0
@@ -658,21 +695,17 @@
             filename = f"xnldorker_{source}_{timestamp}.html"
             with open(filename, "w", encoding="utf-8") as file:
                 file.write(content)
             writerr(colored(f'[ {source} ] Saved HTML content to {filename}', 'cyan')) 
     except Exception as e:
         writerr(colored(f'[ {source} ] Unable to save page contents: {str(e)}', 'cyan')) 
 
-async def processInput():
+async def processInput(dork):
     global browser, sourcesToProcess, duckduckgoEndpoints, bingEndpoints, startpageEndpoints, yahooEndpoints, googleEndpoints
     try:
-        if sys.stdin.isatty():
-            dork = args.input
-        else:
-            dork = sys.stdin.readline().strip()
         
         # Create a single browser instance
         async with async_playwright() as p:
             if args.show_browser:
                 browser = await p.chromium.launch(headless=False)
             else:
                 browser = await p.chromium.launch()
@@ -704,24 +737,44 @@
             except:
                 pass
             
             # Run all searches concurrently using the same browser instance
             results = await asyncio.gather(*includedSources)
             
             # Populate the results dictionary
-            for source, result in zip(sourcesToProcess, results):
-                resultsDict[source] = result
+            #for source, result in zip(sourcesToProcess, results):
+            #    resultsDict[source] = result
             
             # Access the results using the source names
-            duckduckgoEndpoints = resultsDict.get('duckduckgo', [])
-            bingEndpoints = resultsDict.get('bing', [])
-            startpageEndpoints = resultsDict.get('startpage', [])
-            yahooEndpoints = resultsDict.get('yahoo', [])
-            googleEndpoints = resultsDict.get('google', [])
+            #duckduckgoEndpoints = resultsDict.get('duckduckgo', [])
+            #bingEndpoints = resultsDict.get('bing', [])
+            #startpageEndpoints = resultsDict.get('startpage', [])
+            #yahooEndpoints = resultsDict.get('yahoo', [])
+            #googleEndpoints = resultsDict.get('google', [])
             
+            # Populate the results dictionary and endpoint lists
+            for source, result in zip(sourcesToProcess, results):
+                if source not in resultsDict:  # Check if the source is not already in the resultsDict
+                    resultsDict[source] = result  # If not, add it
+                else:
+                    # If the source is already in the resultsDict, append new data to existing data
+                    resultsDict[source].update(result)
+
+                # Update the endpoint lists as well
+                if source == 'duckduckgo':
+                    duckduckgoEndpoints.update(result)
+                elif source == 'bing':
+                    bingEndpoints.update(result)
+                elif source == 'startpage':
+                    startpageEndpoints.update(result)
+                elif source == 'yahoo':
+                    yahooEndpoints.update(result)
+                elif source == 'google':
+                    googleEndpoints.update(result)
+        
             # Close the browser instance once all searches are done
             try:
                 await browser.close()
             except:
                 pass
         
     except Exception as e:
@@ -814,18 +867,18 @@
         except Exception as e:
             writerr(colored('ERROR processOutput 3: ' + str(e), 'red'))
                             
     except Exception as e:
         writerr(colored('ERROR processOutput 1: ' + str(e), 'red'))
 
 def showOptionsAndConfig():
-    global sourcesToProcess
+    global sourcesToProcess, inputDork
     try:
         write(colored('Selected options:', 'cyan'))
-        write(colored('-i: ' + args.input, 'magenta')+colored(' The dork to used to search on the sources.','white'))
+        write(colored('-i: ' + inputDork, 'magenta')+colored(' The dork to used to search on the sources.','white'))
         if args.output is not None:
             write(colored('-o: ' + args.output, 'magenta')+colored(' Where gathered endpoints will be written.','white'))
         else:
             write(colored('-o: <STDOUT>', 'magenta')+colored(' An output file wasn\'t given, so output will be written to STDOUT.','white'))
         write(colored("-ow: " + str(args.output_overwrite), "magenta")+colored(" Whether the output will be overwritten if it already exists.", "white" ))
         if args.sources:
             write(colored('-s: ' + args.sources, 'magenta')+colored(' The sources requested to search.','white'))
@@ -833,14 +886,15 @@
             write(colored('-es: ' + args.exclude_sources, 'magenta')+colored(' The sources excluded from the search.','white'))
         if args.concurrent_sources == 0:
             write(colored('-cs: ALL', 'magenta')+colored(' The browser timeout in seconds','white'))
         else:
             write(colored('-cs: ' + str(args.concurrent_sources), 'magenta')+colored(' The number of concurrent sources that will be searched at a time.','white'))
         write(colored('-t: ' + str(args.timeout), 'magenta')+colored(' The browser timeout in seconds','white'))
         write(colored('-sb: ' + str(args.show_browser), 'magenta')+colored(' Whether the browser will be shown. If False, then headless mode is used.','white'))
+        write(colored('-rwos: ' + str(args.resubmit_without_subs), 'magenta')+colored(' Whether the query will be resubmitted, but excluding the sub domains found in the first search.','white'))
         write(colored('Sources being checked: ', 'magenta')+str(sourcesToProcess))
         write('')
         
     except Exception as e:
         writerr(colored('ERROR showOptionsAndConfig 1: ' + str(e), 'red'))    
 
 # For validating arguments -s and -es
@@ -853,15 +907,15 @@
         raise argparse.ArgumentTypeError(
             f"Invalid sources requested. Can only be a combination of {','.join(SOURCES)}"
         )
     return value
     
 async def run_main():
     
-    global args, sourcesToProcess 
+    global args, sourcesToProcess, allSubs, inputDork
     
     # Tell Python to run the handler() function when SIGINT is received
     signal(SIGINT, handler)
     
     # Parse command line arguments
     parser = argparse.ArgumentParser(
         description='xnldorker - by @Xnl-h4ck3r: Gather results of dorks across a number of search engines.'    
@@ -940,14 +994,20 @@
         "-abt",
         "--antibot-timeout",
         help="How many seconds to wait when the -sb option was used and a known anti-bot mechanism is encountered. This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.",
         default=default_abt,
         type=int,
         metavar="<seconds>",
     )
+    parser.add_argument(
+        '-rwos',
+        '--resubmit-without-subs',
+        action='store_true',
+        help='After the initial search, search again but exclude all subs found previously to get more links.',
+    )
     parser.add_argument('--debug', action='store_true', help='Save page contents on error.')
     parser.add_argument('-nb', '--no-banner', action='store_true', help='Hides the tool banner.')
     parser.add_argument('--version', action='store_true', help='Show version number')
     parser.add_argument('-v', '--verbose', action='store_true', help='Verbose output.')
     parser.add_argument('-vv', '--vverbose', action='store_true', help='Increased verbose output.')
     args = parser.parse_args()
 
@@ -974,25 +1034,41 @@
         if args.sources is None:
             sourcesToProcess = SOURCES
         else:
             sourcesToProcess = args.sources.split(',')
         if args.exclude_sources is not None:
             sourcesToProcess = [source for source in sourcesToProcess if source not in args.exclude_sources]
 
+        # Get the input dork, depending on the input type
+        if sys.stdin.isatty():
+            inputDork = args.input
+        else:
+            inputDork = sys.stdin.readline().strip()
+        
+        # If the input value doesn't seem to start with an advanced search operator and has no spaces, assume it is a domain only and prefix with "site:"
+        if not re.match(r'^[a-z]:', inputDork) and ' ' not in inputDork:
+            inputDork = 'site:'+inputDork
+            
         # If input is not piped, show the banner, and if --verbose option was chosen show options and config values
         if sys.stdin.isatty():
             # Show banner unless requested to hide
             if not args.no_banner:
                 showBanner()
             if verbose():
                 showOptionsAndConfig()
-
+            
         # Process the input given on -i (--input), or <stdin>
-        await processInput()
+        await processInput(inputDork)
 
+        # Process the input given on -i (--input), or <stdin>
+        if args.resubmit_without_subs:
+            inputDork = inputDork + ' ' + ' '.join(['-{}'.format(sub) for sub in allSubs if sub])
+            write(colored('\nResubmitting again for input: ', 'magenta')+colored(inputDork,'white'))
+            await processInput(inputDork)
+        
         # Output the saved urls with parameters
         await processOutput()
         
     except Exception as e:
         writerr(colored('ERROR main 1: ' + str(e), 'red'))      
 
     # Show ko-fi link if verbose and not piped
```

### Comparing `xnldorker-0.1/xnldorker.egg-info/PKG-INFO` & `xnldorker-1.0/xnldorker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: xnldorker
-Version: 0.1
+Version: 1.0
 Summary: Run a dork on different search sites
 Home-page: https://github.com/xnl-h4ck3r/xnldorker
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 Requires-Dist: termcolor
-Requires-Dist: urlparse3
 Requires-Dist: requests
 Requires-Dist: asyncio
 Requires-Dist: beautifulsoup4
 Requires-Dist: playwright
+Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
 
-## About - v0.1
+## About - v1.0
 
 This is a tool used to run a dork on different search sites.
 The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
 
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+
 **WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
 
 ## Installation
 
 `xnldorker` supports **Python 3**.
 
 Install `xnldorker` in default (global) python environment.
@@ -51,15 +53,15 @@
 pipx install git+https://github.com/xnl-h4ck3r/xnldorker.git
 ```
 
 ## Usage
 
 | Argument | Long Argument        | Description                                                                                                                                                                                                                                       |
 | -------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i       | --input              | A dork to use on the search sources.                                                                                                                                                                                                              |
+| -i       | --input              | A dork to use on the search sources. If no advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) are used in the input value, then it is assumed a domain only is passed, and will be prefixed with `site:`                        |
 | -o       | --output             | The output file that will contain the results (default: output.txt). If piped to another program, output will be written to STDOUT instead.                                                                                                       |
 | -ow      | --output-overwrite   | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                           |
 | -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
 | -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
 | -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
 | -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
 | -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
@@ -73,55 +75,66 @@
 | -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
 
 ## Examples
 
 ### Basic use
 
 ```
-urless -i target_urls.txt -v
+xnldorker -i redbull.com -v
 ```
 
 or
 
 ```
-echo "site:redbull.com" | xnldorker -v
+echo "redbull.com" | xnldorker -v
 ```
 
-### Capture output
+(without any advanced search operators (e.g. `site:`, `inurl:`, `intitle:`, etc.) then a domain is assumed and prefied with `site:`. So in this case, `site:redbull.com` is searched for)
 
-```
-xnldorker -i "site:redbull.com" > redbull_endpoints.txt
-```
+### Capture output
 
-or
+In this example, search `google` only and save any links for `redbull.com` that have an extension of `.php`
 
 ```
-xnldorker -i "site:redbull.com" -v -o redbull_endpoints.txt
+xnldorker -i "site:redbull.com ext:php" -s google -v -o redbull_endpoints.txt
 ```
 
+The output can also be piped to another command.
+
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
 
-### Recommendations
+## Recommendations
 
 - Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
 - If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
 - The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
 - You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
+- Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
+- If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
+
+```sh
+xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+```
+
+- After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
 
 ## Issues
 
 If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
 Also, if you have problems, it can be useful to use the `-sb`/`--show-browser` option to see what `xnldorker` is doing.
 If you use the `--debug` option, then `xnldorker` will try to write a html file of the contents that it got stuck on, e.g. `xnldorker_Google_20240423_133700.html`. It would also be useful to include these in the github issue.
 
 ## TODO
 
 - Add more sources.
 - Identify anti bot mechanism pages on other sources (it's only on a few at the moment) so that `xnldorker` can pause to manually respond if the browser is being viewed.
 - Maybe allow a file of dorks to be passed as input.
+- Find our what search operators work on which sources and adjust the `--sources` automatically depending on which sources will get the expected results.
+- Add arguments that let you specify a certain time-frame for results which can often be specified with query parameters in the search engine request.
+- Add argument that let you specify a certain Region for results which can often be specified with query parameters in the search engine request.
 
 ## And finally...
 
 Good luck and good hunting!
 If you really love the tool (or any others), or they helped you find an awesome bounty, consider [BUYING ME A COFFEE!](https://ko-fi.com/xnlh4ck3r) ☕ (I could use the caffeine!)
 
 🤘 /XNL-h4ck3r
```

