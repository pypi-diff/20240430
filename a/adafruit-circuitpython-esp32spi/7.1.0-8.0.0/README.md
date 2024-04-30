# Comparing `tmp/adafruit-circuitpython-esp32spi-7.1.0.tar.gz` & `tmp/adafruit_circuitpython_esp32spi-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp32spi-7.1.0.tar", last modified: Tue Mar 19 17:44:02 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_esp32spi-8.0.0.tar", last modified: Tue Apr 30 15:56:38 2024, max compression
```

## Comparing `adafruit-circuitpython-esp32spi-7.1.0.tar` & `adafruit_circuitpython_esp32spi-8.0.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.862365 adafruit-circuitpython-esp32spi-7.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.850365 adafruit-circuitpython-esp32spi-7.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.854365 adafruit-circuitpython-esp32spi-7.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.854365 adafruit-circuitpython-esp32spi-7.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.854365 adafruit-circuitpython-esp32spi-7.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-19 17:44:02.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-19 17:44:02.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:44:02.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-19 17:44:02.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-19 17:44:02.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.854365 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38979 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:44:02.858365 adafruit-circuitpython-esp32spi-7.1.0/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/examples/server/esp32spi_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-19 17:43:59.000000 adafruit-circuitpython-esp32spi-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-19 17:43:48.000000 adafruit-circuitpython-esp32spi-7.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:44:02.862365 adafruit-circuitpython-esp32spi-7.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.780486 adafruit_circuitpython_esp32spi-8.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.768486 adafruit_circuitpython_esp32spi-8.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.768486 adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38979 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/server/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:56:38.780486 adafruit_circuitpython_esp32spi-8.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/.gitignore` & `adafruit_circuitpython_esp32spi-8.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_esp32spi-8.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/.pylintrc` & `adafruit_circuitpython_esp32spi-8.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_esp32spi-8.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/LICENSE` & `adafruit_circuitpython_esp32spi-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 7.1.0
+Version: 8.0.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/README.rst` & `adafruit_circuitpython_esp32spi-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 7.1.0
+Version: 8.0.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
 adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
 adafruit_circuitpython_esp32spi.egg-info/requires.txt
 adafruit_circuitpython_esp32spi.egg-info/top_level.txt
 adafruit_esp32spi/PWMOut.py
 adafruit_esp32spi/__init__.py
 adafruit_esp32spi/adafruit_esp32spi.py
-adafruit_esp32spi/adafruit_esp32spi_socket.py
+adafruit_esp32spi/adafruit_esp32spi_socketpool.py
 adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
 adafruit_esp32spi/digitalio.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/PWMOut.py` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "7.1.0"
+__version__ = "8.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi_socket.py` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,131 @@
 # SPDX-FileCopyrightText: Copyright (c) 2019 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 """
-`adafruit_esp32spi_socket`
+`adafruit_esp32spi_socketpool`
 ================================================================================
 
 A socket compatible interface thru the ESP SPI command set
 
 * Author(s): ladyada
 """
+from __future__ import annotations
+
+try:
+    from typing import TYPE_CHECKING, Optional
+
+    if TYPE_CHECKING:
+        from esp32spi.adafruit_esp32spi import ESP_SPIcontrol
+except ImportError:
+    pass
 
-# pylint: disable=no-name-in-module
 
 import time
 import gc
 from micropython import const
-from adafruit_esp32spi import adafruit_esp32spi
+from adafruit_esp32spi import adafruit_esp32spi as esp32spi
 
-_the_interface = None  # pylint: disable=invalid-name
+_global_socketpool = {}
 
 
-def set_interface(iface):
-    """Helper to set the global internet interface"""
-    global _the_interface  # pylint: disable=global-statement, invalid-name
-    _the_interface = iface
+class SocketPoolContants:  # pylint: disable=too-few-public-methods
+    """Helper class for the constants that are needed everywhere"""
 
+    SOCK_STREAM = const(0)
+    SOCK_DGRAM = const(1)
+    AF_INET = const(2)
+    NO_SOCKET_AVAIL = const(255)
 
-SOCK_STREAM = const(0)
-SOCK_DGRAM = const(1)
-AF_INET = const(2)
-NO_SOCKET_AVAIL = const(255)
+    MAX_PACKET = const(4000)
 
-MAX_PACKET = const(4000)
 
+class SocketPool(SocketPoolContants):
+    """ESP32SPI SocketPool library"""
 
-# pylint: disable=too-many-arguments, unused-argument
-def getaddrinfo(host, port, family=0, socktype=0, proto=0, flags=0):
-    """Given a hostname and a port name, return a 'socket.getaddrinfo'
-    compatible list of tuples. Honestly, we ignore anything but host & port"""
-    if not isinstance(port, int):
-        raise ValueError("Port must be an integer")
-    ipaddr = _the_interface.get_host_by_name(host)
-    return [(AF_INET, socktype, proto, "", (ipaddr, port))]
+    def __new__(cls, iface: ESP_SPIcontrol):
+        # We want to make sure to return the same pool for the same interface
+        if iface not in _global_socketpool:
+            _global_socketpool[iface] = super().__new__(cls)
+        return _global_socketpool[iface]
 
+    def __init__(self, iface: ESP_SPIcontrol):
+        self._interface = iface
 
-# pylint: enable=too-many-arguments, unused-argument
+    def getaddrinfo(  # pylint: disable=too-many-arguments,unused-argument
+        self, host, port, family=0, socktype=0, proto=0, flags=0
+    ):
+        """Given a hostname and a port name, return a 'socket.getaddrinfo'
+        compatible list of tuples. Honestly, we ignore anything but host & port"""
+        if not isinstance(port, int):
+            raise ValueError("Port must be an integer")
+        ipaddr = self._interface.get_host_by_name(host)
+        return [(SocketPoolContants.AF_INET, socktype, proto, "", (ipaddr, port))]
+
+    def socket(  # pylint: disable=redefined-builtin
+        self,
+        family=SocketPoolContants.AF_INET,
+        type=SocketPoolContants.SOCK_STREAM,
+        proto=0,
+        fileno=None,
+    ):
+        """Create a new socket and return it"""
+        return Socket(self, family, type, proto, fileno)
 
 
-# pylint: disable=unused-argument, redefined-builtin, invalid-name
-class socket:
+class Socket:
     """A simplified implementation of the Python 'socket' class, for connecting
     through an interface to a remote device"""
 
-    # pylint: disable=too-many-arguments
-    def __init__(
-        self, family=AF_INET, type=SOCK_STREAM, proto=0, fileno=None, socknum=None
+    def __init__(  # pylint: disable=redefined-builtin,too-many-arguments,unused-argument
+        self,
+        socket_pool: SocketPool,
+        family: int = SocketPool.AF_INET,
+        type: int = SocketPool.SOCK_STREAM,
+        proto: int = 0,
+        fileno: Optional[int] = None,
     ):
-        if family != AF_INET:
+        if family != SocketPool.AF_INET:
             raise ValueError("Only AF_INET family supported")
+        self._socket_pool = socket_pool
+        self._interface = self._socket_pool._interface
         self._type = type
         self._buffer = b""
-        self._socknum = socknum if socknum else _the_interface.get_socket()
+        self._socknum = self._interface.get_socket()
         self.settimeout(0)
 
-    # pylint: enable=too-many-arguments
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.close()
-        while (
-            _the_interface.socket_status(self._socknum)
-            != adafruit_esp32spi.SOCKET_CLOSED
-        ):
+        while self._interface.socket_status(self._socknum) != esp32spi.SOCKET_CLOSED:
             pass
 
     def connect(self, address, conntype=None):
         """Connect the socket to the 'address' (which can be 32bit packed IP or
         a hostname string). 'conntype' is an extra that may indicate SSL or not,
         depending on the underlying interface"""
         host, port = address
         if conntype is None:
-            conntype = _the_interface.TCP_MODE
-        if not _the_interface.socket_connect(
+            conntype = self._interface.TCP_MODE
+        if not self._interface.socket_connect(
             self._socknum, host, port, conn_mode=conntype
         ):
             raise ConnectionError("Failed to connect to host", host)
         self._buffer = b""
 
-    def send(self, data):  # pylint: disable=no-self-use
+    def send(self, data):
         """Send some data to the socket."""
-        if self._type is SOCK_DGRAM:
-            conntype = _the_interface.UDP_MODE
+        if self._type is SocketPool.SOCK_DGRAM:
+            conntype = self._interface.UDP_MODE
         else:
-            conntype = _the_interface.TCP_MODE
-        _the_interface.socket_write(self._socknum, data, conn_mode=conntype)
+            conntype = self._interface.TCP_MODE
+        self._interface.socket_write(self._socknum, data, conn_mode=conntype)
         gc.collect()
 
     def recv(self, bufsize: int) -> bytes:
         """Reads some bytes from the connected remote address. Will only return
         an empty string after the configured timeout.
 
         :param int bufsize: maximum number of bytes to receive
@@ -136,15 +161,15 @@
                 self._buffer = self._buffer[bytes_to_read:]
                 # explicitly recheck num_to_read to avoid extra checks
                 continue
 
             num_avail = self._available()
             if num_avail > 0:
                 last_read_time = time.monotonic()
-                bytes_read = _the_interface.socket_read(
+                bytes_read = self._interface.socket_read(
                     self._socknum, min(num_to_read, num_avail)
                 )
                 buffer[num_read : num_read + len(bytes_read)] = bytes_read
                 num_read += len(bytes_read)
                 num_to_read -= len(bytes_read)
             elif num_read > 0:
                 # We got a message, but there are no more bytes to read, so we can stop.
@@ -158,47 +183,46 @@
         """Set the read timeout for sockets.
         If value is 0 socket reads will block until a message is available.
         """
         self._timeout = value
 
     def _available(self):
         """Returns how many bytes of data are available to be read (up to the MAX_PACKET length)"""
-        if self._socknum != NO_SOCKET_AVAIL:
-            return min(_the_interface.socket_available(self._socknum), MAX_PACKET)
+        if self._socknum != SocketPool.NO_SOCKET_AVAIL:
+            return min(
+                self._interface.socket_available(self._socknum), SocketPool.MAX_PACKET
+            )
         return 0
 
     def _connected(self):
         """Whether or not we are connected to the socket"""
-        if self._socknum == NO_SOCKET_AVAIL:
+        if self._socknum == SocketPool.NO_SOCKET_AVAIL:
             return False
         if self._available():
             return True
-        status = _the_interface.socket_status(self._socknum)
+        status = self._interface.socket_status(self._socknum)
         result = status not in (
-            adafruit_esp32spi.SOCKET_LISTEN,
-            adafruit_esp32spi.SOCKET_CLOSED,
-            adafruit_esp32spi.SOCKET_FIN_WAIT_1,
-            adafruit_esp32spi.SOCKET_FIN_WAIT_2,
-            adafruit_esp32spi.SOCKET_TIME_WAIT,
-            adafruit_esp32spi.SOCKET_SYN_SENT,
-            adafruit_esp32spi.SOCKET_SYN_RCVD,
-            adafruit_esp32spi.SOCKET_CLOSE_WAIT,
+            esp32spi.SOCKET_LISTEN,
+            esp32spi.SOCKET_CLOSED,
+            esp32spi.SOCKET_FIN_WAIT_1,
+            esp32spi.SOCKET_FIN_WAIT_2,
+            esp32spi.SOCKET_TIME_WAIT,
+            esp32spi.SOCKET_SYN_SENT,
+            esp32spi.SOCKET_SYN_RCVD,
+            esp32spi.SOCKET_CLOSE_WAIT,
         )
         if not result:
             self.close()
-            self._socknum = NO_SOCKET_AVAIL
+            self._socknum = SocketPool.NO_SOCKET_AVAIL
         return result
 
     def close(self):
         """Close the socket, after reading whatever remains"""
-        _the_interface.socket_close(self._socknum)
+        self._interface.socket_close(self._socknum)
 
 
-class timeout(TimeoutError):
+class timeout(TimeoutError):  # pylint: disable=invalid-name
     """TimeoutError class. An instance of this error will be raised by recv_into() if
     the timeout has elapsed and we haven't received any data yet."""
 
     def __init__(self, msg):
         super().__init__(msg)
-
-
-# pylint: enable=unused-argument, redefined-builtin, invalid-name
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/adafruit_esp32spi/digitalio.py` & `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/docs/api.rst` & `adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. If your library file(s) are nested in a directory (e.g. /adafruit_foo/foo.py)
 .. use this format as the module name: "adafruit_foo.foo"
 
 .. automodule:: adafruit_esp32spi.adafruit_esp32spi
    :members:
 
-.. automodule:: adafruit_esp32spi.adafruit_esp32spi_socket
+.. automodule:: adafruit_esp32spi.adafruit_esp32spi_socketpool
    :members:
 
 .. automodule:: adafruit_esp32spi.adafruit_esp32spi_wifimanager
    :members:
 
 .. automodule:: adafruit_esp32spi.digitalio
    :members:
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/docs/conf.py` & `adafruit_circuitpython_esp32spi-8.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/docs/index.rst` & `adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_aio_post.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_cheerlights.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_ipconfig.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_ipconfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: MIT
 
 import time
 from os import getenv
 import board
 import busio
 from digitalio import DigitalInOut
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_esp32spi.adafruit_esp32spi_socketpool as socketpool
 from adafruit_esp32spi import adafruit_esp32spi
 
 # Get wifi details and more from a settings.toml file
 # tokens used by this Demo: CIRCUITPY_WIFI_SSID, CIRCUITPY_WIFI_PASSWORD
 secrets = {
     "ssid": getenv("CIRCUITPY_WIFI_SSID"),
     "password": getenv("CIRCUITPY_WIFI_PASSWORD"),
@@ -47,17 +47,17 @@
 # Secondary (SCK1) SPI used to connect to WiFi board on Arduino Nano Connect RP2040
 if "SCK1" in dir(board):
     spi = busio.SPI(board.SCK1, board.MOSI1, board.MISO1)
 else:
     spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
 
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
-socket.set_interface(esp)
+pool = socketpool.SocketPool(esp)
 
-s_in = socket.socket(type=socket.SOCK_DGRAM)
+s_in = pool.socket(type=pool.SOCK_DGRAM)
 s_in.settimeout(UDP_TIMEOUT)
 print("set hostname:", HOSTNAME)
 esp.set_hostname(HOSTNAME)
 
 if esp.status == adafruit_esp32spi.WL_IDLE_STATUS:
     print("ESP32 found and in idle mode")
 print("Firmware vers.", esp.firmware_version)
@@ -92,15 +92,15 @@
 )
 
 IP_ADDR = esp.pretty_ip(esp.ip_address)
 print("ip:", IP_ADDR)
 print("My IP address is", esp.pretty_ip(esp.ip_address))
 print("udp in addr: ", UDP_IN_ADDR, UDP_IN_PORT)
 
-socketaddr_udp_in = socket.getaddrinfo(UDP_IN_ADDR, UDP_IN_PORT)[0][4]
+socketaddr_udp_in = pool.getaddrinfo(UDP_IN_ADDR, UDP_IN_PORT)[0][4]
 s_in.connect(socketaddr_udp_in, conntype=esp.UDP_MODE)
 print("connected local UDP")
 
 while True:
     data = s_in.recv(1205)
     if len(data) >= 1:
         data = data.decode("utf-8")
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_localtime.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_settings.toml` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_settings.toml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_simpletest.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_simpletest_rp2040.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_tcp_client.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_tcp_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: MIT
 
 from os import getenv
 import board
 import busio
 from digitalio import DigitalInOut
 from adafruit_esp32spi import adafruit_esp32spi
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_esp32spi.adafruit_esp32spi_socketpool as socketpool
 
 # Get wifi details and more from a settings.toml file
 # tokens used by this Demo: CIRCUITPY_WIFI_SSID, CIRCUITPY_WIFI_PASSWORD
 secrets = {
     "ssid": getenv("CIRCUITPY_WIFI_SSID"),
     "password": getenv("CIRCUITPY_WIFI_PASSWORD"),
 }
@@ -44,17 +44,17 @@
 # connect to wifi AP
 esp.connect(secrets)
 
 # test for connectivity to server
 print("Server ping:", esp.ping(HOST), "ms")
 
 # create the socket
-socket.set_interface(esp)
-socketaddr = socket.getaddrinfo(HOST, PORT)[0][4]
-s = socket.socket()
+pool = socketpool.SocketPool(esp)
+socketaddr = pool.getaddrinfo(HOST, PORT)[0][4]
+s = pool.socket()
 s.settimeout(TIMEOUT)
 
 print("Connecting")
 s.connect(socketaddr)
 
 print("Sending")
 s.send(b"GET /testwifi/index.html HTTP/1.0\r\n\r\n")
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_udp_client.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_udp_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import struct
 import time
 from os import getenv
 import board
 import busio
 from digitalio import DigitalInOut
 from adafruit_esp32spi import adafruit_esp32spi
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_esp32spi.adafruit_esp32spi_socketpool as socketpool
 
 # Get wifi details and more from a settings.toml file
 # tokens used by this Demo: CIRCUITPY_WIFI_SSID, CIRCUITPY_WIFI_PASSWORD
 secrets = {
     "ssid": getenv("CIRCUITPY_WIFI_SSID"),
     "password": getenv("CIRCUITPY_WIFI_PASSWORD"),
 }
@@ -47,17 +47,17 @@
 # connect to wifi AP
 esp.connect(secrets)
 
 # test for connectivity to server
 print("Server ping:", esp.ping(HOST), "ms")
 
 # create the socket
-socket.set_interface(esp)
-socketaddr = socket.getaddrinfo(HOST, PORT)[0][4]
-s = socket.socket(type=socket.SOCK_DGRAM)
+pool = socketpool.SocketPool(esp)
+socketaddr = pool.getaddrinfo(HOST, PORT)[0][4]
+s = pool.socket(type=pool.SOCK_DGRAM)
 
 s.settimeout(TIMEOUT)
 
 print("Sending")
 s.connect(socketaddr, conntype=esp.UDP_MODE)
 packet = bytearray(48)
 packet[0] = 0b00100011  # Not leap second, NTP version 4, Client mode
```

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/gpio/esp32spi_gpio.py` & `adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/examples/gpio/gpio.md` & `adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-7.1.0/pyproject.toml` & `adafruit_circuitpython_esp32spi-8.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "7.1.0"
+version = "8.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```

