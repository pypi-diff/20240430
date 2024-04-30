# Comparing `tmp/libro-0.1.7.tar.gz` & `tmp/libro-0.1.8.tar.gz`

## Comparing `libro-0.1.7.tar` & `libro-0.1.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 libro-0.1.7/.npmrc
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro-0.1.7/.python-version
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro-0.1.7/package.json
--rw-r--r--   0        0        0    68855 2020-02-02 00:00:00.000000 libro-0.1.7/src/dev-config/jupyter_server_config.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/_version.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/app.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/execution_handler.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static_handler.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/workspace_handler.py
--rw-r--r--   0        0        0 29280846 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/100.async.js
--rw-r--r--   0        0        0   256130 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/100.chunk.css
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/1330.async.js
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/1438.async.js
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/161.async.js
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/1639.async.js
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/1772.async.js
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/1838.async.js
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/2048.async.js
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/2118.async.js
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/2130.async.js
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/2999.async.js
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/3572.async.js
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/405.async.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4113.async.js
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4116.async.js
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4123.async.js
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/417.async.js
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4266.async.js
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4343.async.js
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4541.async.js
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4621.async.js
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4658.async.js
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4849.async.js
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/4887.async.js
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/5250.async.js
--rw-r--r--   0        0        0  9358642 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/5332.async.js
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/610.async.js
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/628.async.js
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6357.async.js
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6404.async.js
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6486.async.js
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6730.async.js
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6962.async.js
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/6999.async.js
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/7162.async.js
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/7715.async.js
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/7851.async.js
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/79.async.js
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/8227.async.js
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/8305.async.js
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/8370.async.js
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/8525.async.js
--rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/8945.chunk.css
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9095.async.js
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9150.async.js
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9402.async.js
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9669.async.js
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9674.async.js
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9749.async.js
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/9905.async.js
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/index.html
--rw-r--r--   0        0        0    62202 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/p__execution__index.async.js
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/p__execution__index.chunk.css
--rw-r--r--   0        0        0    17908 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/p__libro__index.async.js
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/p__libro__index.chunk.css
--rw-r--r--   0        0        0   849550 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/umi.js
--rw-r--r--   0        0        0    73464 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/codicon.589e0820.ttf
--rw-r--r--   0        0        0    49764 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/devopicons.3c46801a.woff2
--rw-r--r--   0        0        0    90680 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/file-icons.2cbb51ef.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.cf011583.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.e9955780.woff2
--rw-r--r--   0        0        0   387787 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.f05dad85.svg
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/fontawesome.e9955780.woff2
--rw-r--r--   0        0        0    24412 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/mfixx.8e0807ce.woff2
--rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/octicons.c982f59d.woff2
--rw-r--r--   0        0        0   466610 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/onig.25dd2e6f.wasm
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/static/static/plotly.eb7b9072.svg
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/templates/error.html
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/templates/libro.html
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 libro-0.1.7/src/libro_server/templates/page.html
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libro-0.1.7/.gitignore
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 libro-0.1.7/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 libro-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 libro-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 libro-0.1.8/.npmrc
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro-0.1.8/.python-version
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro-0.1.8/package.json
+-rw-r--r--   0        0        0    68855 2020-02-02 00:00:00.000000 libro-0.1.8/src/dev-config/jupyter_server_config.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/_version.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/app.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/execution_handler.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static_handler.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/workspace_handler.py
+-rw-r--r--   0        0        0 29285132 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/100.async.js
+-rw-r--r--   0        0        0   256130 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/100.chunk.css
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/1330.async.js
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/1438.async.js
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/161.async.js
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/1639.async.js
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/1772.async.js
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/1838.async.js
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/2048.async.js
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/2118.async.js
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/2130.async.js
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/2999.async.js
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/3572.async.js
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/405.async.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4113.async.js
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4116.async.js
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4123.async.js
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/417.async.js
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4266.async.js
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4343.async.js
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4541.async.js
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4621.async.js
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4658.async.js
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4849.async.js
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/4887.async.js
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/5250.async.js
+-rw-r--r--   0        0        0  9358642 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/5332.async.js
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/610.async.js
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/628.async.js
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6357.async.js
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6404.async.js
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6486.async.js
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6730.async.js
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6962.async.js
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/6999.async.js
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/7162.async.js
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/7715.async.js
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/7851.async.js
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/79.async.js
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/8227.async.js
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/8305.async.js
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/8370.async.js
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/8525.async.js
+-rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/8945.chunk.css
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9095.async.js
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9150.async.js
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9402.async.js
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9669.async.js
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9674.async.js
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9749.async.js
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/9905.async.js
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/index.html
+-rw-r--r--   0        0        0    62202 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/p__execution__index.async.js
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/p__execution__index.chunk.css
+-rw-r--r--   0        0        0    17774 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/p__libro__index.async.js
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/p__libro__index.chunk.css
+-rw-r--r--   0        0        0   850557 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/umi.js
+-rw-r--r--   0        0        0    73464 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/codicon.589e0820.ttf
+-rw-r--r--   0        0        0    49764 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/devopicons.3c46801a.woff2
+-rw-r--r--   0        0        0    90680 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/file-icons.2cbb51ef.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.cf011583.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.e9955780.woff2
+-rw-r--r--   0        0        0   387787 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.f05dad85.svg
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/fontawesome.e9955780.woff2
+-rw-r--r--   0        0        0    24412 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/mfixx.8e0807ce.woff2
+-rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/octicons.c982f59d.woff2
+-rw-r--r--   0        0        0   466610 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/onig.25dd2e6f.wasm
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/static/static/plotly.eb7b9072.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/templates/error.html
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/templates/libro.html
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 libro-0.1.8/src/libro_server/templates/page.html
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libro-0.1.8/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 libro-0.1.8/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 libro-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 libro-0.1.8/PKG-INFO
```

### Comparing `libro-0.1.7/src/dev-config/jupyter_server_config.py` & `libro-0.1.8/src/dev-config/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/app.py` & `libro-0.1.8/src/libro_server/app.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/execution_handler.py` & `libro-0.1.8/src/libro_server/execution_handler.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static_handler.py` & `libro-0.1.8/src/libro_server/static_handler.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/100.async.js` & `libro-0.1.8/src/libro_server/static/100.async.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -541293,15 +541293,15 @@
                         return /* reexport */ isCellView;
                     },
                     QS: function() {
                         return /* reexport */ notebookViewFactoryId;
                     }
                 });
 
-                // UNUSED EXPORTS: AddCellOutlined, CellModelFactory, CellOption, CellOutputContent, CellSideToolbarVisible, CellTopToolbarSetting, CellViewOptions, ClearOutlined, CollapseServiceOption, DefaultContentContribution, DefaultEncodedFormatter, DefaultOutputContribution, DefaultSaveContentContribution, DeleteOutlined, DisableOutputScroll, DndCellContainer, DndCellItemContainer, DndCellItemContent, DndCellItemRender, DndCellRender, DndCellsRender, DndList, EnableOutputScroll, FormatCellIcon, FormatterStringContribution, FormatterTransContribution, FormatterTransDefaultContribution, HeaderToolbarVisible, HolderOutlined, LibroAddCell, LibroAddCellSlotContribution, LibroAddCellView, LibroBetweenCellContent, LibroCellComponent, LibroCellContribution, LibroCellExecutionTime, LibroCellInputBottonBlank, LibroCellVisualization, LibroCommandContribution, LibroCommandModule, LibroComponent, LibroContentComponent, LibroContentModule, LibroContentService, LibroContextKeys, LibroExtensionViewComponent, LibroFormatterManager, LibroFormatterModule, LibroOutputModel, LibroRender, LibroSideToolbarMenuInlines, LibroSlotManager, LibroSlotModule, LibroSlotView, LibroToolbarContribution, LibroUserSettingStorage, LibroUserSettingsNamespace, LibroWrappedAddCell, ModelFactory, MoreOutlined, MoveDownOutlined, MoveUpOutlined, MultiSelectionWhenShiftClick, MultipleSelectionPreviewMemo, NotebookModel, NotebookOption, OutputScrollBtnVisiable, PauseCircleOutlined, PerformaceStatisticOption, PlusOutlined, Redo, Reload, RightContentFixed, SettingsContribution, SettingsModal, SettingsModalComponent, SettingsModule, SingleSelectionPreviewMemo, SupportCodeFormat, Undo, VirtualizedManager, VirtualizedManagerOption, VirtualizedManagerOptionFactory, getLibroCellType, isDisplayView, isLibroCellModel, normalize, removeOverwrittenChars
+                // UNUSED EXPORTS: AddCellOutlined, CellModelFactory, CellOption, CellOutputContent, CellSideToolbarVisible, CellTopToolbarSetting, CellViewOptions, ClearOutlined, CollapseServiceOption, DefaultContentContribution, DefaultEncodedFormatter, DefaultOutputContribution, DefaultSaveContentContribution, DeleteOutlined, DisableOutputScroll, DndCellContainer, DndCellItemContainer, DndCellItemContent, DndCellItemRender, DndCellRender, DndCellsRender, DndList, EnableOutputScroll, FormatCellIcon, FormatterStringContribution, FormatterTransContribution, FormatterTransDefaultContribution, HeaderToolbarVisible, HolderOutlined, LibroAddCell, LibroAddCellSlotContribution, LibroAddCellView, LibroBetweenCellContent, LibroCellComponent, LibroCellContribution, LibroCellExecutionTime, LibroCellInputBottonBlank, LibroCellVisualization, LibroCommandContribution, LibroCommandModule, LibroComponent, LibroContentComponent, LibroContentModule, LibroContentService, LibroContextKeys, LibroExtensionViewComponent, LibroFormatterManager, LibroFormatterModule, LibroOutputModel, LibroRender, LibroSideToolbarMenuInlines, LibroSlotManager, LibroSlotModule, LibroSlotView, LibroToolbarContribution, LibroUserSettingStorage, LibroUserSettingsNamespace, LibroWrappedAddCell, LirboContextKey, ModelFactory, MoreOutlined, MoveDownOutlined, MoveUpOutlined, MultiSelectionWhenShiftClick, MultipleSelectionPreviewMemo, NotebookModel, NotebookOption, OutputScrollBtnVisiable, PauseCircleOutlined, PerformaceStatisticOption, PlusOutlined, Redo, Reload, RightContentFixed, SettingsContribution, SettingsModal, SettingsModalComponent, SettingsModule, SingleSelectionPreviewMemo, SupportCodeFormat, Undo, VirtualizedManager, VirtualizedManagerOption, VirtualizedManagerOptionFactory, getLibroCellType, isDisplayView, isLibroCellModel, normalize, removeOverwrittenChars
 
                 // NAMESPACE OBJECT: ./node_modules/react-dnd-html5-backend/dist/NativeTypes.js
                 var NativeTypes_namespaceObject = {};
                 __webpack_require__.r(NativeTypes_namespaceObject);
                 __webpack_require__.d(NativeTypes_namespaceObject, {
                     FILE: function() {
                         return FILE;
@@ -547170,14 +547170,18 @@
                             var _this$libroService$ac;
                             this.commandMode = this.contextKeyService.createKey(LibroContextKeys.commandMode, !!((_this$libroService$ac = this.libroService.active) !== null && _this$libroService$ac !== void 0 && _this$libroService$ac.model.commandMode));
                             this.listenToActive();
                         }
                     }]);
                     return LibroContextKey;
                 }()) || libro_context_key_class);
+                /**
+                 * @deprecated use LibroContextKey instead.
+                 */
+                var LirboContextKey = ( /* unused pure expression or super */ null && (LibroContextKey));
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/configuration/configuration-registry.js
                 var configuration_registry = __webpack_require__(73397);
                 // EXTERNAL MODULE: ./node_modules/antd/es/modal/index.js + 27 modules
                 var modal = __webpack_require__(59259);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/configuration/module.js
                 var configuration_module = __webpack_require__(17407);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/configuration/configuration-render-registry.js
@@ -589063,14 +589067,15 @@
 
 
 
 
 
 
 
+
                 /***/
             }),
 
         /***/
         24159:
             /***/
             (function(__unused_webpack___webpack_module__, __webpack_exports__, __webpack_require__) {
@@ -589197,15 +589202,15 @@
                         return /* reexport */ es /* hasErrorOutput */ .DJ;
                     },
                     CZ3: function() {
                         return /* reexport */ es /* isCellView */ .CZ;
                     }
                 });
 
-                // UNUSED EXPORTS: AbstractSearchProvider, AddCellOutlined, AdditionalCompletionTriggerKinds, ArrayIterator, ArrowDown, ArrowRight, AutoInsertWhenNoCell, BaseWorkspaceService, BetweenCellProvider, CellCollapsible, CellEditorMemo, CellExecutionTip, CellInputBottomBlank, CellModelContribution, CellModelFactory, CellOption, CellOptions, CellOutputContent, CellSearchProviderContribution, CellService, CellSideToolbarVisible, CellTopToolbarSetting, CellViewContribution, CellViewOptions, CheckCircleOutlined, ClearOutlined, CodeCellModelFactory, CodeCellModule, CodeCellSearchOption, CodeCellSearchProvider, CodeCellSearchProviderFactory, CodeEditorCellContribution, CodeEditorCellSearchProvider, CodeEditorContribution, CodeEditorManager, CodeEditorModule, CodeEditorRender, CodeEditorSearchHighlighterFactory, CodeEditorSetting, CodeEditorSettings, CodeEditorView, CodeExtractorsManager, CodeMirrorEditor, CodeMirrorEditorModule, CollapseService, CollapseServiceFactory, CollapseServiceOption, CompletionContext, CompletionItemKind, CompletionItemTag, CompletionMonitor, CompletionTriggerKind, ConfigAppContribution, ContentContribution, ContentSaveContribution, ContentsManager, DefaultCollapseService, DefaultContentContribution, DefaultEncodedFormatter, DefaultMap, DefaultOutputContribution, DefaultRenderMimeRegistry, DefaultSaveContentContribution, DeleteOutlined, DiagnosticSeverity, DiagnosticTag, DisableOutputScroll, DisplayDataOutputContribution, DisplayDataOutputModel, DisplayDataOutputModule, DisplayWrapComponent, DndCellContainer, DndCellItemContainer, DndCellItemContent, DndCellItemRender, DndCellRender, DndCellsRender, DndList, Document, DocumentCommands, DocumentConnectionManager, DocumentHighlightKind, Drive, E2EditorClassname, E2LoadedDeferred, EditorCellView, EditorConfiguration, EditorStatus, EditorView, EnableOutputScroll, EnterEditModeWhenAddCell, ErrorOutputContribution, ErrorOutputModel, ErrorOutputModule, ExecutableNotebookModel, ExecutedWithKernelCellModel, FeatureManager, FileCommands, FileCreateDirModalComponent, FileCreateModalComponent, FileDirCreateModal, FileTreeContextMenuGroups, FileTreeContextMenuPath, FileType, FormatCellIcon, FormatterStringContribution, FormatterTransContribution, FormatterTransDefaultContribution, GenericSearchProvider, GenericSearchProviderFactory, HeaderToolbarVisible, HolderOutlined, ILSPCodeExtractorsManager, ILSPDocumentConnectionManager, ILSPFeatureManager, ILSPOptions, ILanguageServerManagerFactory, ILanguageServerManagerOptions, ILibroWorkspaceService, IPoll, IRenderMimeRegistryOptions, IVirtualDocumentOptions, InfoCircle, JupyterCodeCellModel, JupyterCodeCellView, JupyterServerLaunchManager, KERNEL_SERVICE_URL, KernelCommands, KernelConnection, KernelConnectionOptions, KernelId, KernelMessage, KernelMetaOption, KernelRestAPI, KernelSelector, KernelSpecManager, KernelSpecRestAPI, KernelStatusAndSelectorProvider, KernelStatusSelector, KeybindInstructionsContribution, KeybindInstructionsIcon, KeybindInstructionsModule, KeybindInstructionsOutlined, KeybindInstrutionModal, KeybindInstrutionsComponent, KeybindInstrutionsService, LIBRO_SEARCH_FOUND_CLASSES, LIBRO_SEARCH_SELECTED_CLASSES, LSPConnection, LSPConnectionFactory, LSPMonitor, LanguageServerManager, LanguageSpecContribution, Languages, LibroAddBetweenCellCommand, LibroAddBetweenCellCommandContribution, LibroAddCell, LibroAddCellModule, LibroAddCellSlotContribution, LibroAddCellView, LibroBetweenCellContent, LibroBetweenCellModule, LibroCellComponent, LibroCellContribution, LibroCellExecutionTime, LibroCellInputBottonBlank, LibroCellModel, LibroCellView, LibroCellVisualization, LibroCodeCellModel, LibroCodeCellView, LibroCommandContribution, LibroCommandModule, LibroCommandRegister, LibroComponent, LibroConfigAllowDownload, LibroConfigAllowUpload, LibroConfigOpenSlot, LibroContentComponent, LibroContentModule, LibroContentService, LibroContentsModule, LibroContextKey, LibroContextKeys, LibroE2Editor, LibroE2EditorContribution, LibroE2EditorFactory, LibroE2EditorModule, LibroE2EditorOptions, LibroE2EditorState, LibroEditorCellView, LibroEditorComponent, LibroExecutableCellView, LibroExtensionSlotContribution, LibroExtensionViewComponent, LibroFileError, LibroFormatterManager, LibroFormatterModule, LibroJupyterColorContribution, LibroJupyterCommandContribution, LibroJupyterContentContribution, LibroJupyterFileModule, LibroJupyterFileService, LibroJupyterKeybindingContribution, LibroJupyterOpenHandler, LibroJupyterOutputArea, LibroJupyterSettingContribution, LibroJupyterToolbarContribution, LibroKernelConnectionFactory, LibroKernelConnectionManager, LibroKernelFactory, LibroKernelManageModule, LibroKernelManager, LibroKernelModule, LibroKernelSpecModule, LibroKeybindItems, LibroKeybindRegistry, LibroLSPModule, LibroLanguageSpecs, LibroMarkdownCellModel, LibroModel, LibroModule, LibroNavigatableViewFactoryId, LibroOutputArea, LibroOutputModel, LibroOutputView, LibroPlotlyMimeTypeContribution, LibroRawCellModel, LibroRawCellView, LibroRender, LibroRenderMimeModule, LibroSQLRequestAPI, LibroSearchManager, LibroSearchModule, LibroSearchToggleCommand, LibroSearchUtils, LibroSearchView, LibroServerModule, LibroSessionFactory, LibroSessionManager, LibroSessionModule, LibroSideToolbarMenu, LibroSideToolbarMenuInlines, LibroSlotManager, LibroSlotModule, LibroSlotView, LibroToolbarArea, LibroToolbarContribution, LibroToolbarModule, LibroUserSettingStorage, LibroUserSettingsNamespace, LibroView, LibroViewTracker, LibroWrappedAddCell, Location, MAJOR_VERSION, MIME, MIME_TYPE, MINOR_VERSION, MarkdownCell, MarkdownCellContribution, MarkdownCellModel, MarkdownCellModelFactory, MarkdownCellModule, MarkdownCellView, MarkdownPreview, MessageKind, Method, Model, ModelFactory, MonacoRange, MoreOutlined, MoveDownOutlined, MoveUpOutlined, MultiSelectionWhenShiftClick, MultipleSelectionPreviewMemo, NetworkError, NotebookModel, NotebookOption, NotebookService, Option, OutputContribution, OutputModule, OutputScrollBtnVisiable, PathExt, PauseCircleOutlined, PerformaceStatisticOption, PlotlyModule, PlotlyRender, PlusOutlined, Poll, ProtocolCoordinates, Provider, RawCellContribution, RawCellModelFactory, RawCellModule, Redo, Reload, RenderMimeRegistry, RenderedPlotly, ReplaceToggle, ResponseError, RightContentFixed, SESSION_SERVICE_URL, SQLIcon, Sanitizer, SaveFileErrorContribution, SaveFileErrorModal, SaveFileModalComponent, SearchCodeCellModule, SearchComponent, SearchContent, SearchIndex, SearchIndexMemo, SearchProviderOption, ServerLaunchManager, SessionId, SessionMetaOption, SessionRestAPI, SettingsContribution, SettingsModal, SettingsModalComponent, SettingsModule, SingleSelectionPreviewMemo, StreamOutputContribution, StreamOutputModel, StreamOutputModule, SupportCodeFormat, TextForeignCodeExtractor, URL, URL_NS, Undo, UpdateManager, VirtualDocument, VirtualDocumentFactory, VirtualDocumentInfo, VirtualDocumentInfoFactory, VirtualDocumentInfoOptions, VirtualizedManager, VirtualizedManagerHelper, VirtualizedManagerOption, VirtualizedManagerOptionFactory, WarningIcon, WidgetLSPAdapter, acceptCompletion, ansiSpan, applyCompletion, asSource, autocompletion, autolink, clearSnippet, closeBrackets, closeBracketsKeymap, closeCompletion, codeMirrorDefaultConfig, codeMirrorEditorFactory, collectDocuments, completeAnyWord, completeFromList, completionKeymap, completionPlugin, completionStatus, copy2clipboard, createEditor, createHeaderId, createResponseError, cur, currentCompletions, deepCopy, deepEqual, defaultConfig, defaultMimeType, defaultSanitizer, defaultSelectionStyle, defaultTheme, deleteBracketPair, e2StateFactory, each, elementInViewport, emptyArray, emptyObject, ensure, ensureAnchor, evalInnerHTMLScriptTags, expandDottedPaths, expandPath, extract, findBest, findByExtension, findByFileName, findByMIME, findByName, findFirstArrayIndex, findFirstArrayValue, findLastArrayIndex, findLastArrayValue, firstIndexOfArray, formatCell, formatContents, formatKeymap, getData, getLibroCellType, getModeInfo, getSessionUrl, getTheme, handleDefaults, handleUrls, htmlRendererFactory, ifIn, ifNotIn, imageRendererFactory, insertBracket, insertCompletionText, isArray, isClearOutputMsg, isCode, isCommCloseMsg, isCommMsgMsg, isCommOpenMsg, isDebugEventMsg, isDebugReplyMsg, isDebugRequestMsg, isDisplayData, isDisplayDataMsg, isDisplayUpdate, isDisplayView, isEqual, isError, isErrorMsg, isExecuteInputMsg, isExecuteReplyMsg, isExecuteResult, isExecuteResultMsg, isInfoRequestMsg, isInputReplyMsg, isInputRequestMsg, isLibroCellModel, isMarkdown, isObject, isOutput, isPrimitive, isRaw, isStatusMsg, isStream, isStreamMsg, isUpdateDisplayDataMsg, isWithinRange, iter, jupyterEditorTheme, jupyterHighlightStyle, jupyterServiceStatus, jupyterTheme, kernelStatus, langBundles, latexRendererFactory, libroArgsMimetype, libroE2DefaultConfig, libroVisCellLangBundles, loadE2, lowerArrayBound, lspFormat, lspLint, lspPythonCompletion, lspTooltip, markdownRendererFactory, monitorPlugin, moveCompletionSelection, nextSnippetField, normalize, notebookViewFactoryId, offsetAtPosition, offsetToPos, pickedCompletion, posToOffset, positionAtOffset, prevSnippetField, readFromClipboard, registerModeInfo, registerTheme, removeAllWhereFromArray, removeOverwrittenChars, renderHTML, renderImage, renderMarkdown, renderMarkdownContent, renderMarkupContent, renderPlotly, renderSVG, renderText, run, searchInHTML, searchText, selectedCompletion, selectedCompletionIndex, setSelectedCompletion, sleep, snippet, snippetCompletion, snippetKeymap, sortedTypes, splitShallowNode, standardRendererFactories, startCompletion, startFormatEffect, stateFactory, statusToColor, svgRendererFactory, textRendererFactory, toArray, untilReady, upperArrayBound, validateCheckpointModel, validateContentsModel, validateMimeValue
+                // UNUSED EXPORTS: AbstractSearchProvider, AddCellOutlined, AdditionalCompletionTriggerKinds, ArrayIterator, ArrowDown, ArrowRight, AutoInsertWhenNoCell, BaseWorkspaceService, BetweenCellProvider, CellCollapsible, CellEditorMemo, CellExecutionTip, CellInputBottomBlank, CellModelContribution, CellModelFactory, CellOption, CellOptions, CellOutputContent, CellSearchProviderContribution, CellService, CellSideToolbarVisible, CellTopToolbarSetting, CellViewContribution, CellViewOptions, CheckCircleOutlined, ClearOutlined, CodeCellModelFactory, CodeCellModule, CodeCellSearchOption, CodeCellSearchProvider, CodeCellSearchProviderFactory, CodeEditorCellContribution, CodeEditorCellSearchProvider, CodeEditorContribution, CodeEditorManager, CodeEditorModule, CodeEditorRender, CodeEditorSearchHighlighterFactory, CodeEditorSetting, CodeEditorSettings, CodeEditorView, CodeExtractorsManager, CodeMirrorEditor, CodeMirrorEditorModule, CollapseService, CollapseServiceFactory, CollapseServiceOption, CompletionContext, CompletionItemKind, CompletionItemTag, CompletionMonitor, CompletionTriggerKind, ConfigAppContribution, ContentContribution, ContentSaveContribution, ContentsManager, DefaultCollapseService, DefaultContentContribution, DefaultEncodedFormatter, DefaultMap, DefaultOutputContribution, DefaultRenderMimeRegistry, DefaultSaveContentContribution, DeleteOutlined, DiagnosticSeverity, DiagnosticTag, DisableOutputScroll, DisplayDataOutputContribution, DisplayDataOutputModel, DisplayDataOutputModule, DisplayWrapComponent, DndCellContainer, DndCellItemContainer, DndCellItemContent, DndCellItemRender, DndCellRender, DndCellsRender, DndList, Document, DocumentCommands, DocumentConnectionManager, DocumentHighlightKind, Drive, E2EditorClassname, E2LoadedDeferred, EditorCellView, EditorConfiguration, EditorStatus, EditorView, EnableOutputScroll, EnterEditModeWhenAddCell, ErrorOutputContribution, ErrorOutputModel, ErrorOutputModule, ExecutableNotebookModel, ExecutedWithKernelCellModel, FeatureManager, FileCommands, FileCreateDirModalComponent, FileCreateModalComponent, FileDirCreateModal, FileTreeContextMenuGroups, FileTreeContextMenuPath, FileType, FormatCellIcon, FormatterStringContribution, FormatterTransContribution, FormatterTransDefaultContribution, GenericSearchProvider, GenericSearchProviderFactory, HeaderToolbarVisible, HolderOutlined, ILSPCodeExtractorsManager, ILSPDocumentConnectionManager, ILSPFeatureManager, ILSPOptions, ILanguageServerManagerFactory, ILanguageServerManagerOptions, ILibroWorkspaceService, IPoll, IRenderMimeRegistryOptions, IVirtualDocumentOptions, InfoCircle, JupyterCodeCellModel, JupyterCodeCellView, JupyterServerLaunchManager, KERNEL_SERVICE_URL, KernelCommands, KernelConnection, KernelConnectionOptions, KernelId, KernelMessage, KernelMetaOption, KernelRestAPI, KernelSelector, KernelSpecManager, KernelSpecRestAPI, KernelStatusAndSelectorProvider, KernelStatusSelector, KeybindInstructionsContribution, KeybindInstructionsIcon, KeybindInstructionsModule, KeybindInstructionsOutlined, KeybindInstrutionModal, KeybindInstrutionsComponent, KeybindInstrutionsService, LIBRO_SEARCH_FOUND_CLASSES, LIBRO_SEARCH_SELECTED_CLASSES, LSPConnection, LSPConnectionFactory, LSPMonitor, LanguageServerManager, LanguageSpecContribution, Languages, LibroAddBetweenCellCommand, LibroAddBetweenCellCommandContribution, LibroAddCell, LibroAddCellModule, LibroAddCellSlotContribution, LibroAddCellView, LibroBetweenCellContent, LibroBetweenCellModule, LibroCellComponent, LibroCellContribution, LibroCellExecutionTime, LibroCellInputBottonBlank, LibroCellModel, LibroCellView, LibroCellVisualization, LibroCodeCellModel, LibroCodeCellView, LibroCommandContribution, LibroCommandModule, LibroCommandRegister, LibroComponent, LibroConfigAllowDownload, LibroConfigAllowUpload, LibroConfigOpenSlot, LibroContentComponent, LibroContentModule, LibroContentService, LibroContentsModule, LibroContextKey, LibroContextKeys, LibroE2Editor, LibroE2EditorContribution, LibroE2EditorFactory, LibroE2EditorModule, LibroE2EditorOptions, LibroE2EditorState, LibroEditorCellView, LibroEditorComponent, LibroExecutableCellView, LibroExtensionSlotContribution, LibroExtensionViewComponent, LibroFileError, LibroFormatterManager, LibroFormatterModule, LibroJupyterColorContribution, LibroJupyterCommandContribution, LibroJupyterContentContribution, LibroJupyterFileModule, LibroJupyterFileService, LibroJupyterKeybindingContribution, LibroJupyterOpenHandler, LibroJupyterOutputArea, LibroJupyterSettingContribution, LibroJupyterToolbarContribution, LibroKernelConnectionFactory, LibroKernelConnectionManager, LibroKernelFactory, LibroKernelManageModule, LibroKernelManager, LibroKernelModule, LibroKernelSpecModule, LibroKeybindItems, LibroKeybindRegistry, LibroLSPModule, LibroLanguageSpecs, LibroMarkdownCellModel, LibroModel, LibroModule, LibroNavigatableViewFactoryId, LibroOutputArea, LibroOutputModel, LibroOutputView, LibroPlotlyMimeTypeContribution, LibroRawCellModel, LibroRawCellView, LibroRender, LibroRenderMimeModule, LibroSQLRequestAPI, LibroSearchManager, LibroSearchModule, LibroSearchToggleCommand, LibroSearchUtils, LibroSearchView, LibroServerModule, LibroSessionFactory, LibroSessionManager, LibroSessionModule, LibroSideToolbarMenu, LibroSideToolbarMenuInlines, LibroSlotManager, LibroSlotModule, LibroSlotView, LibroToolbarArea, LibroToolbarContribution, LibroToolbarModule, LibroUserSettingStorage, LibroUserSettingsNamespace, LibroView, LibroViewTracker, LibroWrappedAddCell, LirboContextKey, Location, MAJOR_VERSION, MIME, MIME_TYPE, MINOR_VERSION, MarkdownCell, MarkdownCellContribution, MarkdownCellModel, MarkdownCellModelFactory, MarkdownCellModule, MarkdownCellView, MarkdownPreview, MessageKind, Method, Model, ModelFactory, MonacoRange, MoreOutlined, MoveDownOutlined, MoveUpOutlined, MultiSelectionWhenShiftClick, MultipleSelectionPreviewMemo, NetworkError, NotebookModel, NotebookOption, NotebookService, Option, OutputContribution, OutputModule, OutputScrollBtnVisiable, PathExt, PauseCircleOutlined, PerformaceStatisticOption, PlotlyModule, PlotlyRender, PlusOutlined, Poll, ProtocolCoordinates, Provider, RawCellContribution, RawCellModelFactory, RawCellModule, Redo, Reload, RenderMimeRegistry, RenderedPlotly, ReplaceToggle, ResponseError, RightContentFixed, SESSION_SERVICE_URL, SQLIcon, Sanitizer, SaveFileErrorContribution, SaveFileErrorModal, SaveFileModalComponent, SearchCodeCellModule, SearchComponent, SearchContent, SearchIndex, SearchIndexMemo, SearchProviderOption, ServerLaunchManager, SessionId, SessionMetaOption, SessionRestAPI, SettingsContribution, SettingsModal, SettingsModalComponent, SettingsModule, SingleSelectionPreviewMemo, StreamOutputContribution, StreamOutputModel, StreamOutputModule, SupportCodeFormat, TextForeignCodeExtractor, URL, URL_NS, Undo, UpdateManager, VirtualDocument, VirtualDocumentFactory, VirtualDocumentInfo, VirtualDocumentInfoFactory, VirtualDocumentInfoOptions, VirtualizedManager, VirtualizedManagerHelper, VirtualizedManagerOption, VirtualizedManagerOptionFactory, WarningIcon, WidgetLSPAdapter, acceptCompletion, ansiSpan, applyCompletion, asSource, autocompletion, autolink, clearSnippet, closeBrackets, closeBracketsKeymap, closeCompletion, codeMirrorDefaultConfig, codeMirrorEditorFactory, collectDocuments, completeAnyWord, completeFromList, completionKeymap, completionPlugin, completionStatus, copy2clipboard, createEditor, createHeaderId, createResponseError, cur, currentCompletions, deepCopy, deepEqual, defaultConfig, defaultMimeType, defaultSanitizer, defaultSelectionStyle, defaultTheme, deleteBracketPair, e2StateFactory, each, elementInViewport, emptyArray, emptyObject, ensure, ensureAnchor, evalInnerHTMLScriptTags, expandDottedPaths, expandPath, extract, findBest, findByExtension, findByFileName, findByMIME, findByName, findFirstArrayIndex, findFirstArrayValue, findLastArrayIndex, findLastArrayValue, firstIndexOfArray, formatCell, formatContents, formatKeymap, getData, getLibroCellType, getModeInfo, getSessionUrl, getTheme, handleDefaults, handleUrls, htmlRendererFactory, ifIn, ifNotIn, imageRendererFactory, insertBracket, insertCompletionText, isArray, isClearOutputMsg, isCode, isCommCloseMsg, isCommMsgMsg, isCommOpenMsg, isDebugEventMsg, isDebugReplyMsg, isDebugRequestMsg, isDisplayData, isDisplayDataMsg, isDisplayUpdate, isDisplayView, isEqual, isError, isErrorMsg, isExecuteInputMsg, isExecuteReplyMsg, isExecuteResult, isExecuteResultMsg, isInfoRequestMsg, isInputReplyMsg, isInputRequestMsg, isLibroCellModel, isMarkdown, isObject, isOutput, isPrimitive, isRaw, isStatusMsg, isStream, isStreamMsg, isUpdateDisplayDataMsg, isWithinRange, iter, jupyterEditorTheme, jupyterHighlightStyle, jupyterServiceStatus, jupyterTheme, kernelStatus, langBundles, latexRendererFactory, libroArgsMimetype, libroE2DefaultConfig, libroVisCellLangBundles, loadE2, lowerArrayBound, lspFormat, lspLint, lspPythonCompletion, lspTooltip, markdownRendererFactory, monitorPlugin, moveCompletionSelection, nextSnippetField, normalize, notebookViewFactoryId, offsetAtPosition, offsetToPos, pickedCompletion, posToOffset, positionAtOffset, prevSnippetField, readFromClipboard, registerModeInfo, registerTheme, removeAllWhereFromArray, removeOverwrittenChars, renderHTML, renderImage, renderMarkdown, renderMarkdownContent, renderMarkupContent, renderPlotly, renderSVG, renderText, run, searchInHTML, searchText, selectedCompletion, selectedCompletionIndex, setSelectedCompletion, sleep, snippet, snippetCompletion, snippetKeymap, sortedTypes, splitShallowNode, standardRendererFactories, startCompletion, startFormatEffect, stateFactory, statusToColor, svgRendererFactory, textRendererFactory, toArray, untilReady, upperArrayBound, validateCheckpointModel, validateContentsModel, validateMimeValue
 
                 // EXTERNAL MODULE: ./node_modules/@difizen/libro-core/es/index.js + 273 modules
                 var es = __webpack_require__(59445);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-syringe/es/index.js + 15 modules
                 var mana_syringe_es = __webpack_require__(49383);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-code-cell/es/code-cell-protocol.js
                 var CodeCellModelFactory = Symbol('CodeCellModelFactory');
                 // EXTERNAL MODULE: ./node_modules/@difizen/libro-code-editor/es/index.js + 9 modules
@@ -812467,18 +812472,19 @@
                             }
                             return handleCommOpen;
                         }())
                     }, {
                         key: "registerWidgetView",
                         value: function registerWidgetView(model_id, model) {
                             var _this2 = this;
-                            model.then(function(WidgetView) {
-                                _this2.models.set(model_id, WidgetView);
+                            model.then(function(model) {
+                                _this2.models.set(model_id, model);
+                                _this2.models.set(model.toModelKey(), model);
                                 _this2.widgetEmitter.fire({
-                                    WidgetViewName: WidgetView.model_name
+                                    WidgetViewName: model.model_name
                                 });
                                 return;
                             }).catch(function() {
                                 //
                             });
                         }
                     }, {
@@ -812510,15 +812516,16 @@
                                             }
                                             throw new Error('Neither comm nor model_id provided in options object. At least one must exist.');
                                         case 3:
                                             options.model_id = model_id;
                                             provider = this.findProvider(attributes);
                                             WidgetView = provider.factory({
                                                 attributes: attributes,
-                                                options: options
+                                                options: options,
+                                                widgetsId: this.id
                                             });
                                             this.registerWidgetView(model_id, WidgetView);
                                             return _context4.abrupt("return", WidgetView);
                                         case 8:
                                         case "end":
                                             return _context4.stop();
                                     }
@@ -812544,14 +812551,27 @@
                          * as dead.
                          */
                     }, {
                         key: "disconnect",
                         value: function disconnect() {
                             // this.models.forEach(model => model.clear());
                         }
+                    }, {
+                        key: "toJSON",
+                        value:
+                            /**
+                             * Serialize the model.  See the deserialization function at the top of this file
+                             * and the kernel-side serializer/deserializer.
+                             */
+                            function toJSON() {
+                                return JSON.stringify({
+                                    kc_id: this.kernelConnection.id,
+                                    id: this.id
+                                });
+                            }
                     }]);
                     return LibroWidgets;
                 }(), (_descriptor = _applyDecoratedDescriptor(_class2.prototype, "WidgetViewProvider", [_dec2], {
                     configurable: true,
                     enumerable: true,
                     writable: true,
                     initializer: null
@@ -812566,24 +812586,193 @@
                 // EXTERNAL MODULE: ./node_modules/@difizen/libro-core/es/index.js + 273 modules
                 var libro_core_es = __webpack_require__(59445);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/view/decorator.js
                 var decorator = __webpack_require__(64424);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/view/view-protocol.js
                 var view_protocol = __webpack_require__(45573);
                 // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/view/default-view.js + 1 modules
-                var default_view = __webpack_require__(58304);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/widget-view.js
+                var default_view = __webpack_require__(58304);
+                // EXTERNAL MODULE: ./node_modules/@difizen/libro-kernel/es/index.js + 41 modules
+                var libro_kernel_es = __webpack_require__(11716);
+                // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/application/application.js
+                var application = __webpack_require__(15910);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/widget-manager.js
+                function widget_manager_typeof(o) {
+                    "@babel/helpers - typeof";
+                    return widget_manager_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(o) {
+                        return typeof o;
+                    } : function(o) {
+                        return o && "function" == typeof Symbol && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o;
+                    }, widget_manager_typeof(o);
+                }
+                var widget_manager_dec, widget_manager_dec2, widget_manager_dec3, _dec4, _dec5, widget_manager_class, widget_manager_class2, widget_manager_descriptor, widget_manager_descriptor2, _descriptor3, _descriptor4;
+
+                function widget_manager_initializerDefineProperty(target, property, descriptor, context) {
+                    if (!descriptor) return;
+                    Object.defineProperty(target, property, {
+                        enumerable: descriptor.enumerable,
+                        configurable: descriptor.configurable,
+                        writable: descriptor.writable,
+                        value: descriptor.initializer ? descriptor.initializer.call(context) : void 0
+                    });
+                }
+
+                function widget_manager_classCallCheck(instance, Constructor) {
+                    if (!(instance instanceof Constructor)) {
+                        throw new TypeError("Cannot call a class as a function");
+                    }
+                }
+
+                function widget_manager_defineProperties(target, props) {
+                    for (var i = 0; i < props.length; i++) {
+                        var descriptor = props[i];
+                        descriptor.enumerable = descriptor.enumerable || false;
+                        descriptor.configurable = true;
+                        if ("value" in descriptor) descriptor.writable = true;
+                        Object.defineProperty(target, widget_manager_toPropertyKey(descriptor.key), descriptor);
+                    }
+                }
+
+                function widget_manager_createClass(Constructor, protoProps, staticProps) {
+                    if (protoProps) widget_manager_defineProperties(Constructor.prototype, protoProps);
+                    if (staticProps) widget_manager_defineProperties(Constructor, staticProps);
+                    Object.defineProperty(Constructor, "prototype", {
+                        writable: false
+                    });
+                    return Constructor;
+                }
+
+                function widget_manager_toPropertyKey(t) {
+                    var i = widget_manager_toPrimitive(t, "string");
+                    return "symbol" == widget_manager_typeof(i) ? i : String(i);
+                }
+
+                function widget_manager_toPrimitive(t, r) {
+                    if ("object" != widget_manager_typeof(t) || !t) return t;
+                    var e = t[Symbol.toPrimitive];
+                    if (void 0 !== e) {
+                        var i = e.call(t, r || "default");
+                        if ("object" != widget_manager_typeof(i)) return i;
+                        throw new TypeError("@@toPrimitive must return a primitive value.");
+                    }
+                    return ("string" === r ? String : Number)(t);
+                }
+
+                function widget_manager_applyDecoratedDescriptor(target, property, decorators, descriptor, context) {
+                    var desc = {};
+                    Object.keys(descriptor).forEach(function(key) {
+                        desc[key] = descriptor[key];
+                    });
+                    desc.enumerable = !!desc.enumerable;
+                    desc.configurable = !!desc.configurable;
+                    if ('value' in desc || desc.initializer) {
+                        desc.writable = true;
+                    }
+                    desc = decorators.slice().reverse().reduce(function(desc, decorator) {
+                        return decorator(target, property, desc) || desc;
+                    }, desc);
+                    if (context && desc.initializer !== void 0) {
+                        desc.value = desc.initializer ? desc.initializer.call(context) : void 0;
+                        desc.initializer = undefined;
+                    }
+                    if (desc.initializer === void 0) {
+                        Object.defineProperty(target, property, desc);
+                        desc = null;
+                    }
+                    return desc;
+                }
+
+                function widget_manager_initializerWarningHelper(descriptor, context) {
+                    throw new Error('Decorating class property failed. Please ensure that ' + 'transform-class-properties is enabled and runs after the decorators transform.');
+                }
+
+
+
+
+                var LibroWidgetManager = (widget_manager_dec = (0, mana_syringe_es /* singleton */ .ri)({
+                    contrib: application /* ApplicationContribution */ .rS
+                }), widget_manager_dec2 = (0, mana_syringe_es /* inject */ .f3)(LibroWidgetsFactory), widget_manager_dec3 = (0, mana_syringe_es /* inject */ .f3)(libro_kernel_es /* LibroKernelManager */ .uc), _dec4 = (0, mana_syringe_es /* inject */ .f3)(libro_core_es /* LibroService */ .W$), _dec5 = (0, mana_observable_es /* prop */ .vg)(), widget_manager_dec(widget_manager_class = (widget_manager_class2 = /*#__PURE__*/ function() {
+                    function LibroWidgetManager() {
+                        var _this = this;
+                        widget_manager_classCallCheck(this, LibroWidgetManager);
+                        widget_manager_initializerDefineProperty(this, "widgetsFactory", widget_manager_descriptor, this);
+                        widget_manager_initializerDefineProperty(this, "kernelManager", widget_manager_descriptor2, this);
+                        widget_manager_initializerDefineProperty(this, "libroService", _descriptor3, this);
+                        this.initialize = function() {
+                            _this.kernelManager.onConnectToKernel(function(kc) {
+                                if (kc instanceof libro_kernel_es /* KernelConnection */ .Ye) {
+                                    _this.getOrCreateWidgets(kc);
+                                }
+                            });
+                        };
+                        this.getOrCreateWidgets = function(kc) {
+                            var widgets = _this.widgets.get(kc.id);
+                            if (widgets) {
+                                return widgets;
+                            }
+                            var newWidgets = _this.widgetsFactory({
+                                kc: kc,
+                                id: kc.id
+                            });
+                            _this.widgets.set(kc.id, newWidgets);
+                            return newWidgets;
+                        };
+                        /**
+                         * Dictionary of model ids and model instance promises
+                         */
+                        widget_manager_initializerDefineProperty(this, "widgets", _descriptor4, this);
+                    }
+                    widget_manager_createClass(LibroWidgetManager, [{
+                        key: "getWidgets",
+                        value: function getWidgets(id) {
+                            return this.widgets.get(id);
+                        }
+                    }]);
+                    return LibroWidgetManager;
+                }(), (widget_manager_descriptor = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "widgetsFactory", [widget_manager_dec2], {
+                    configurable: true,
+                    enumerable: true,
+                    writable: true,
+                    initializer: null
+                }), widget_manager_descriptor2 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "kernelManager", [widget_manager_dec3], {
+                    configurable: true,
+                    enumerable: true,
+                    writable: true,
+                    initializer: null
+                }), _descriptor3 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "libroService", [_dec4], {
+                    configurable: true,
+                    enumerable: true,
+                    writable: true,
+                    initializer: null
+                }), _descriptor4 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "widgets", [_dec5], {
+                    configurable: true,
+                    enumerable: true,
+                    writable: true,
+                    initializer: function initializer() {
+                        return new Map();
+                    }
+                })), widget_manager_class2)) || widget_manager_class);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/widget-view.js
                 function widget_view_typeof(o) {
                     "@babel/helpers - typeof";
                     return widget_view_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(o) {
                         return typeof o;
                     } : function(o) {
                         return o && "function" == typeof Symbol && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o;
                     }, widget_view_typeof(o);
                 }
-                var widget_view_dec, widget_view_dec2, widget_view_class;
+                var widget_view_dec, widget_view_dec2, widget_view_dec3, widget_view_dec4, widget_view_dec5, _dec6, widget_view_class, widget_view_class2, widget_view_descriptor, widget_view_descriptor2, widget_view_descriptor3, widget_view_descriptor4;
+
+                function widget_view_initializerDefineProperty(target, property, descriptor, context) {
+                    if (!descriptor) return;
+                    Object.defineProperty(target, property, {
+                        enumerable: descriptor.enumerable,
+                        configurable: descriptor.configurable,
+                        writable: descriptor.writable,
+                        value: descriptor.initializer ? descriptor.initializer.call(context) : void 0
+                    });
+                }
 
                 function widget_view_classCallCheck(instance, Constructor) {
                     if (!(instance instanceof Constructor)) {
                         throw new TypeError("Cannot call a class as a function");
                     }
                 }
 
@@ -812693,54 +812882,88 @@
                 function _getPrototypeOf(o) {
                     _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function _getPrototypeOf(o) {
                         return o.__proto__ || Object.getPrototypeOf(o);
                     };
                     return _getPrototypeOf(o);
                 }
 
+                function widget_view_applyDecoratedDescriptor(target, property, decorators, descriptor, context) {
+                    var desc = {};
+                    Object.keys(descriptor).forEach(function(key) {
+                        desc[key] = descriptor[key];
+                    });
+                    desc.enumerable = !!desc.enumerable;
+                    desc.configurable = !!desc.configurable;
+                    if ('value' in desc || desc.initializer) {
+                        desc.writable = true;
+                    }
+                    desc = decorators.slice().reverse().reduce(function(desc, decorator) {
+                        return decorator(target, property, desc) || desc;
+                    }, desc);
+                    if (context && desc.initializer !== void 0) {
+                        desc.value = desc.initializer ? desc.initializer.call(context) : void 0;
+                        desc.initializer = undefined;
+                    }
+                    if (desc.initializer === void 0) {
+                        Object.defineProperty(target, property, desc);
+                        desc = null;
+                    }
+                    return desc;
+                }
+
+                function widget_view_initializerWarningHelper(descriptor, context) {
+                    throw new Error('Decorating class property failed. Please ensure that ' + 'transform-class-properties is enabled and runs after the decorators transform.');
+                }
+
+
 
 
 
 
 
                 var LibroWidgetComponent = /*#__PURE__*/ (0, react.forwardRef)(function LibroWidgetComponent() {
                     return /*#__PURE__*/ (0, jsx_runtime.jsx)(jsx_runtime.Fragment, {});
                 });
-                var WidgetView = (widget_view_dec = (0, mana_syringe_es /* transient */ .H3)(), widget_view_dec2 = (0, decorator /* view */ .ei)('libro-widget-view'), widget_view_dec(widget_view_class = widget_view_dec2(widget_view_class = /*#__PURE__*/ function(_BaseView) {
+                var WidgetView = (widget_view_dec = (0, mana_syringe_es /* transient */ .H3)(), widget_view_dec2 = (0, decorator /* view */ .ei)('libro-widget-view'), widget_view_dec3 = (0, mana_syringe_es /* inject */ .f3)(LibroWidgetManager), widget_view_dec4 = (0, mana_observable_es /* prop */ .vg)(), widget_view_dec5 = (0, mana_observable_es /* prop */ .vg)(), _dec6 = (0, mana_observable_es /* prop */ .vg)(), widget_view_dec(widget_view_class = widget_view_dec2(widget_view_class = (widget_view_class2 = /*#__PURE__*/ function(_BaseView) {
                     _inherits(WidgetView, _BaseView);
                     var _super = _createSuper(WidgetView);
 
                     function WidgetView(props, libroContextKey) {
                         var _this;
                         widget_view_classCallCheck(this, WidgetView);
                         _this = _super.call(this);
                         _this.view = LibroWidgetComponent;
+                        widget_view_initializerDefineProperty(_this, "libroWidgetManager", widget_view_descriptor, _assertThisInitialized(_this));
                         _this.disableCommandMode = true;
                         _this.handleCommClosed = function() {
                             _this.isCommClosed = true;
                         };
                         /**
                          * Send a custom msg over the comm.
                          */
                         _this.send = function(data, callbacks, buffers) {
                             if (_this.comm !== undefined) {
                                 _this.comm.send(data, callbacks, {}, buffers);
                             }
                         };
+                        widget_view_initializerDefineProperty(_this, "widgets", widget_view_descriptor2, _assertThisInitialized(_this));
                         _this.isCommClosed = false;
+                        widget_view_initializerDefineProperty(_this, "tabbable", widget_view_descriptor3, _assertThisInitialized(_this));
+                        widget_view_initializerDefineProperty(_this, "tooltip", widget_view_descriptor4, _assertThisInitialized(_this));
                         _this.initialize(props);
                         _this.libroContextKey = libroContextKey;
                         return _this;
                     }
                     WidgetView = (0, mana_syringe_es /* inject */ .f3)(libro_core_es /* LibroContextKey */ .z4)(WidgetView, undefined, 1) || WidgetView;
                     WidgetView = (0, mana_syringe_es /* inject */ .f3)(view_protocol /* ViewOption */ .Hj)(WidgetView, undefined, 0) || WidgetView;
                     widget_view_createClass(WidgetView, [{
                         key: "onViewMount",
                         value: function onViewMount() {
                             var _this2 = this;
+                            this.widgets = this.libroWidgetManager.getWidgets(this.widgetsId);
                             if (this.container && this.container.current && this.disableCommandMode) {
                                 this.container.current.addEventListener('focusin', function() {
                                     _this2.libroContextKey.disableCommandMode();
                                 });
                                 this.container.current.addEventListener('blur', function(e) {
                                     var _this2$container;
                                     if ((_this2$container = _this2.container) !== null && _this2$container !== void 0 && (_this2$container = _this2$container.current) !== null && _this2$container !== void 0 && _this2$container.contains(e.relatedTarget)) {
@@ -812750,37 +812973,47 @@
                                     }
                                 });
                             }
                         }
                     }, {
                         key: "initialize",
                         value: function initialize(props) {
-                            this.model_module = props.attributes._model_module;
-                            this.model_name = props.attributes._model_name;
-                            this.model_module_version = props.attributes._model_module_version;
-                            this.view_module = props.attributes._view_module;
-                            this.view_name = props.attributes._view_name;
-                            this.view_module_version = props.attributes._view_module_version;
-                            this.view_count = props.attributes._view_count;
+                            this.widgetsId = props.widgetsId;
+                            var attributes = props.attributes;
+                            this.model_module = attributes._model_module;
+                            this.model_name = attributes._model_name;
+                            this.model_module_version = attributes._model_module_version;
+                            this.view_module = attributes._view_module;
+                            this.view_name = attributes._view_name;
+                            this.view_module_version = attributes._view_module_version;
+                            this.view_count = attributes._view_count;
 
                             // Attributes should be initialized here, since user initialization may depend on it
-                            // this.libroWidgets = props.options.libroWidgets;
                             var comm = props.options.comm;
                             if (comm) {
                                 // Remember comm associated with the model.
                                 this.comm = comm;
 
                                 // Hook comm messages up to model.
                                 comm.on_close(this.handleCommClosed.bind(this));
                                 comm.on_msg(this.handleCommMsg.bind(this));
                             } else {
                                 this.isCommClosed = false;
                             }
                             this.model_id = props.options.model_id;
                             this.state_change = Promise.resolve();
+                            this.trySetValue(attributes, 'tabbable');
+                            this.trySetValue(attributes, 'tooltip');
+                        }
+                    }, {
+                        key: "trySetValue",
+                        value: function trySetValue(attributes, propKey) {
+                            if (propKey in attributes && attributes[propKey] !== undefined) {
+                                this[propKey] = attributes[propKey];
+                            }
                         }
 
                         /**
                          * Handle incoming comm msg.
                          */
                     }, {
                         key: "handleCommMsg",
@@ -812811,169 +813044,48 @@
                         /**
                          * Serialize the model.  See the deserialization function at the top of this file
                          * and the kernel-side serializer/deserializer.
                          */
                     }, {
                         key: "toJSON",
                         value: function toJSON() {
+                            return this.toModelKey();
+                        }
+                    }, {
+                        key: "toModelKey",
+                        value: function toModelKey() {
                             return "IPY_MODEL_".concat(this.model_id);
                         }
                     }]);
                     return WidgetView;
-                }(default_view /* BaseView */ .P)) || widget_view_class) || widget_view_class);
-                // EXTERNAL MODULE: ./node_modules/@difizen/libro-kernel/es/index.js + 41 modules
-                var libro_kernel_es = __webpack_require__(11716);
-                // EXTERNAL MODULE: ./node_modules/@difizen/mana-core/es/application/application.js
-                var application = __webpack_require__(15910);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/widget-manager.js
-                function widget_manager_typeof(o) {
-                    "@babel/helpers - typeof";
-                    return widget_manager_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(o) {
-                        return typeof o;
-                    } : function(o) {
-                        return o && "function" == typeof Symbol && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o;
-                    }, widget_manager_typeof(o);
-                }
-                var widget_manager_dec, widget_manager_dec2, widget_manager_dec3, _dec4, _dec5, widget_manager_class, widget_manager_class2, widget_manager_descriptor, widget_manager_descriptor2, _descriptor3, _descriptor4;
-
-                function widget_manager_initializerDefineProperty(target, property, descriptor, context) {
-                    if (!descriptor) return;
-                    Object.defineProperty(target, property, {
-                        enumerable: descriptor.enumerable,
-                        configurable: descriptor.configurable,
-                        writable: descriptor.writable,
-                        value: descriptor.initializer ? descriptor.initializer.call(context) : void 0
-                    });
-                }
-
-                function widget_manager_defineProperties(target, props) {
-                    for (var i = 0; i < props.length; i++) {
-                        var descriptor = props[i];
-                        descriptor.enumerable = descriptor.enumerable || false;
-                        descriptor.configurable = true;
-                        if ("value" in descriptor) descriptor.writable = true;
-                        Object.defineProperty(target, widget_manager_toPropertyKey(descriptor.key), descriptor);
-                    }
-                }
-
-                function widget_manager_createClass(Constructor, protoProps, staticProps) {
-                    if (protoProps) widget_manager_defineProperties(Constructor.prototype, protoProps);
-                    if (staticProps) widget_manager_defineProperties(Constructor, staticProps);
-                    Object.defineProperty(Constructor, "prototype", {
-                        writable: false
-                    });
-                    return Constructor;
-                }
-
-                function widget_manager_toPropertyKey(t) {
-                    var i = widget_manager_toPrimitive(t, "string");
-                    return "symbol" == widget_manager_typeof(i) ? i : String(i);
-                }
-
-                function widget_manager_toPrimitive(t, r) {
-                    if ("object" != widget_manager_typeof(t) || !t) return t;
-                    var e = t[Symbol.toPrimitive];
-                    if (void 0 !== e) {
-                        var i = e.call(t, r || "default");
-                        if ("object" != widget_manager_typeof(i)) return i;
-                        throw new TypeError("@@toPrimitive must return a primitive value.");
-                    }
-                    return ("string" === r ? String : Number)(t);
-                }
-
-                function widget_manager_classCallCheck(instance, Constructor) {
-                    if (!(instance instanceof Constructor)) {
-                        throw new TypeError("Cannot call a class as a function");
-                    }
-                }
-
-                function widget_manager_applyDecoratedDescriptor(target, property, decorators, descriptor, context) {
-                    var desc = {};
-                    Object.keys(descriptor).forEach(function(key) {
-                        desc[key] = descriptor[key];
-                    });
-                    desc.enumerable = !!desc.enumerable;
-                    desc.configurable = !!desc.configurable;
-                    if ('value' in desc || desc.initializer) {
-                        desc.writable = true;
-                    }
-                    desc = decorators.slice().reverse().reduce(function(desc, decorator) {
-                        return decorator(target, property, desc) || desc;
-                    }, desc);
-                    if (context && desc.initializer !== void 0) {
-                        desc.value = desc.initializer ? desc.initializer.call(context) : void 0;
-                        desc.initializer = undefined;
-                    }
-                    if (desc.initializer === void 0) {
-                        Object.defineProperty(target, property, desc);
-                        desc = null;
-                    }
-                    return desc;
-                }
-
-                function widget_manager_initializerWarningHelper(descriptor, context) {
-                    throw new Error('Decorating class property failed. Please ensure that ' + 'transform-class-properties is enabled and runs after the decorators transform.');
-                }
-
-
-
-
-                var LibroWidgetManager = (widget_manager_dec = (0, mana_syringe_es /* singleton */ .ri)({
-                    contrib: application /* ApplicationContribution */ .rS
-                }), widget_manager_dec2 = (0, mana_syringe_es /* inject */ .f3)(LibroWidgetsFactory), widget_manager_dec3 = (0, mana_syringe_es /* inject */ .f3)(libro_kernel_es /* LibroKernelManager */ .uc), _dec4 = (0, mana_syringe_es /* inject */ .f3)(libro_core_es /* LibroService */ .W$), _dec5 = (0, mana_observable_es /* prop */ .vg)(), widget_manager_dec(widget_manager_class = (widget_manager_class2 = /*#__PURE__*/ widget_manager_createClass(function LibroWidgetManager() {
-                    var _this = this;
-                    widget_manager_classCallCheck(this, LibroWidgetManager);
-                    widget_manager_initializerDefineProperty(this, "widgetsFactory", widget_manager_descriptor, this);
-                    widget_manager_initializerDefineProperty(this, "kernelManager", widget_manager_descriptor2, this);
-                    widget_manager_initializerDefineProperty(this, "libroService", _descriptor3, this);
-                    this.initialize = function() {
-                        _this.kernelManager.onConnectToKernel(function(kc) {
-                            if (kc instanceof libro_kernel_es /* KernelConnection */ .Ye) {
-                                _this.getOrCreateWidgets(kc);
-                            }
-                        });
-                    };
-                    this.getOrCreateWidgets = function(kc) {
-                        var widgets = _this.widgets.get(kc.id);
-                        if (widgets) {
-                            return widgets;
-                        }
-                        var newWidgets = _this.widgetsFactory({
-                            kc: kc,
-                            id: kc.id
-                        });
-                        _this.widgets.set(kc.id, newWidgets);
-                        return newWidgets;
-                    };
-                    /**
-                     * Dictionary of model ids and model instance promises
-                     */
-                    widget_manager_initializerDefineProperty(this, "widgets", _descriptor4, this);
-                }), (widget_manager_descriptor = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "widgetsFactory", [widget_manager_dec2], {
+                }(default_view /* BaseView */ .P), (widget_view_descriptor = widget_view_applyDecoratedDescriptor(widget_view_class2.prototype, "libroWidgetManager", [widget_view_dec3], {
                     configurable: true,
                     enumerable: true,
                     writable: true,
                     initializer: null
-                }), widget_manager_descriptor2 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "kernelManager", [widget_manager_dec3], {
+                }), widget_view_descriptor2 = widget_view_applyDecoratedDescriptor(widget_view_class2.prototype, "widgets", [widget_view_dec4], {
                     configurable: true,
                     enumerable: true,
                     writable: true,
                     initializer: null
-                }), _descriptor3 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "libroService", [_dec4], {
+                }), widget_view_descriptor3 = widget_view_applyDecoratedDescriptor(widget_view_class2.prototype, "tabbable", [widget_view_dec5], {
                     configurable: true,
                     enumerable: true,
                     writable: true,
-                    initializer: null
-                }), _descriptor4 = widget_manager_applyDecoratedDescriptor(widget_manager_class2.prototype, "widgets", [_dec5], {
+                    initializer: function initializer() {
+                        return null;
+                    }
+                }), widget_view_descriptor4 = widget_view_applyDecoratedDescriptor(widget_view_class2.prototype, "tooltip", [_dec6], {
                     configurable: true,
                     enumerable: true,
                     writable: true,
                     initializer: function initializer() {
-                        return new Map();
+                        return null;
                     }
-                })), widget_manager_class2)) || widget_manager_class);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/comm.js
+                })), widget_view_class2)) || widget_view_class) || widget_view_class);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/base/comm.js
                 function comm_typeof(o) {
                     "@babel/helpers - typeof";
                     return comm_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(o) {
                         return typeof o;
                     } : function(o) {
                         return o && "function" == typeof Symbol && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o;
                     }, comm_typeof(o);
@@ -813420,15 +813532,14 @@
                 }
 
 
 
 
 
 
-
                 var HBoxWidgetComponent = /*#__PURE__*/ (0, react.forwardRef)(function HBoxWidgetComponent() {
                     var widgetView = (0, mana_observable_es /* useInject */ .oC)(view_protocol /* ViewInstance */ .yd);
                     if (widgetView.isCommClosed) {
                         return null;
                     }
                     var hboxChildrenWidget = widgetView.get_child_model();
                     return /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {
@@ -813440,37 +813551,35 @@
                         })
                     });
                 });
                 var HBoxWidget = (hbox_widget_view_dec = (0, mana_syringe_es /* transient */ .H3)(), hbox_widget_view_dec2 = (0, decorator /* view */ .ei)('libro-hbox-widget-view'), hbox_widget_view_dec(hbox_widget_view_class = hbox_widget_view_dec2(hbox_widget_view_class = /*#__PURE__*/ function(_WidgetView) {
                     hbox_widget_view_inherits(HBoxWidget, _WidgetView);
                     var _super = hbox_widget_view_createSuper(HBoxWidget);
 
-                    function HBoxWidget(props, libroContextKey, libroWidgets) {
+                    function HBoxWidget(props, libroContextKey) {
                         var _this;
                         hbox_widget_view_classCallCheck(this, HBoxWidget);
                         _this = _super.call(this, props, libroContextKey);
                         _this.view = HBoxWidgetComponent;
                         _this.box_style = props.attributes.bar_style;
                         _this.layout = props.attributes.layout;
                         _this.children = props.attributes.children;
                         _this.libroContextKey = libroContextKey;
-                        _this.libroWidgets = libroWidgets;
                         return _this;
                     }
-                    HBoxWidget = (0, mana_syringe_es /* inject */ .f3)(LibroWidgets)(HBoxWidget, undefined, 2) || HBoxWidget;
                     HBoxWidget = (0, mana_syringe_es /* inject */ .f3)(libro_core_es /* LibroContextKey */ .z4)(HBoxWidget, undefined, 1) || HBoxWidget;
                     HBoxWidget = (0, mana_syringe_es /* inject */ .f3)(view_protocol /* ViewOption */ .Hj)(HBoxWidget, undefined, 0) || HBoxWidget;
                     hbox_widget_view_createClass(HBoxWidget, [{
                         key: "get_child_model",
                         value: function get_child_model() {
                             var _this2 = this;
                             var childrenWidgets = [];
                             this.children.forEach(function(child) {
-                                if (_this2.libroWidgets.hasModel(child.substring(10))) {
-                                    childrenWidgets.push(_this2.libroWidgets.getModel(child.substring(10)));
+                                if (_this2.widgets.hasModel(child.substring(10))) {
+                                    childrenWidgets.push(_this2.widgets.getModel(child.substring(10)));
                                 }
                             });
                             return childrenWidgets;
                         }
                     }]);
                     return HBoxWidget;
                 }(WidgetView)) || hbox_widget_view_class) || hbox_widget_view_class);; // CONCATENATED MODULE: ./node_modules/@difizen/libro-widget/es/widgets/hbox-widget-view-contribution.js
```

### Comparing `libro-0.1.7/src/libro_server/static/100.chunk.css` & `libro-0.1.8/src/libro_server/static/100.chunk.css`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/1330.async.js` & `libro-0.1.8/src/libro_server/static/1330.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/1438.async.js` & `libro-0.1.8/src/libro_server/static/1438.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/161.async.js` & `libro-0.1.8/src/libro_server/static/161.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/1639.async.js` & `libro-0.1.8/src/libro_server/static/1639.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/1772.async.js` & `libro-0.1.8/src/libro_server/static/1772.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/1838.async.js` & `libro-0.1.8/src/libro_server/static/1838.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/2048.async.js` & `libro-0.1.8/src/libro_server/static/2048.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/2118.async.js` & `libro-0.1.8/src/libro_server/static/2118.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/2130.async.js` & `libro-0.1.8/src/libro_server/static/2130.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/2999.async.js` & `libro-0.1.8/src/libro_server/static/2999.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/3572.async.js` & `libro-0.1.8/src/libro_server/static/3572.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/405.async.js` & `libro-0.1.8/src/libro_server/static/405.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4116.async.js` & `libro-0.1.8/src/libro_server/static/4116.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4123.async.js` & `libro-0.1.8/src/libro_server/static/4123.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/417.async.js` & `libro-0.1.8/src/libro_server/static/417.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4266.async.js` & `libro-0.1.8/src/libro_server/static/4266.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4343.async.js` & `libro-0.1.8/src/libro_server/static/4343.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4541.async.js` & `libro-0.1.8/src/libro_server/static/4541.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4621.async.js` & `libro-0.1.8/src/libro_server/static/4621.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4658.async.js` & `libro-0.1.8/src/libro_server/static/4658.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4849.async.js` & `libro-0.1.8/src/libro_server/static/4849.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/4887.async.js` & `libro-0.1.8/src/libro_server/static/4887.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/5250.async.js` & `libro-0.1.8/src/libro_server/static/5250.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/5332.async.js` & `libro-0.1.8/src/libro_server/static/5332.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/610.async.js` & `libro-0.1.8/src/libro_server/static/610.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/628.async.js` & `libro-0.1.8/src/libro_server/static/628.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6357.async.js` & `libro-0.1.8/src/libro_server/static/6357.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6404.async.js` & `libro-0.1.8/src/libro_server/static/6404.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6486.async.js` & `libro-0.1.8/src/libro_server/static/6486.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6730.async.js` & `libro-0.1.8/src/libro_server/static/6730.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6962.async.js` & `libro-0.1.8/src/libro_server/static/6962.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/6999.async.js` & `libro-0.1.8/src/libro_server/static/6999.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/7162.async.js` & `libro-0.1.8/src/libro_server/static/7162.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/7715.async.js` & `libro-0.1.8/src/libro_server/static/7715.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/7851.async.js` & `libro-0.1.8/src/libro_server/static/7851.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/79.async.js` & `libro-0.1.8/src/libro_server/static/79.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/8227.async.js` & `libro-0.1.8/src/libro_server/static/8227.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/8305.async.js` & `libro-0.1.8/src/libro_server/static/8305.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/8370.async.js` & `libro-0.1.8/src/libro_server/static/8370.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/8525.async.js` & `libro-0.1.8/src/libro_server/static/8525.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/8945.chunk.css` & `libro-0.1.8/src/libro_server/static/8945.chunk.css`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9095.async.js` & `libro-0.1.8/src/libro_server/static/9095.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9150.async.js` & `libro-0.1.8/src/libro_server/static/9150.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9402.async.js` & `libro-0.1.8/src/libro_server/static/9402.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9669.async.js` & `libro-0.1.8/src/libro_server/static/9669.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9674.async.js` & `libro-0.1.8/src/libro_server/static/9674.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9749.async.js` & `libro-0.1.8/src/libro_server/static/9749.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/9905.async.js` & `libro-0.1.8/src/libro_server/static/9905.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/index.html` & `libro-0.1.8/src/libro_server/static/index.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/p__execution__index.async.js` & `libro-0.1.8/src/libro_server/static/p__execution__index.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/p__execution__index.chunk.css` & `libro-0.1.8/src/libro_server/static/p__execution__index.chunk.css`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/p__libro__index.async.js` & `libro-0.1.8/src/libro_server/static/p__libro__index.async.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -308,21 +308,17 @@
 
                     function LibroSchemaFormtWidget(props, libroContextKey) {
                         var _this;
                         classCallCheck_default()(this, LibroSchemaFormtWidget);
                         _this = _super.call(this, props, libroContextKey);
                         _this.view = LibroSchemaFormWidgetComponent;
                         _this.schema = void 0;
-                        _this.comm = void 0;
-                        _this.modelId = void 0;
                         initializerDefineProperty_default()(_this, "value", view_descriptor, assertThisInitialized_default()(_this));
                         _this.schema = props.attributes.schema;
                         _this.value = props.attributes.value;
-                        _this.comm = props.options.comm;
-                        _this.modelId = props.options.model_id;
                         return _this;
                     }
                     LibroSchemaFormtWidget = (0, mana_syringe_es /* inject */ .f3)(libro_core_es /* LibroContextKey */ .z4)(LibroSchemaFormtWidget, undefined, 1) || LibroSchemaFormtWidget;
                     LibroSchemaFormtWidget = (0, mana_syringe_es /* inject */ .f3)(view_protocol /* ViewOption */ .Hj)(LibroSchemaFormtWidget, undefined, 0) || LibroSchemaFormtWidget;
                     createClass_default()(LibroSchemaFormtWidget, [{
                         key: "handleCommMsg",
                         value: function handleCommMsg(msg) {
```

### Comparing `libro-0.1.7/src/libro_server/static/umi.js` & `libro-0.1.8/src/libro_server/static/umi.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -29825,14 +29825,23 @@
         __webpack_require__.r(helmet_namespaceObject);
         __webpack_require__.d(helmet_namespaceObject, {
             innerProvider: function() {
                 return innerProvider;
             }
         });
 
+        // NAMESPACE OBJECT: ./src/.umi-production/plugin-routerBase/runtime.ts
+        var plugin_routerBase_runtime_namespaceObject = {};
+        __webpack_require__.r(plugin_routerBase_runtime_namespaceObject);
+        __webpack_require__.d(plugin_routerBase_runtime_namespaceObject, {
+            modifyContextOpts: function() {
+                return modifyContextOpts;
+            }
+        });
+
         // EXTERNAL MODULE: ./node_modules/@umijs/babel-preset-umi/node_modules/@babel/runtime/helpers/regeneratorRuntime.js
         var regeneratorRuntime = __webpack_require__(15009);
         var regeneratorRuntime_default = /*#__PURE__*/ __webpack_require__.n(regeneratorRuntime);
         // EXTERNAL MODULE: ./node_modules/@umijs/babel-preset-umi/node_modules/@babel/runtime/helpers/objectSpread2.js
         var objectSpread2 = __webpack_require__(97857);
         var objectSpread2_default = /*#__PURE__*/ __webpack_require__.n(objectSpread2);
         // EXTERNAL MODULE: ./node_modules/@umijs/babel-preset-umi/node_modules/@babel/runtime/helpers/asyncToGenerator.js
@@ -32928,14 +32937,22 @@
             window.__webpack_public_path__ = cdn;
             window.publicPath = cdn;
             // @ts-ignore
             if (__webpack_require__) {
                 // @ts-ignore
                 __webpack_require__.p = cdn;
             }
+            var el = document.getElementById('jupyter-config-data');
+            if (el) {
+                var pageConfig = JSON.parse(el.textContent || '');
+                var baseUrl = pageConfig['baseUrl'];
+                if (baseUrl && baseUrl.startsWith('/')) {
+                    window.routerBase = baseUrl;
+                }
+            }
         }
         initPublicPath();
         // EXTERNAL MODULE: ./node_modules/prop-types/index.js
         var prop_types = __webpack_require__(45697);
         var prop_types_default = /*#__PURE__*/ __webpack_require__.n(prop_types);
         // EXTERNAL MODULE: ./node_modules/react-fast-compare/index.js
         var react_fast_compare = __webpack_require__(69590);
@@ -33575,14 +33592,23 @@
 
 
 
         var innerProvider = function innerProvider(container) {
             return /*#__PURE__*/ react.createElement(q, {
                 context: context
             }, container);
+        };; // CONCATENATED MODULE: ./src/.umi-production/plugin-routerBase/runtime.ts
+
+        // @ts-nocheck
+        // This file is generated by Umi automatically
+        // DO NOT CHANGE IT MANUALLY!
+        function modifyContextOpts(memo) {
+            return objectSpread2_default()(objectSpread2_default()({}, memo), {}, {
+                basename: window.routerBase
+            });
         };; // CONCATENATED MODULE: ./node_modules/umi/node_modules/@babel/runtime/helpers/esm/typeof.js
         function typeof_typeof(o) {
             "@babel/helpers - typeof";
 
             return typeof_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(o) {
                 return typeof o;
             } : function(o) {
@@ -34506,33 +34532,37 @@
         var useServerInsertedHTML = function useServerInsertedHTML() {};; // CONCATENATED MODULE: ./src/.umi-production/core/plugin.ts
         // @ts-nocheck
         // This file is generated by Umi automatically
         // DO NOT CHANGE IT MANUALLY!
 
 
 
+
         function __defaultExport(obj) {
             if (obj["default"]) {
                 return typeof obj["default"] === 'function' ? obj["default"]() : obj["default"];
             }
             return obj;
         }
 
         function getPlugins() {
             return [{
                 apply: __defaultExport(app_namespaceObject),
                 path: true ? void 0 : 0
             }, {
                 apply: helmet_namespaceObject,
                 path: true ? void 0 : 0
+            }, {
+                apply: plugin_routerBase_runtime_namespaceObject,
+                path: true ? void 0 : 0
             }];
         }
 
         function getValidKeys() {
-            return ['patchRoutes', 'patchClientRoutes', 'modifyContextOpts', 'modifyClientRenderOpts', 'rootContainer', 'innerProvider', 'i18nProvider', 'accessProvider', 'dataflowProvider', 'outerProvider', 'render', 'onRouteChange'];
+            return ['patchRoutes', 'patchClientRoutes', 'modifyContextOpts', 'modifyClientRenderOpts', 'rootContainer', 'innerProvider', 'i18nProvider', 'accessProvider', 'dataflowProvider', 'outerProvider', 'render', 'onRouteChange', 'routerBase'];
         }
         var pluginManager = null;
 
         function createPluginManager() {
             pluginManager = PluginManager.create({
                 plugins: getPlugins(),
                 validKeys: getValidKeys()
```

### Comparing `libro-0.1.7/src/libro_server/static/static/codicon.589e0820.ttf` & `libro-0.1.8/src/libro_server/static/static/codicon.589e0820.ttf`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/devopicons.3c46801a.woff2` & `libro-0.1.8/src/libro_server/static/static/devopicons.3c46801a.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/file-icons.2cbb51ef.woff2` & `libro-0.1.8/src/libro_server/static/static/file-icons.2cbb51ef.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.2b13baa7.eot` & `libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.2b13baa7.eot`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf` & `libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.cf011583.woff` & `libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.cf011583.woff`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.e9955780.woff2` & `libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.e9955780.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome-webfont.f05dad85.svg` & `libro-0.1.8/src/libro_server/static/static/fontawesome-webfont.f05dad85.svg`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/fontawesome.e9955780.woff2` & `libro-0.1.8/src/libro_server/static/static/fontawesome.e9955780.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/mfixx.8e0807ce.woff2` & `libro-0.1.8/src/libro_server/static/static/mfixx.8e0807ce.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/octicons.c982f59d.woff2` & `libro-0.1.8/src/libro_server/static/static/octicons.c982f59d.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/onig.25dd2e6f.wasm` & `libro-0.1.8/src/libro_server/static/static/onig.25dd2e6f.wasm`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/static/static/plotly.eb7b9072.svg` & `libro-0.1.8/src/libro_server/static/static/plotly.eb7b9072.svg`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/templates/libro.html` & `libro-0.1.8/src/libro_server/templates/libro.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/src/libro_server/templates/page.html` & `libro-0.1.8/src/libro_server/templates/page.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.7/pyproject.toml` & `libro-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libro"
-version = "0.1.7"
+version = "0.1.8"
 description = "Libro notebook editor"
 authors = [
     { name = "zhanba", email = "c5e1856@gmail.com" },
     { name = "brokun", email = "brokun0128@gmail.com" }
 ]
 dependencies = [
     "jupyter-server>=2.13.0",
```

