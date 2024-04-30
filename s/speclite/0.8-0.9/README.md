# Comparing `tmp/speclite-0.8.tar.gz` & `tmp/speclite-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/speclite-0.8.tar", last modified: Tue Sep 11 20:10:10 2018, max compression
+gzip compressed data, was "dist/speclite-0.9.tar", last modified: Fri Oct 30 21:31:00 2020, max compression
```

## Comparing `speclite-0.8.tar` & `speclite-0.9.tar`

### file list

```diff
@@ -1,188 +1,137 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/
--rw-r--r--   0 david      (501) staff       (20)    36850 2018-08-21 16:46:28.000000 speclite-0.8/ah_bootstrap.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/
--rw-r--r--   0 david      (501) staff       (20)    35044 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/
--rw-r--r--   0 david      (501) staff       (20)     1836 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 david      (501) staff       (20)        0 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2940 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 david      (501) staff       (20)    11722 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/_test_compat.py
--rw-r--r--   0 david      (501) staff       (20)    19700 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 david      (501) staff       (20)     1454 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/build_py.py
--rw-r--r--   0 david      (501) staff       (20)    10431 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-r--r--   0 david      (501) staff       (20)      486 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/install.py
--rw-r--r--   0 david      (501) staff       (20)      512 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/install_lib.py
--rw-r--r--   0 david      (501) staff       (20)     2407 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/register.py
--rw-r--r--   0 david      (501) staff       (20)      120 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 david      (501) staff       (20)     3033 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 david      (501) staff       (20)     1364 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/commands/test.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/compat/
--rw-r--r--   0 david      (501) staff       (20)      368 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/compat/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     7922 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/distutils_helpers.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/
--rw-r--r--   0 david      (501) staff       (20)      589 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/
--rw-r--r--   0 david      (501) staff       (20)       20 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     5316 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
--rw-r--r--   0 david      (501) staff       (20)    15785 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
--rw-r--r--   0 david      (501) staff       (20)    26026 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
--rw-r--r--   0 david      (501) staff       (20)     3711 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
--rw-r--r--   0 david      (501) staff       (20)     7140 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/
--rw-r--r--   0 david      (501) staff       (20)       94 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    18074 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
--rw-r--r--   0 david      (501) staff       (20)     9527 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
--rw-r--r--   0 david      (501) staff       (20)     2507 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/linkcode.py
--rw-r--r--   0 david      (501) staff       (20)     6648 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
--rw-r--r--   0 david      (501) staff       (20)      161 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/extern/setup_package.py
--rw-r--r--   0 david      (501) staff       (20)     6104 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 david      (501) staff       (20)    26678 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 david      (501) staff       (20)      437 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    12228 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/conf.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/
--rw-r--r--   0 david      (501) staff       (20)       66 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2832 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
--rw-r--r--   0 david      (501) staff       (20)     1312 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
--rw-r--r--   0 david      (501) staff       (20)     5857 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/
--rw-r--r--   0 david      (501) staff       (20)        0 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
--rw-r--r--   0 david      (501) staff       (20)      677 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/local/
--rw-r--r--   0 david      (501) staff       (20)      562 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
--rw-r--r--   0 david      (501) staff       (20)     1638 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
--rw-r--r--   0 david      (501) staff       (20)      658 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
--rw-r--r--   0 david      (501) staff       (20)     2820 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
--rw-r--r--   0 david      (501) staff       (20)      292 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/setup_package.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
--rw-r--r--   0 david      (501) staff       (20)       73 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
--rw-r--r--   0 david      (501) staff       (20)     3433 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
--rw-r--r--   0 david      (501) staff       (20)       34 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
--rw-r--r--   0 david      (501) staff       (20)      272 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
--rw-r--r--   0 david      (501) staff       (20)     5201 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
--rw-r--r--   0 david      (501) staff       (20)     1725 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
--rw-r--r--   0 david      (501) staff       (20)    32988 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
--rw-r--r--   0 david      (501) staff       (20)     4634 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
--rw-r--r--   0 david      (501) staff       (20)     1884 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
--rw-r--r--   0 david      (501) staff       (20)    12067 2017-03-20 19:24:51.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
--rw-r--r--   0 david      (501) staff       (20)     2769 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
--rw-r--r--   0 david      (501) staff       (20)     4971 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
--rw-r--r--   0 david      (501) staff       (20)      192 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
--rw-r--r--   0 david      (501) staff       (20)      515 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/test_helpers.py
--rw-r--r--   0 david      (501) staff       (20)    27125 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 david      (501) staff       (20)      547 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 david      (501) staff       (20)     9659 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 david      (501) staff       (20)        1 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 david      (501) staff       (20)     2970 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     3366 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)       16 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/astropy_helpers.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)    15081 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/CHANGES.rst
--rw-r--r--   0 david      (501) staff       (20)    12537 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/ez_setup.py
--rw-r--r--   0 david      (501) staff       (20)     1491 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/LICENSE.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/astropy_helpers/licenses/
--rw-r--r--   0 david      (501) staff       (20)     2505 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
--rw-r--r--   0 david      (501) staff       (20)     5959 2015-07-22 14:51:57.000000 speclite-0.8/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
--rw-r--r--   0 david      (501) staff       (20)     2577 2017-10-02 23:07:57.000000 speclite-0.8/astropy_helpers/README.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/cextern/
--rw-r--r--   0 david      (501) staff       (20)      298 2015-07-17 09:24:47.000000 speclite-0.8/cextern/README.rst
--rw-r--r--   0 david      (501) staff       (20)     1375 2018-09-11 20:09:47.000000 speclite-0.8/CHANGES.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/docs/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/docs/_static/
--rw-r--r--   0 david      (501) staff       (20)    36278 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/bessell.png
--rw-r--r--   0 david      (501) staff       (20)    21888 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/custom.png
--rw-r--r--   0 david      (501) staff       (20)    37822 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/decam2014.png
--rw-r--r--   0 david      (501) staff       (20)    24731 2018-08-22 06:34:12.000000 speclite-0.8/docs/_static/desi_imaging.png
--rw-r--r--   0 david      (501) staff       (20)    27112 2017-10-03 01:22:04.000000 speclite-0.8/docs/_static/hsc2017.png
--rw-r--r--   0 david      (501) staff       (20)    31832 2016-08-22 18:42:44.000000 speclite-0.8/docs/_static/lsst2016.png
--rw-r--r--   0 david      (501) staff       (20)    46616 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/sampling.png
--rw-r--r--   0 david      (501) staff       (20)    30420 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/sdss2010.png
--rw-r--r--   0 david      (501) staff       (20)    30536 2016-02-05 18:36:11.000000 speclite-0.8/docs/_static/wise2010.png
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/docs/_templates/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/docs/_templates/autosummary/
--rw-r--r--   0 david      (501) staff       (20)      250 2015-07-17 09:24:47.000000 speclite-0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 david      (501) staff       (20)      251 2015-07-17 09:24:47.000000 speclite-0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 david      (501) staff       (20)      252 2015-07-17 09:24:47.000000 speclite-0.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 david      (501) staff       (20)      409 2016-02-05 18:36:11.000000 speclite-0.8/docs/api.rst
--rw-r--r--   0 david      (501) staff       (20)     6847 2017-03-21 14:33:35.000000 speclite-0.8/docs/conf.py
--rw-r--r--   0 david      (501) staff       (20)     9367 2018-08-22 06:34:12.000000 speclite-0.8/docs/filters.rst
--rw-r--r--   0 david      (501) staff       (20)      214 2016-02-05 18:36:11.000000 speclite-0.8/docs/index.rst
--rw-r--r--   0 david      (501) staff       (20)      272 2015-08-05 17:54:15.000000 speclite-0.8/docs/install.rst
--rw-r--r--   0 david      (501) staff       (20)     4513 2015-07-17 09:24:47.000000 speclite-0.8/docs/make.bat
--rw-r--r--   0 david      (501) staff       (20)     4581 2016-08-22 18:42:44.000000 speclite-0.8/docs/Makefile
--rw-r--r--   0 david      (501) staff       (20)     3749 2018-08-22 06:34:12.000000 speclite-0.8/docs/overview.rst
--rw-r--r--   0 david      (501) staff       (20)       43 2015-08-03 14:34:48.000000 speclite-0.8/docs/rtd-pip-requirements
--rw-r--r--   0 david      (501) staff       (20)    12537 2017-10-03 21:38:45.000000 speclite-0.8/ez_setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/licenses/
--rw-r--r--   0 david      (501) staff       (20)     1510 2015-11-03 13:28:11.000000 speclite-0.8/licenses/LICENSE.rst
--rw-r--r--   0 david      (501) staff       (20)      162 2015-07-17 09:24:47.000000 speclite-0.8/licenses/README.rst
--rw-r--r--   0 david      (501) staff       (20)      415 2018-09-11 20:10:10.000000 speclite-0.8/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1422 2016-08-22 18:42:44.000000 speclite-0.8/README.rst
--rw-r--r--   0 david      (501) staff       (20)     1456 2018-09-11 20:09:47.000000 speclite-0.8/setup.cfg
--rwxr-xr-x   0 david      (501) staff       (20)     4773 2017-03-21 14:33:35.000000 speclite-0.8/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/
--rw-r--r--   0 david      (501) staff       (20)      661 2017-03-20 16:42:18.000000 speclite-0.8/speclite/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     5273 2016-09-28 00:51:31.000000 speclite-0.8/speclite/_astropy_init.py
--rw-r--r--   0 david      (501) staff       (20)    10091 2017-03-21 14:33:35.000000 speclite-0.8/speclite/accumulate.py
--rw-r--r--   0 david      (501) staff       (20)     4088 2017-10-03 01:22:04.000000 speclite-0.8/speclite/benchmark.py
--rw-r--r--   0 david      (501) staff       (20)     1435 2016-08-22 18:42:44.000000 speclite-0.8/speclite/conftest.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/data/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/data/filters/
--rw-r--r--   0 david      (501) staff       (20)     5914 2018-08-22 06:34:12.000000 speclite-0.8/speclite/data/filters/BASS-g.ecsv
--rw-r--r--   0 david      (501) staff       (20)     5493 2018-08-22 06:34:12.000000 speclite-0.8/speclite/data/filters/BASS-r.ecsv
--rw-r--r--   0 david      (501) staff       (20)      868 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/bessell-B.ecsv
--rw-r--r--   0 david      (501) staff       (20)      885 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/bessell-I.ecsv
--rw-r--r--   0 david      (501) staff       (20)      889 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/bessell-R.ecsv
--rw-r--r--   0 david      (501) staff       (20)      924 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/bessell-U.ecsv
--rw-r--r--   0 david      (501) staff       (20)      906 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/bessell-V.ecsv
--rw-r--r--   0 david      (501) staff       (20)     7675 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-g.ecsv
--rw-r--r--   0 david      (501) staff       (20)     9163 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-i.ecsv
--rw-r--r--   0 david      (501) staff       (20)     8980 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-r.ecsv
--rw-r--r--   0 david      (501) staff       (20)     4611 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-u.ecsv
--rw-r--r--   0 david      (501) staff       (20)     9482 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-Y.ecsv
--rw-r--r--   0 david      (501) staff       (20)     9602 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/decam2014-z.ecsv
--rw-r--r--   0 david      (501) staff       (20)     3645 2017-10-03 01:22:04.000000 speclite-0.8/speclite/data/filters/hsc2017-g.ecsv
--rw-r--r--   0 david      (501) staff       (20)     3783 2017-10-03 01:22:04.000000 speclite-0.8/speclite/data/filters/hsc2017-i.ecsv
--rw-r--r--   0 david      (501) staff       (20)     3669 2017-10-03 01:22:04.000000 speclite-0.8/speclite/data/filters/hsc2017-r.ecsv
--rw-r--r--   0 david      (501) staff       (20)     3018 2017-10-03 01:22:04.000000 speclite-0.8/speclite/data/filters/hsc2017-y.ecsv
--rw-r--r--   0 david      (501) staff       (20)     2192 2017-10-03 01:22:04.000000 speclite-0.8/speclite/data/filters/hsc2017-z.ecsv
--rw-r--r--   0 david      (501) staff       (20)    38598 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-g.ecsv
--rw-r--r--   0 david      (501) staff       (20)    33561 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-i.ecsv
--rw-r--r--   0 david      (501) staff       (20)    36070 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-r.ecsv
--rw-r--r--   0 david      (501) staff       (20)    23071 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-u.ecsv
--rw-r--r--   0 david      (501) staff       (20)    42778 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-y.ecsv
--rw-r--r--   0 david      (501) staff       (20)    29108 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/filters/lsst2016-z.ecsv
--rw-r--r--   0 david      (501) staff       (20)     7414 2018-08-22 06:34:12.000000 speclite-0.8/speclite/data/filters/MzLS-z.ecsv
--rw-r--r--   0 david      (501) staff       (20)     2181 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/sdss2010-g.ecsv
--rw-r--r--   0 david      (501) staff       (20)     2029 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/sdss2010-i.ecsv
--rw-r--r--   0 david      (501) staff       (20)     1943 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/sdss2010-r.ecsv
--rw-r--r--   0 david      (501) staff       (20)     1909 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/sdss2010-u.ecsv
--rw-r--r--   0 david      (501) staff       (20)     3096 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/sdss2010-z.ecsv
--rw-r--r--   0 david      (501) staff       (20)     2322 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/wise2010-W1.ecsv
--rw-r--r--   0 david      (501) staff       (20)     2601 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/wise2010-W2.ecsv
--rw-r--r--   0 david      (501) staff       (20)    16585 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/wise2010-W3.ecsv
--rw-r--r--   0 david      (501) staff       (20)    11673 2016-02-05 18:36:11.000000 speclite-0.8/speclite/data/filters/wise2010-W4.ecsv
--rw-r--r--   0 david      (501) staff       (20)      331 2016-08-22 18:42:44.000000 speclite-0.8/speclite/data/README.rst
--rw-r--r--   0 david      (501) staff       (20)     8282 2017-03-21 14:33:35.000000 speclite-0.8/speclite/downsample.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/extern/
--rw-r--r--   0 david      (501) staff       (20)      445 2016-02-05 18:36:11.000000 speclite-0.8/speclite/extern/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    85400 2018-08-23 07:41:42.000000 speclite-0.8/speclite/filters.py
--rw-r--r--   0 david      (501) staff       (20)     8936 2018-08-22 06:34:12.000000 speclite-0.8/speclite/redshift.py
--rw-r--r--   0 david      (501) staff       (20)     8768 2017-03-21 14:33:35.000000 speclite-0.8/speclite/resample.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/tests/
--rw-r--r--   0 david      (501) staff       (20)      121 2015-07-17 09:24:47.000000 speclite-0.8/speclite/tests/__init__.py
--rw-r--r--   0 david      (501) staff       (20)      768 2015-07-17 09:24:47.000000 speclite-0.8/speclite/tests/coveragerc
--rw-r--r--   0 david      (501) staff       (20)       96 2015-07-17 09:24:47.000000 speclite-0.8/speclite/tests/setup_package.py
--rw-r--r--   0 david      (501) staff       (20)    10471 2016-02-05 18:36:11.000000 speclite-0.8/speclite/tests/test_accumulate.py
--rw-r--r--   0 david      (501) staff       (20)     5339 2016-08-22 18:42:44.000000 speclite-0.8/speclite/tests/test_downsample.py
--rw-r--r--   0 david      (501) staff       (20)    19495 2018-08-22 06:34:12.000000 speclite-0.8/speclite/tests/test_filters.py
--rw-r--r--   0 david      (501) staff       (20)     8338 2016-09-28 00:05:54.000000 speclite-0.8/speclite/tests/test_redshift.py
--rw-r--r--   0 david      (501) staff       (20)     8596 2016-09-28 00:05:54.000000 speclite-0.8/speclite/tests/test_resample.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2018-09-11 20:10:10.000000 speclite-0.8/speclite/utils/
--rw-r--r--   0 david      (501) staff       (20)      199 2015-07-17 09:24:47.000000 speclite-0.8/speclite/utils/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     6957 2018-09-11 20:10:07.000000 speclite-0.8/speclite/version.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/
+-rw-r--r--   0 david      (501) staff       (20)     1429 2018-09-11 20:10:26.000000 speclite-0.9/CHANGES.rst
+-rw-r--r--   0 david      (501) staff       (20)      415 2020-10-30 21:31:00.000000 speclite-0.9/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1422 2016-08-22 18:42:44.000000 speclite-0.9/README.rst
+-rw-r--r--   0 david      (501) staff       (20)    37507 2020-07-17 21:48:28.000000 speclite-0.9/ah_bootstrap.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/
+-rw-r--r--   0 david      (501) staff       (20)    22464 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/CHANGES.rst
+-rw-r--r--   0 david      (501) staff       (20)     1491 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/LICENSE.rst
+-rw-r--r--   0 david      (501) staff       (20)     1525 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/README.rst
+-rw-r--r--   0 david      (501) staff       (20)    37507 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/ah_bootstrap.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/astropy_helpers/
+-rw-r--r--   0 david      (501) staff       (20)     1738 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/
+-rw-r--r--   0 david      (501) staff       (20)        0 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2762 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/_dummy.py
+-rw-r--r--   0 david      (501) staff       (20)     8674 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/build_ext.py
+-rw-r--r--   0 david      (501) staff       (20)     8176 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/build_sphinx.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/src/
+-rw-r--r--   0 david      (501) staff       (20)     2720 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/src/compiler.c
+-rw-r--r--   0 david      (501) staff       (20)     1466 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/commands/test.py
+-rw-r--r--   0 david      (501) staff       (20)     1930 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/conftest.py
+-rw-r--r--   0 david      (501) staff       (20)     8121 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/distutils_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)     6495 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/git_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)     9329 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/openmp_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)    29034 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/setup_helpers.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/astropy_helpers/sphinx/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/sphinx/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      156 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/sphinx/conf.py
+-rw-r--r--   0 david      (501) staff       (20)     8567 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/utils.py
+-rw-r--r--   0 david      (501) staff       (20)      547 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers/version.py
+-rw-r--r--   0 david      (501) staff       (20)    12694 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/astropy_helpers/version_helpers.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     2970 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     3366 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 david      (501) staff       (20)       16 2015-07-22 14:51:57.000000 speclite-0.9/astropy_helpers/astropy_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/astropy_helpers/licenses/
+-rw-r--r--   0 david      (501) staff       (20)     1644 2020-04-17 18:23:46.000000 speclite-0.9/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/cextern/
+-rw-r--r--   0 david      (501) staff       (20)      298 2015-07-17 09:24:47.000000 speclite-0.9/cextern/README.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/docs/
+-rw-r--r--   0 david      (501) staff       (20)     4581 2016-08-22 18:42:44.000000 speclite-0.9/docs/Makefile
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/docs/_static/
+-rw-r--r--   0 david      (501) staff       (20)    36278 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/bessell.png
+-rw-r--r--   0 david      (501) staff       (20)    21888 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/custom.png
+-rw-r--r--   0 david      (501) staff       (20)    37822 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/decam2014.png
+-rw-r--r--   0 david      (501) staff       (20)    24731 2018-08-22 06:34:12.000000 speclite-0.9/docs/_static/desi_imaging.png
+-rw-r--r--   0 david      (501) staff       (20)    43237 2020-04-17 15:51:12.000000 speclite-0.9/docs/_static/euclid.png
+-rw-r--r--   0 david      (501) staff       (20)    27112 2017-10-03 01:22:04.000000 speclite-0.9/docs/_static/hsc2017.png
+-rw-r--r--   0 david      (501) staff       (20)    31832 2016-08-22 18:42:44.000000 speclite-0.9/docs/_static/lsst2016.png
+-rw-r--r--   0 david      (501) staff       (20)    46616 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/sampling.png
+-rw-r--r--   0 david      (501) staff       (20)    30420 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/sdss2010.png
+-rw-r--r--   0 david      (501) staff       (20)    30536 2016-02-05 18:36:11.000000 speclite-0.9/docs/_static/wise2010.png
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/docs/_templates/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/docs/_templates/autosummary/
+-rw-r--r--   0 david      (501) staff       (20)      250 2015-07-17 09:24:47.000000 speclite-0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 david      (501) staff       (20)      251 2015-07-17 09:24:47.000000 speclite-0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 david      (501) staff       (20)      252 2015-07-17 09:24:47.000000 speclite-0.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 david      (501) staff       (20)      409 2016-02-05 18:36:11.000000 speclite-0.9/docs/api.rst
+-rw-r--r--   0 david      (501) staff       (20)     6799 2020-07-17 21:48:28.000000 speclite-0.9/docs/conf.py
+-rw-r--r--   0 david      (501) staff       (20)     9994 2020-04-17 15:51:12.000000 speclite-0.9/docs/filters.rst
+-rw-r--r--   0 david      (501) staff       (20)      214 2016-02-05 18:36:11.000000 speclite-0.9/docs/index.rst
+-rw-r--r--   0 david      (501) staff       (20)      272 2015-08-05 17:54:15.000000 speclite-0.9/docs/install.rst
+-rw-r--r--   0 david      (501) staff       (20)     4513 2015-07-17 09:24:47.000000 speclite-0.9/docs/make.bat
+-rw-r--r--   0 david      (501) staff       (20)     3749 2018-08-22 06:34:12.000000 speclite-0.9/docs/overview.rst
+-rw-r--r--   0 david      (501) staff       (20)       43 2015-08-03 14:34:48.000000 speclite-0.9/docs/rtd-pip-requirements
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/licenses/
+-rw-r--r--   0 david      (501) staff       (20)     1510 2015-11-03 13:28:11.000000 speclite-0.9/licenses/LICENSE.rst
+-rw-r--r--   0 david      (501) staff       (20)      162 2015-07-17 09:24:47.000000 speclite-0.9/licenses/README.rst
+-rw-r--r--   0 david      (501) staff       (20)     1472 2020-10-30 21:30:10.000000 speclite-0.9/setup.cfg
+-rwxr-xr-x   0 david      (501) staff       (20)     4693 2020-10-30 21:29:54.000000 speclite-0.9/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/
+-rw-r--r--   0 david      (501) staff       (20)      661 2017-03-20 16:42:18.000000 speclite-0.9/speclite/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     5273 2016-09-28 00:51:31.000000 speclite-0.9/speclite/_astropy_init.py
+-rw-r--r--   0 david      (501) staff       (20)    10091 2017-03-21 14:33:35.000000 speclite-0.9/speclite/accumulate.py
+-rw-r--r--   0 david      (501) staff       (20)     4088 2017-10-03 01:22:04.000000 speclite-0.9/speclite/benchmark.py
+-rw-r--r--   0 david      (501) staff       (20)     2099 2020-07-17 21:48:28.000000 speclite-0.9/speclite/conftest.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/data/
+-rw-r--r--   0 david      (501) staff       (20)      331 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/README.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/data/filters/
+-rw-r--r--   0 david      (501) staff       (20)     5914 2018-08-22 06:34:12.000000 speclite-0.9/speclite/data/filters/BASS-g.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     5493 2018-08-22 06:34:12.000000 speclite-0.9/speclite/data/filters/BASS-r.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    59247 2020-04-17 15:51:12.000000 speclite-0.9/speclite/data/filters/Euclid-H.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    63755 2020-04-17 15:51:12.000000 speclite-0.9/speclite/data/filters/Euclid-J.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    27622 2020-04-17 15:51:12.000000 speclite-0.9/speclite/data/filters/Euclid-VIS.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    64865 2020-04-17 15:51:12.000000 speclite-0.9/speclite/data/filters/Euclid-Y.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     7414 2018-08-22 06:34:12.000000 speclite-0.9/speclite/data/filters/MzLS-z.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      868 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/bessell-B.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      885 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/bessell-I.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      889 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/bessell-R.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      924 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/bessell-U.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      906 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/bessell-V.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     9482 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-Y.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     7675 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-g.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     9163 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-i.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     8980 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-r.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     4611 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-u.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     9602 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/decam2014-z.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     3645 2017-10-03 01:22:04.000000 speclite-0.9/speclite/data/filters/hsc2017-g.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     3783 2017-10-03 01:22:04.000000 speclite-0.9/speclite/data/filters/hsc2017-i.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     3669 2017-10-03 01:22:04.000000 speclite-0.9/speclite/data/filters/hsc2017-r.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     3018 2017-10-03 01:22:04.000000 speclite-0.9/speclite/data/filters/hsc2017-y.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     2192 2017-10-03 01:22:04.000000 speclite-0.9/speclite/data/filters/hsc2017-z.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    38598 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-g.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    33561 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-i.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    36070 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-r.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    23071 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-u.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    42778 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-y.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    29108 2016-08-22 18:42:44.000000 speclite-0.9/speclite/data/filters/lsst2016-z.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     2181 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/sdss2010-g.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     2029 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/sdss2010-i.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     1943 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/sdss2010-r.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     1909 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/sdss2010-u.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     3096 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/sdss2010-z.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     2322 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/wise2010-W1.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     2601 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/wise2010-W2.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    16585 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/wise2010-W3.ecsv
+-rw-r--r--   0 david      (501) staff       (20)    11673 2016-02-05 18:36:11.000000 speclite-0.9/speclite/data/filters/wise2010-W4.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     8282 2017-03-21 14:33:35.000000 speclite-0.9/speclite/downsample.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/extern/
+-rw-r--r--   0 david      (501) staff       (20)      445 2016-02-05 18:36:11.000000 speclite-0.9/speclite/extern/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    85446 2020-04-17 15:51:12.000000 speclite-0.9/speclite/filters.py
+-rw-r--r--   0 david      (501) staff       (20)     8936 2018-08-22 06:34:12.000000 speclite-0.9/speclite/redshift.py
+-rw-r--r--   0 david      (501) staff       (20)     9297 2020-04-17 15:51:12.000000 speclite-0.9/speclite/resample.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/tests/
+-rw-r--r--   0 david      (501) staff       (20)      121 2015-07-17 09:24:47.000000 speclite-0.9/speclite/tests/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      768 2015-07-17 09:24:47.000000 speclite-0.9/speclite/tests/coveragerc
+-rw-r--r--   0 david      (501) staff       (20)       96 2015-07-17 09:24:47.000000 speclite-0.9/speclite/tests/setup_package.py
+-rw-r--r--   0 david      (501) staff       (20)    10471 2016-02-05 18:36:11.000000 speclite-0.9/speclite/tests/test_accumulate.py
+-rw-r--r--   0 david      (501) staff       (20)     5339 2016-08-22 18:42:44.000000 speclite-0.9/speclite/tests/test_downsample.py
+-rw-r--r--   0 david      (501) staff       (20)    19827 2020-04-17 15:51:12.000000 speclite-0.9/speclite/tests/test_filters.py
+-rw-r--r--   0 david      (501) staff       (20)     8338 2016-09-28 00:05:54.000000 speclite-0.9/speclite/tests/test_redshift.py
+-rw-r--r--   0 david      (501) staff       (20)     8596 2016-09-28 00:05:54.000000 speclite-0.9/speclite/tests/test_resample.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2020-10-30 21:31:00.000000 speclite-0.9/speclite/utils/
+-rw-r--r--   0 david      (501) staff       (20)      199 2015-07-17 09:24:47.000000 speclite-0.9/speclite/utils/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      372 2020-10-30 21:30:58.000000 speclite-0.9/speclite/version.py
```

### Comparing `speclite-0.8/ah_bootstrap.py` & `speclite-0.9/ah_bootstrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,71 +34,140 @@
 
 See https://github.com/astropy/astropy-helpers for more details, and for the
 latest version of this module.
 """
 
 import contextlib
 import errno
-import imp
 import io
 import locale
 import os
 import re
 import subprocess as sp
 import sys
 
-try:
-    from ConfigParser import ConfigParser, RawConfigParser
-except ImportError:
-    from configparser import ConfigParser, RawConfigParser
+from distutils import log
+from distutils.debug import DEBUG
 
+from configparser import ConfigParser, RawConfigParser
 
-if sys.version_info[0] < 3:
-    _str_types = (str, unicode)
-    _text_type = unicode
-    PY3 = False
+import pkg_resources
+
+from setuptools import Distribution
+from setuptools.package_index import PackageIndex
+
+# This is the minimum Python version required for astropy-helpers
+__minimum_python_version__ = (3, 5)
+
+# TODO: Maybe enable checking for a specific version of astropy_helpers?
+DIST_NAME = 'astropy-helpers'
+PACKAGE_NAME = 'astropy_helpers'
+UPPER_VERSION_EXCLUSIVE = None
+
+# Defaults for other options
+DOWNLOAD_IF_NEEDED = True
+INDEX_URL = 'https://pypi.python.org/simple'
+USE_GIT = True
+OFFLINE = False
+AUTO_UPGRADE = True
+
+# A list of all the configuration options and their required types
+CFG_OPTIONS = [
+    ('auto_use', bool), ('path', str), ('download_if_needed', bool),
+    ('index_url', str), ('use_git', bool), ('offline', bool),
+    ('auto_upgrade', bool)
+]
+
+# Start off by parsing the setup.cfg file
+
+_err_help_msg = """
+If the problem persists consider installing astropy_helpers manually using pip
+(`pip install astropy_helpers`) or by manually downloading the source archive,
+extracting it, and installing by running `python setup.py install` from the
+root of the extracted source code.
+"""
+
+SETUP_CFG = ConfigParser()
+
+if os.path.exists('setup.cfg'):
+
+    try:
+        SETUP_CFG.read('setup.cfg')
+    except Exception as e:
+        if DEBUG:
+            raise
+
+        log.error(
+            "Error reading setup.cfg: {0!r}\n{1} will not be "
+            "automatically bootstrapped and package installation may fail."
+            "\n{2}".format(e, PACKAGE_NAME, _err_help_msg))
+
+# We used package_name in the package template for a while instead of name
+if SETUP_CFG.has_option('metadata', 'name'):
+    parent_package = SETUP_CFG.get('metadata', 'name')
+elif SETUP_CFG.has_option('metadata', 'package_name'):
+    parent_package = SETUP_CFG.get('metadata', 'package_name')
 else:
-    _str_types = (str, bytes)
-    _text_type = str
-    PY3 = True
+    parent_package = None
+
+if SETUP_CFG.has_option('options', 'python_requires'):
+
+    python_requires = SETUP_CFG.get('options', 'python_requires')
+
+    # The python_requires key has a syntax that can be parsed by SpecifierSet
+    # in the packaging package. However, we don't want to have to depend on that
+    # package, so instead we can use setuptools (which bundles packaging). We
+    # have to add 'python' to parse it with Requirement.
+
+    from pkg_resources import Requirement
+    req = Requirement.parse('python' + python_requires)
+
+    # We want the Python version as a string, which we can get from the platform module
+    import platform
+    # strip off trailing '+' incase this is a dev install of python
+    python_version = platform.python_version().strip('+')
+    # allow pre-releases to count as 'new enough'
+    if not req.specifier.contains(python_version, True):
+        if parent_package is None:
+            message = "ERROR: Python {} is required by this package\n".format(req.specifier)
+        else:
+            message = "ERROR: Python {} is required by {}\n".format(req.specifier, parent_package)
+        sys.stderr.write(message)
+        sys.exit(1)
+
+if sys.version_info < __minimum_python_version__:
+
+    if parent_package is None:
+        message = "ERROR: Python {} or later is required by astropy-helpers\n".format(
+            __minimum_python_version__)
+    else:
+        message = "ERROR: Python {} or later is required by astropy-helpers for {}\n".format(
+            __minimum_python_version__, parent_package)
+
+    sys.stderr.write(message)
+    sys.exit(1)
+
+_str_types = (str, bytes)
 
 
 # What follows are several import statements meant to deal with install-time
 # issues with either missing or misbehaving pacakges (including making sure
 # setuptools itself is installed):
 
+# Check that setuptools 30.3 or later is present
+from distutils.version import LooseVersion
 
-# Some pre-setuptools checks to ensure that either distribute or setuptools >=
-# 0.7 is used (over pre-distribute setuptools) if it is available on the path;
-# otherwise the latest setuptools will be downloaded and bootstrapped with
-# ``ez_setup.py``.  This used to be included in a separate file called
-# setuptools_bootstrap.py; but it was combined into ah_bootstrap.py
 try:
-    import pkg_resources
-    _setuptools_req = pkg_resources.Requirement.parse('setuptools>=0.7')
-    # This may raise a DistributionNotFound in which case no version of
-    # setuptools or distribute is properly installed
-    _setuptools = pkg_resources.get_distribution('setuptools')
-    if _setuptools not in _setuptools_req:
-        # Older version of setuptools; check if we have distribute; again if
-        # this results in DistributionNotFound we want to give up
-        _distribute = pkg_resources.get_distribution('distribute')
-        if _setuptools != _distribute:
-            # It's possible on some pathological systems to have an old version
-            # of setuptools and distribute on sys.path simultaneously; make
-            # sure distribute is the one that's used
-            sys.path.insert(1, _distribute.location)
-            _distribute.activate()
-            imp.reload(pkg_resources)
-except:
-    # There are several types of exceptions that can occur here; if all else
-    # fails bootstrap and use the bootstrapped version
-    from ez_setup import use_setuptools
-    use_setuptools()
+    import setuptools
+    assert LooseVersion(setuptools.__version__) >= LooseVersion('30.3')
+except (ImportError, AssertionError):
+    sys.stderr.write("ERROR: setuptools 30.3 or later is required by astropy-helpers\n")
+    sys.exit(1)
 
+SETUPTOOLS_LT_42 = LooseVersion(setuptools.__version__) < LooseVersion('42')
 
 # typing as a dependency for 1.6.1+ Sphinx causes issues when imported after
 # initializing submodule with ah_boostrap.py
 # See discussion and references in
 # https://github.com/astropy/astropy-helpers/issues/302
 
 try:
@@ -133,48 +202,14 @@
     # Ignore if this fails for *any* reason*
     pass
 
 
 # End compatibility imports...
 
 
-# In case it didn't successfully import before the ez_setup checks
-import pkg_resources
-
-from setuptools import Distribution
-from setuptools.package_index import PackageIndex
-
-from distutils import log
-from distutils.debug import DEBUG
-
-
-# TODO: Maybe enable checking for a specific version of astropy_helpers?
-DIST_NAME = 'astropy-helpers'
-PACKAGE_NAME = 'astropy_helpers'
-
-if PY3:
-    UPPER_VERSION_EXCLUSIVE = None
-else:
-    UPPER_VERSION_EXCLUSIVE = '3'
-
-# Defaults for other options
-DOWNLOAD_IF_NEEDED = True
-INDEX_URL = 'https://pypi.python.org/simple'
-USE_GIT = True
-OFFLINE = False
-AUTO_UPGRADE = True
-
-# A list of all the configuration options and their required types
-CFG_OPTIONS = [
-    ('auto_use', bool), ('path', str), ('download_if_needed', bool),
-    ('index_url', str), ('use_git', bool), ('offline', bool),
-    ('auto_upgrade', bool)
-]
-
-
 class _Bootstrapper(object):
     """
     Bootstrapper implementation.  See ``use_astropy_helpers`` for parameter
     documentation.
     """
 
     def __init__(self, path=None, index_url=None, use_git=None, offline=None,
@@ -182,15 +217,15 @@
 
         if path is None:
             path = PACKAGE_NAME
 
         if not (isinstance(path, _str_types) or path is False):
             raise TypeError('path must be a string or False')
 
-        if PY3 and not isinstance(path, _text_type):
+        if not isinstance(path, str):
             fs_encoding = sys.getfilesystemencoding()
             path = path.decode(fs_encoding)  # path to unicode
 
         self.path = path
 
         # Set other option attributes, using defaults where necessary
         self.index_url = index_url if index_url is not None else INDEX_URL
@@ -236,44 +271,28 @@
             # bootstrapper manually after reconfiguring it.
             bootstrapper.run()
 
         return bootstrapper
 
     @classmethod
     def parse_config(cls):
-        if not os.path.exists('setup.cfg'):
-            return {}
-
-        cfg = ConfigParser()
-
-        try:
-            cfg.read('setup.cfg')
-        except Exception as e:
-            if DEBUG:
-                raise
-
-            log.error(
-                "Error reading setup.cfg: {0!r}\n{1} will not be "
-                "automatically bootstrapped and package installation may fail."
-                "\n{2}".format(e, PACKAGE_NAME, _err_help_msg))
-            return {}
 
-        if not cfg.has_section('ah_bootstrap'):
+        if not SETUP_CFG.has_section('ah_bootstrap'):
             return {}
 
         config = {}
 
         for option, type_ in CFG_OPTIONS:
-            if not cfg.has_option('ah_bootstrap', option):
+            if not SETUP_CFG.has_option('ah_bootstrap', option):
                 continue
 
             if type_ is bool:
-                value = cfg.getboolean('ah_bootstrap', option)
+                value = SETUP_CFG.getboolean('ah_bootstrap', option)
             else:
-                value = cfg.get('ah_bootstrap', option)
+                value = SETUP_CFG.get('ah_bootstrap', option)
 
             config[option] = value
 
         return config
 
     @classmethod
     def parse_command_line(cls, argv=None):
@@ -512,15 +531,17 @@
             def get_option_dict(self, command_name):
                 opts = Distribution.get_option_dict(self, command_name)
                 if command_name == 'easy_install':
                     if find_links is not None:
                         opts['find_links'] = ('setup script', find_links)
                     if index_url is not None:
                         opts['index_url'] = ('setup script', index_url)
-                    if allow_hosts is not None:
+                    # For setuptools>=42, the allow_hosts option can't
+                    # be used because pip doesn't support it.
+                    if allow_hosts is not None and SETUPTOOLS_LT_42:
                         opts['allow_hosts'] = ('setup script', allow_hosts)
                 return opts
 
         if version:
             req = '{0}=={1}'.format(DIST_NAME, version)
         else:
             if UPPER_VERSION_EXCLUSIVE is None:
@@ -654,16 +675,16 @@
         # correct)
         #
         # 3. The output of `git describe` for the submodule's current commit
         # hash (this includes for example what branches the commit is on) but
         # only if the submodule is initialized.  We ignore this information for
         # now
         _git_submodule_status_re = re.compile(
-            '^(?P<status>[+-U ])(?P<commit>[0-9a-f]{40}) '
-            '(?P<submodule>\S+)( .*)?$')
+            r'^(?P<status>[+-U ])(?P<commit>[0-9a-f]{40}) '
+            r'(?P<submodule>\S+)( .*)?$')
 
         # The stdout should only contain one line--the status of the
         # requested submodule
         m = _git_submodule_status_re.match(stdout)
         if m:
             # Yes, the path *is* a git submodule
             self._update_submodule(m.group('submodule'), m.group('status'))
@@ -825,17 +846,17 @@
     except ValueError:
         # Due to an OSX oddity locale.getdefaultlocale() can also crash
         # depending on the user's locale/language settings.  See:
         # http://bugs.python.org/issue18378
         stdio_encoding = 'latin1'
 
     # Unlikely to fail at this point but even then let's be flexible
-    if not isinstance(stdout, _text_type):
+    if not isinstance(stdout, str):
         stdout = stdout.decode(stdio_encoding, 'replace')
-    if not isinstance(stderr, _text_type):
+    if not isinstance(stderr, str):
         stderr = stderr.decode(stdio_encoding, 'replace')
 
     return (p.returncode, stdout, stderr)
 
 
 def _next_version(version):
     """
@@ -907,22 +928,14 @@
         raise
 
     if not exception_occurred:
         sys.stdout = old_stdout
         sys.stderr = old_stderr
 
 
-_err_help_msg = """
-If the problem persists consider installing astropy_helpers manually using pip
-(`pip install astropy_helpers`) or by manually downloading the source archive,
-extracting it, and installing by running `python setup.py install` from the
-root of the extracted source code.
-"""
-
-
 class _AHBootstrapSystemExit(SystemExit):
     def __init__(self, *args):
         if not args:
             msg = 'An unknown problem occurred bootstrapping astropy_helpers.'
         else:
             msg = args[0]
```

### Comparing `speclite-0.8/astropy_helpers/ah_bootstrap.py` & `speclite-0.9/astropy_helpers/ah_bootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,85 +15,159 @@
 When this module is imported or otherwise executed it automatically calls a
 main function that attempts to read the project's setup.cfg file, which it
 checks for a configuration section called ``[ah_bootstrap]`` the presences of
 that section, and options therein, determine the next step taken:  If it
 contains an option called ``auto_use`` with a value of ``True``, it will
 automatically call the main function of this module called
 `use_astropy_helpers` (see that function's docstring for full details).
-Otherwise no further action is taken (however,
-``ah_bootstrap.use_astropy_helpers`` may be called manually from within the
-setup.py script).
+Otherwise no further action is taken and by default the system-installed version
+of astropy-helpers will be used (however, ``ah_bootstrap.use_astropy_helpers``
+may be called manually from within the setup.py script).
+
+This behavior can also be controlled using the ``--auto-use`` and
+``--no-auto-use`` command-line flags. For clarity, an alias for
+``--no-auto-use`` is ``--use-system-astropy-helpers``, and we recommend using
+the latter if needed.
 
 Additional options in the ``[ah_boostrap]`` section of setup.cfg have the same
 names as the arguments to `use_astropy_helpers`, and can be used to configure
 the bootstrap script when ``auto_use = True``.
 
 See https://github.com/astropy/astropy-helpers for more details, and for the
 latest version of this module.
 """
 
 import contextlib
 import errno
-import imp
 import io
 import locale
 import os
 import re
 import subprocess as sp
 import sys
 
-try:
-    from ConfigParser import ConfigParser, RawConfigParser
-except ImportError:
-    from configparser import ConfigParser, RawConfigParser
+from distutils import log
+from distutils.debug import DEBUG
+
+from configparser import ConfigParser, RawConfigParser
+
+import pkg_resources
+
+from setuptools import Distribution
+from setuptools.package_index import PackageIndex
+
+# This is the minimum Python version required for astropy-helpers
+__minimum_python_version__ = (3, 5)
+
+# TODO: Maybe enable checking for a specific version of astropy_helpers?
+DIST_NAME = 'astropy-helpers'
+PACKAGE_NAME = 'astropy_helpers'
+UPPER_VERSION_EXCLUSIVE = None
+
+# Defaults for other options
+DOWNLOAD_IF_NEEDED = True
+INDEX_URL = 'https://pypi.python.org/simple'
+USE_GIT = True
+OFFLINE = False
+AUTO_UPGRADE = True
+
+# A list of all the configuration options and their required types
+CFG_OPTIONS = [
+    ('auto_use', bool), ('path', str), ('download_if_needed', bool),
+    ('index_url', str), ('use_git', bool), ('offline', bool),
+    ('auto_upgrade', bool)
+]
+
+# Start off by parsing the setup.cfg file
+
+_err_help_msg = """
+If the problem persists consider installing astropy_helpers manually using pip
+(`pip install astropy_helpers`) or by manually downloading the source archive,
+extracting it, and installing by running `python setup.py install` from the
+root of the extracted source code.
+"""
+
+SETUP_CFG = ConfigParser()
+
+if os.path.exists('setup.cfg'):
 
+    try:
+        SETUP_CFG.read('setup.cfg')
+    except Exception as e:
+        if DEBUG:
+            raise
 
-if sys.version_info[0] < 3:
-    _str_types = (str, unicode)
-    _text_type = unicode
-    PY3 = False
+        log.error(
+            "Error reading setup.cfg: {0!r}\n{1} will not be "
+            "automatically bootstrapped and package installation may fail."
+            "\n{2}".format(e, PACKAGE_NAME, _err_help_msg))
+
+# We used package_name in the package template for a while instead of name
+if SETUP_CFG.has_option('metadata', 'name'):
+    parent_package = SETUP_CFG.get('metadata', 'name')
+elif SETUP_CFG.has_option('metadata', 'package_name'):
+    parent_package = SETUP_CFG.get('metadata', 'package_name')
 else:
-    _str_types = (str, bytes)
-    _text_type = str
-    PY3 = True
+    parent_package = None
+
+if SETUP_CFG.has_option('options', 'python_requires'):
+
+    python_requires = SETUP_CFG.get('options', 'python_requires')
+
+    # The python_requires key has a syntax that can be parsed by SpecifierSet
+    # in the packaging package. However, we don't want to have to depend on that
+    # package, so instead we can use setuptools (which bundles packaging). We
+    # have to add 'python' to parse it with Requirement.
+
+    from pkg_resources import Requirement
+    req = Requirement.parse('python' + python_requires)
+
+    # We want the Python version as a string, which we can get from the platform module
+    import platform
+    # strip off trailing '+' incase this is a dev install of python
+    python_version = platform.python_version().strip('+')
+    # allow pre-releases to count as 'new enough'
+    if not req.specifier.contains(python_version, True):
+        if parent_package is None:
+            message = "ERROR: Python {} is required by this package\n".format(req.specifier)
+        else:
+            message = "ERROR: Python {} is required by {}\n".format(req.specifier, parent_package)
+        sys.stderr.write(message)
+        sys.exit(1)
+
+if sys.version_info < __minimum_python_version__:
+
+    if parent_package is None:
+        message = "ERROR: Python {} or later is required by astropy-helpers\n".format(
+            __minimum_python_version__)
+    else:
+        message = "ERROR: Python {} or later is required by astropy-helpers for {}\n".format(
+            __minimum_python_version__, parent_package)
+
+    sys.stderr.write(message)
+    sys.exit(1)
+
+_str_types = (str, bytes)
 
 
 # What follows are several import statements meant to deal with install-time
 # issues with either missing or misbehaving pacakges (including making sure
 # setuptools itself is installed):
 
+# Check that setuptools 30.3 or later is present
+from distutils.version import LooseVersion
 
-# Some pre-setuptools checks to ensure that either distribute or setuptools >=
-# 0.7 is used (over pre-distribute setuptools) if it is available on the path;
-# otherwise the latest setuptools will be downloaded and bootstrapped with
-# ``ez_setup.py``.  This used to be included in a separate file called
-# setuptools_bootstrap.py; but it was combined into ah_bootstrap.py
 try:
-    import pkg_resources
-    _setuptools_req = pkg_resources.Requirement.parse('setuptools>=0.7')
-    # This may raise a DistributionNotFound in which case no version of
-    # setuptools or distribute is properly installed
-    _setuptools = pkg_resources.get_distribution('setuptools')
-    if _setuptools not in _setuptools_req:
-        # Older version of setuptools; check if we have distribute; again if
-        # this results in DistributionNotFound we want to give up
-        _distribute = pkg_resources.get_distribution('distribute')
-        if _setuptools != _distribute:
-            # It's possible on some pathological systems to have an old version
-            # of setuptools and distribute on sys.path simultaneously; make
-            # sure distribute is the one that's used
-            sys.path.insert(1, _distribute.location)
-            _distribute.activate()
-            imp.reload(pkg_resources)
-except:
-    # There are several types of exceptions that can occur here; if all else
-    # fails bootstrap and use the bootstrapped version
-    from ez_setup import use_setuptools
-    use_setuptools()
+    import setuptools
+    assert LooseVersion(setuptools.__version__) >= LooseVersion('30.3')
+except (ImportError, AssertionError):
+    sys.stderr.write("ERROR: setuptools 30.3 or later is required by astropy-helpers\n")
+    sys.exit(1)
 
+SETUPTOOLS_LT_42 = LooseVersion(setuptools.__version__) < LooseVersion('42')
 
 # typing as a dependency for 1.6.1+ Sphinx causes issues when imported after
 # initializing submodule with ah_boostrap.py
 # See discussion and references in
 # https://github.com/astropy/astropy-helpers/issues/302
 
 try:
@@ -128,44 +202,14 @@
     # Ignore if this fails for *any* reason*
     pass
 
 
 # End compatibility imports...
 
 
-# In case it didn't successfully import before the ez_setup checks
-import pkg_resources
-
-from setuptools import Distribution
-from setuptools.package_index import PackageIndex
-from setuptools.sandbox import run_setup
-
-from distutils import log
-from distutils.debug import DEBUG
-
-
-# TODO: Maybe enable checking for a specific version of astropy_helpers?
-DIST_NAME = 'astropy-helpers'
-PACKAGE_NAME = 'astropy_helpers'
-
-# Defaults for other options
-DOWNLOAD_IF_NEEDED = True
-INDEX_URL = 'https://pypi.python.org/simple'
-USE_GIT = True
-OFFLINE = False
-AUTO_UPGRADE = True
-
-# A list of all the configuration options and their required types
-CFG_OPTIONS = [
-    ('auto_use', bool), ('path', str), ('download_if_needed', bool),
-    ('index_url', str), ('use_git', bool), ('offline', bool),
-    ('auto_upgrade', bool)
-]
-
-
 class _Bootstrapper(object):
     """
     Bootstrapper implementation.  See ``use_astropy_helpers`` for parameter
     documentation.
     """
 
     def __init__(self, path=None, index_url=None, use_git=None, offline=None,
@@ -173,15 +217,15 @@
 
         if path is None:
             path = PACKAGE_NAME
 
         if not (isinstance(path, _str_types) or path is False):
             raise TypeError('path must be a string or False')
 
-        if PY3 and not isinstance(path, _text_type):
+        if not isinstance(path, str):
             fs_encoding = sys.getfilesystemencoding()
             path = path.decode(fs_encoding)  # path to unicode
 
         self.path = path
 
         # Set other option attributes, using defaults where necessary
         self.index_url = index_url if index_url is not None else INDEX_URL
@@ -227,44 +271,28 @@
             # bootstrapper manually after reconfiguring it.
             bootstrapper.run()
 
         return bootstrapper
 
     @classmethod
     def parse_config(cls):
-        if not os.path.exists('setup.cfg'):
-            return {}
-
-        cfg = ConfigParser()
-
-        try:
-            cfg.read('setup.cfg')
-        except Exception as e:
-            if DEBUG:
-                raise
 
-            log.error(
-                "Error reading setup.cfg: {0!r}\n{1} will not be "
-                "automatically bootstrapped and package installation may fail."
-                "\n{2}".format(e, PACKAGE_NAME, _err_help_msg))
-            return {}
-
-        if not cfg.has_section('ah_bootstrap'):
+        if not SETUP_CFG.has_section('ah_bootstrap'):
             return {}
 
         config = {}
 
         for option, type_ in CFG_OPTIONS:
-            if not cfg.has_option('ah_bootstrap', option):
+            if not SETUP_CFG.has_option('ah_bootstrap', option):
                 continue
 
             if type_ is bool:
-                value = cfg.getboolean('ah_bootstrap', option)
+                value = SETUP_CFG.getboolean('ah_bootstrap', option)
             else:
-                value = cfg.get('ah_bootstrap', option)
+                value = SETUP_CFG.get('ah_bootstrap', option)
 
             config[option] = value
 
         return config
 
     @classmethod
     def parse_command_line(cls, argv=None):
@@ -283,14 +311,26 @@
             config['use_git'] = False
             argv.remove('--no-git')
 
         if '--offline' in argv:
             config['offline'] = True
             argv.remove('--offline')
 
+        if '--auto-use' in argv:
+            config['auto_use'] = True
+            argv.remove('--auto-use')
+
+        if '--no-auto-use' in argv:
+            config['auto_use'] = False
+            argv.remove('--no-auto-use')
+
+        if '--use-system-astropy-helpers' in argv:
+            config['auto_use'] = False
+            argv.remove('--use-system-astropy-helpers')
+
         return config
 
     def run(self):
         strategies = ['local_directory', 'local_file', 'index']
         dist = None
 
         # First, remove any previously imported versions of astropy_helpers;
@@ -460,17 +500,18 @@
         dist = ws.by_key.get(DIST_NAME)
 
         if dist is None:
             # We didn't find an egg-info/dist-info in the given path, but if a
             # setup.py exists we can generate it
             setup_py = os.path.join(path, 'setup.py')
             if os.path.isfile(setup_py):
-                with _silence():
-                    run_setup(os.path.join(path, 'setup.py'),
-                              ['egg_info'])
+                # We use subprocess instead of run_setup from setuptools to
+                # avoid segmentation faults - see the following for more details:
+                # https://github.com/cython/cython/issues/2104
+                sp.check_output([sys.executable, 'setup.py', 'egg_info'], cwd=path)
 
                 for dist in pkg_resources.find_distributions(path, True):
                     # There should be only one...
                     return dist
 
         return dist
 
@@ -490,31 +531,49 @@
             def get_option_dict(self, command_name):
                 opts = Distribution.get_option_dict(self, command_name)
                 if command_name == 'easy_install':
                     if find_links is not None:
                         opts['find_links'] = ('setup script', find_links)
                     if index_url is not None:
                         opts['index_url'] = ('setup script', index_url)
-                    if allow_hosts is not None:
+                    # For setuptools>=42, the allow_hosts option can't
+                    # be used because pip doesn't support it.
+                    if allow_hosts is not None and SETUPTOOLS_LT_42:
                         opts['allow_hosts'] = ('setup script', allow_hosts)
                 return opts
 
         if version:
             req = '{0}=={1}'.format(DIST_NAME, version)
         else:
-            req = DIST_NAME
+            if UPPER_VERSION_EXCLUSIVE is None:
+                req = DIST_NAME
+            else:
+                req = '{0}<{1}'.format(DIST_NAME, UPPER_VERSION_EXCLUSIVE)
 
         attrs = {'setup_requires': [req]}
 
+        # NOTE: we need to parse the config file (e.g. setup.cfg) to make sure
+        # it honours the options set in the [easy_install] section, and we need
+        # to explicitly fetch the requirement eggs as setup_requires does not
+        # get honored in recent versions of setuptools:
+        # https://github.com/pypa/setuptools/issues/1273
+
         try:
-            if DEBUG:
-                _Distribution(attrs=attrs)
-            else:
-                with _silence():
-                    _Distribution(attrs=attrs)
+
+            context = _verbose if DEBUG else _silence
+            with context():
+                dist = _Distribution(attrs=attrs)
+                try:
+                    dist.parse_config_files(ignore_option_errors=True)
+                    dist.fetch_build_eggs(req)
+                except TypeError:
+                    # On older versions of setuptools, ignore_option_errors
+                    # doesn't exist, and the above two lines are not needed
+                    # so we can just continue
+                    pass
 
             # If the setup_requires succeeded it will have added the new dist to
             # the main working_set
             return pkg_resources.working_set.by_key.get(DIST_NAME)
         except Exception as e:
             if DEBUG:
                 raise
@@ -616,16 +675,16 @@
         # correct)
         #
         # 3. The output of `git describe` for the submodule's current commit
         # hash (this includes for example what branches the commit is on) but
         # only if the submodule is initialized.  We ignore this information for
         # now
         _git_submodule_status_re = re.compile(
-            '^(?P<status>[+-U ])(?P<commit>[0-9a-f]{40}) '
-            '(?P<submodule>\S+)( .*)?$')
+            r'^(?P<status>[+-U ])(?P<commit>[0-9a-f]{40}) '
+            r'(?P<submodule>\S+)( .*)?$')
 
         # The stdout should only contain one line--the status of the
         # requested submodule
         m = _git_submodule_status_re.match(stdout)
         if m:
             # Yes, the path *is* a git submodule
             self._update_submodule(m.group('submodule'), m.group('status'))
@@ -787,17 +846,17 @@
     except ValueError:
         # Due to an OSX oddity locale.getdefaultlocale() can also crash
         # depending on the user's locale/language settings.  See:
         # http://bugs.python.org/issue18378
         stdio_encoding = 'latin1'
 
     # Unlikely to fail at this point but even then let's be flexible
-    if not isinstance(stdout, _text_type):
+    if not isinstance(stdout, str):
         stdout = stdout.decode(stdio_encoding, 'replace')
-    if not isinstance(stderr, _text_type):
+    if not isinstance(stderr, str):
         stderr = stderr.decode(stdio_encoding, 'replace')
 
     return (p.returncode, stdout, stderr)
 
 
 def _next_version(version):
     """
@@ -843,14 +902,18 @@
         pass
 
     def flush(self):
         pass
 
 
 @contextlib.contextmanager
+def _verbose():
+    yield
+
+@contextlib.contextmanager
 def _silence():
     """A context manager that silences sys.stdout and sys.stderr."""
 
     old_stdout = sys.stdout
     old_stderr = sys.stderr
     sys.stdout = _DummyFile()
     sys.stderr = _DummyFile()
@@ -865,22 +928,14 @@
         raise
 
     if not exception_occurred:
         sys.stdout = old_stdout
         sys.stderr = old_stderr
 
 
-_err_help_msg = """
-If the problem persists consider installing astropy_helpers manually using pip
-(`pip install astropy_helpers`) or by manually downloading the source archive,
-extracting it, and installing by running `python setup.py install` from the
-root of the extracted source code.
-"""
-
-
 class _AHBootstrapSystemExit(SystemExit):
     def __init__(self, *args):
         if not args:
             msg = 'An unknown problem occurred bootstrapping astropy_helpers.'
         else:
             msg = args[0]
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/__init__.py` & `speclite-0.9/astropy_helpers/astropy_helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,11 @@
 # Ensure that all module-level code in astropy or other packages know that
 # we're in setup mode:
 if ('__main__' in sys.modules and
         hasattr(sys.modules['__main__'], '__file__')):
     filename = os.path.basename(sys.modules['__main__'].__file__)
 
     if filename.rstrip('co') == 'setup.py':
-        if sys.version_info[0] >= 3:
-            import builtins
-        else:
-            import __builtin__ as builtins
+        import builtins
         builtins._ASTROPY_SETUP_ = True
 
     del filename
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/commands/_dummy.py` & `speclite-0.9/astropy_helpers/astropy_helpers/commands/_dummy.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,17 @@
 
         if not hasattr(cls, 'error_msg'):
             raise TypeError(
                 "_DummyCommand subclass must have an 'error_msg' "
                 "attribute.")
 
     def __getattribute__(cls, attr):
-        if attr in ('description', 'error_msg'):
+        if attr in ('description', 'error_msg') or attr.startswith('_'):
             # Allow cls.description to work so that `./setup.py
             # --help-commands` still works
             return super(_DummyCommandMeta, cls).__getattribute__(attr)
 
         raise DistutilsArgError(cls.error_msg)
 
 
-if sys.version_info[0] < 3:
-    exec(dedent("""
-        class _DummyCommand(Command, object):
-            __metaclass__ = _DummyCommandMeta
-    """))
-else:
-    exec(dedent("""
-        class _DummyCommand(Command, object, metaclass=_DummyCommandMeta):
-            pass
-    """))
+class _DummyCommand(Command, object, metaclass=_DummyCommandMeta):
+    pass
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/commands/src/compiler.c` & `speclite-0.9/astropy_helpers/astropy_helpers/commands/src/compiler.c`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 /***************************************************************************
  * Macros for determining the compiler version.
  *
  * These are borrowed from boost, and majorly abridged to include only
  * the compilers we care about.
  ***************************************************************************/
 
-#ifndef PY3K
-#if PY_MAJOR_VERSION >= 3
-#define PY3K 1
-#else
-#define PY3K 0
-#endif
-#endif
-
-
 #define STRINGIZE(X) DO_STRINGIZE(X)
 #define DO_STRINGIZE(X) #X
 
 #if defined __clang__
 /*  Clang C++ emulates GCC, so it has to appear early. */
 #    define COMPILER "Clang version " __clang_version__
 
@@ -80,50 +71,37 @@
 struct module_state {
 /* The Sun compiler can't handle empty structs */
 #if defined(__SUNPRO_C) || defined(_MSC_VER)
     int _dummy;
 #endif
 };
 
-#if PY3K
-    static struct PyModuleDef moduledef = {
-        PyModuleDef_HEAD_INIT,
-        "_compiler",
-        NULL,
-        sizeof(struct module_state),
-        NULL,
-        NULL,
-        NULL,
-        NULL,
-        NULL
-    };
-
-    #define INITERROR return NULL
+static struct PyModuleDef moduledef = {
+    PyModuleDef_HEAD_INIT,
+    "compiler_version",
+    NULL,
+    sizeof(struct module_state),
+    NULL,
+    NULL,
+    NULL,
+    NULL,
+    NULL
+};
 
-    PyMODINIT_FUNC
-    PyInit__compiler(void)
+#define INITERROR return NULL
 
-#else
-    #define INITERROR return
+PyMODINIT_FUNC
+PyInit_compiler_version(void)
 
-    PyMODINIT_FUNC
-    init_compiler(void)
-#endif
 
 {
   PyObject* m;
 
-#if PY3K
   m = PyModule_Create(&moduledef);
-#else
-  m = Py_InitModule3("_compiler", NULL, NULL);
-#endif
 
   if (m == NULL)
     INITERROR;
 
   PyModule_AddStringConstant(m, "compiler", COMPILER);
 
-#if PY3K
   return m;
-#endif
 }
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/distutils_helpers.py` & `speclite-0.9/astropy_helpers/astropy_helpers/distutils_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,20 @@
             # get raise for ./setup.py --help SystemExit can be raised if a
             # display option was used, for example
             pass
 
     return dist
 
 
+def get_main_package_directory(distribution):
+    """
+    Given a Distribution object, return the main package directory.
+    """
+    return min(distribution.packages, key=len).replace('.', os.sep)
+
 def get_distutils_option(option, commands):
     """ Returns the value of the given distutils option.
 
     Parameters
     ----------
     option : str
         The name of the option
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/git_helpers.py` & `speclite-0.9/astropy_helpers/astropy_helpers/git_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # BEGIN
 
 import locale
 import os
 import subprocess
 import warnings
 
+__all__ = ['get_git_devstr']
+
 
 def _decode_stdio(stream):
     try:
         stdio_encoding = locale.getdefaultlocale()[1] or 'utf-8'
     except ValueError:
         stdio_encoding = 'utf-8'
 
@@ -86,16 +88,14 @@
         SHA1 hash of the current commit (if `sha` is True), or an empty string
         if git version info could not be identified.
 
     """
 
     if path is None:
         path = os.getcwd()
-        if not _get_repo_path(path, levels=0):
-            return ''
 
     if not os.path.isdir(path):
         path = os.path.abspath(os.path.dirname(path))
 
     if sha:
         # Faster for getting just the hash of HEAD
         cmd = ['rev-parse', 'HEAD']
@@ -131,15 +131,20 @@
                               'count: {0}'.format(_decode_stdio(stderr)))
             return (p.returncode, stdout, stderr)
 
         return p.returncode, stdout, stderr
 
     returncode, stdout, stderr = run_git(cmd)
 
-    if not sha and returncode == 129:
+    if not sha and returncode == 128:
+        # git returns 128 if the command is not run from within a git
+        # repository tree. In this case, a warning is produced above but we
+        # return the default dev version of '0'.
+        return '0'
+    elif not sha and returncode == 129:
         # git returns 129 if a command option failed to parse; in
         # particular this could happen in git versions older than 1.7.2
         # where the --count option is not supported
         # Also use --abbrev-commit and --abbrev=0 to display the minimum
         # number of characters needed per-commit (rather than the full hash)
         cmd = ['rev-list', '--abbrev-commit', '--abbrev=0', 'HEAD']
         returncode, stdout, stderr = run_git(cmd)
@@ -151,15 +156,17 @@
             return ''
     elif sha:
         return _decode_stdio(stdout)[:40]
     else:
         return _decode_stdio(stdout).strip()
 
 
-def _get_repo_path(pathname, levels=None):
+# This function is tested but it is only ever executed within a subprocess when
+# creating a fake package, so it doesn't get picked up by coverage metrics.
+def _get_repo_path(pathname, levels=None):  # pragma: no cover
     """
     Given a file or directory name, determine the root of the git repository
     this path is under.  If given, this won't look any higher than ``levels``
     (that is, if ``levels=0`` then the given path must be the root of the git
     repository and is returned if so.
 
     Returns `None` if the given path could not be determined to belong to a git
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/setup_helpers.py` & `speclite-0.9/astropy_helpers/astropy_helpers/setup_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module contains a number of utilities for use during
 setup/build/packaging that are useful to astropy as a whole.
 """
 
-from __future__ import absolute_import, print_function
-
 import collections
 import os
 import re
 import subprocess
 import sys
 import traceback
 import warnings
+from configparser import ConfigParser
+import builtins
 
 from distutils import log
-from distutils.dist import Distribution
 from distutils.errors import DistutilsOptionError, DistutilsModuleError
 from distutils.core import Extension
 from distutils.core import Command
 from distutils.command.sdist import sdist as DistutilsSdist
 
+from setuptools import setup as setuptools_setup
+from setuptools.config import read_configuration
 from setuptools import find_packages as _find_packages
 
 from .distutils_helpers import (add_command_option, get_compiler_option,
                                 get_dummy_distribution, get_distutils_build_option,
                                 get_distutils_build_or_install_option)
-from .version_helpers import get_pkg_version_module
+from .version_helpers import get_pkg_version_module, generate_version_py
 from .utils import (walk_skip_hidden, import_file, extends_doc,
                     resolve_name, AstropyDeprecationWarning)
 
-from .commands.build_ext import generate_build_ext_command
-from .commands.build_py import AstropyBuildPy
-from .commands.install import AstropyInstall
-from .commands.install_lib import AstropyInstallLib
-from .commands.register import AstropyRegister
+from .commands.build_ext import AstropyHelpersBuildExt
 from .commands.test import AstropyTest
 
 # These imports are not used in this module, but are included for backwards
 # compat with older versions of this module
 from .utils import get_numpy_include_path, write_if_different  # noqa
-from .commands.build_ext import should_build_with_cython, get_compiler_version  # noqa
+
+__all__ = ['register_commands', 'get_package_info']
 
 _module_state = {'registered_commands': None,
                  'have_sphinx': False,
-                 'package_cache': None}
+                 'package_cache': None,
+                 'exclude_packages': set(),
+                 'excludes_too_late': False}
 
 try:
     import sphinx  # noqa
     _module_state['have_sphinx'] = True
 except ValueError as e:
     # This can occur deep in the bowels of Sphinx's imports by way of docutils
     # and an occurrence of this bug: http://bugs.python.org/issue18378
@@ -63,45 +63,54 @@
 except ImportError:
     pass
 except SyntaxError:
     # occurs if markupsafe is recent version, which doesn't support Python 3.2
     pass
 
 
-PY3 = sys.version_info[0] >= 3
+def setup(**kwargs):
+    """
+    A wrapper around setuptools' setup() function that automatically sets up
+    custom commands, generates a version file, and customizes the setup process
+    via the ``setup_package.py`` files.
+    """
+
+    # DEPRECATED: store the package name in a built-in variable so it's easy
+    # to get from other parts of the setup infrastructure. We should phase this
+    # out in packages that use it - the cookiecutter template should now be
+    # able to put the right package name where needed.
+    conf = read_configuration('setup.cfg')
+    builtins._ASTROPY_PACKAGE_NAME_ = conf['metadata']['name']
+
+    # Create a dictionary with setup command overrides. Note that this gets
+    # information about the package (name and version) from the setup.cfg file.
+    cmdclass = register_commands()
+
+    # Freeze build information in version.py. Note that this gets information
+    # about the package (name and version) from the setup.cfg file.
+    version = generate_version_py()
+
+    # Get configuration information from all of the various subpackages.
+    # See the docstring for setup_helpers.update_package_files for more
+    # details.
+    package_info = get_package_info()
+    package_info['cmdclass'] = cmdclass
+    package_info['version'] = version
 
+    # Override using any specified keyword arguments
+    package_info.update(kwargs)
 
-# This adds a new keyword to the setup() function
-Distribution.skip_2to3 = []
+    setuptools_setup(**package_info)
 
 
 def adjust_compiler(package):
-    """
-    This function detects broken compilers and switches to another.  If
-    the environment variable CC is explicitly set, or a compiler is
-    specified on the commandline, no override is performed -- the purpose
-    here is to only override a default compiler.
-
-    The specific compilers with problems are:
-
-        * The default compiler in XCode-4.2, llvm-gcc-4.2,
-          segfaults when compiling wcslib.
-
-    The set of broken compilers can be updated by changing the
-    compiler_mapping variable.  It is a list of 2-tuples where the
-    first in the pair is a regular expression matching the version
-    of the broken compiler, and the second is the compiler to change
-    to.
-    """
-
     warnings.warn(
-        'Direct use of the adjust_compiler function in setup.py is '
-        'deprecated and can be removed from your setup.py.  This '
-        'functionality is now incorporated directly into the build_ext '
-        'command.', AstropyDeprecationWarning)
+        'The adjust_compiler function in setup.py is '
+        'deprecated and can be removed from your setup.py.',
+        AstropyDeprecationWarning)
 
 
 def get_debug_option(packagename):
     """ Determines if the build is in debug mode.
 
     Returns
     -------
@@ -123,20 +132,70 @@
     if any(cmd in dist.commands for cmd in ['build', 'build_ext']):
         debug = bool(get_distutils_build_option('debug'))
     else:
         debug = bool(current_debug)
 
     if current_debug is not None and current_debug != debug:
         build_ext_cmd = dist.get_command_class('build_ext')
-        build_ext_cmd.force_rebuild = True
+        build_ext_cmd._force_rebuild = True
 
     return debug
 
 
-def register_commands(package, version, release, srcdir='.'):
+def add_exclude_packages(excludes):
+
+    if _module_state['excludes_too_late']:
+        raise RuntimeError(
+            "add_package_excludes must be called before all other setup helper "
+            "functions in order to properly handle excluded packages")
+
+    _module_state['exclude_packages'].update(set(excludes))
+
+
+def register_commands(package=None, version=None, release=None, srcdir='.'):
+    """
+    This function generates a dictionary containing customized commands that
+    can then be passed to the ``cmdclass`` argument in ``setup()``.
+    """
+
+    if package is not None:
+        warnings.warn('The package argument to generate_version_py has '
+                      'been deprecated and will be removed in future. Specify '
+                      'the package name in setup.cfg instead', AstropyDeprecationWarning)
+
+    if version is not None:
+        warnings.warn('The version argument to generate_version_py has '
+                      'been deprecated and will be removed in future. Specify '
+                      'the version number in setup.cfg instead', AstropyDeprecationWarning)
+
+    if release is not None:
+        warnings.warn('The release argument to generate_version_py has '
+                      'been deprecated and will be removed in future. We now '
+                      'use the presence of the "dev" string in the version to '
+                      'determine whether this is a release', AstropyDeprecationWarning)
+
+    # We use ConfigParser instead of read_configuration here because the latter
+    # only reads in keys recognized by setuptools, but we need to access
+    # package_name below.
+    conf = ConfigParser()
+    conf.read('setup.cfg')
+
+    if conf.has_option('metadata', 'name'):
+        package = conf.get('metadata', 'name')
+    elif conf.has_option('metadata', 'package_name'):
+        # The package-template used package_name instead of name for a while
+        warnings.warn('Specifying the package name using the "package_name" '
+                      'option in setup.cfg is deprecated - use the "name" '
+                      'option instead.', AstropyDeprecationWarning)
+        package = conf.get('metadata', 'package_name')
+    elif package is not None:  # deprecated
+        pass
+    else:
+        sys.stderr.write('ERROR: Could not read package name from setup.cfg\n')
+        sys.exit(1)
 
     if _module_state['registered_commands'] is not None:
         return _module_state['registered_commands']
 
     if _module_state['have_sphinx']:
         try:
             from .commands.build_sphinx import (AstropyBuildSphinx,
@@ -150,28 +209,15 @@
         'test': generate_test_command(package),
 
         # Use distutils' sdist because it respects package_data.
         # setuptools/distributes sdist requires duplication of information in
         # MANIFEST.in
         'sdist': DistutilsSdist,
 
-        # The exact form of the build_ext command depends on whether or not
-        # we're building a release version
-        'build_ext': generate_build_ext_command(package, release),
-
-        # We have a custom build_py to generate the default configuration file
-        'build_py': AstropyBuildPy,
-
-        # Since install can (in some circumstances) be run without
-        # first building, we also need to override install and
-        # install_lib.  See #2223
-        'install': AstropyInstall,
-        'install_lib': AstropyInstallLib,
-
-        'register': AstropyRegister,
+        'build_ext': AstropyHelpersBuildExt,
         'build_sphinx': AstropyBuildSphinx,
         'build_docs': AstropyBuildDocs
     }
 
     # Need to override the __name__ here so that the commandline options are
     # presented as being related to the "build" command, for example; normally
     # this wouldn't be necessary since commands also have a command_name
@@ -212,15 +258,15 @@
     # written)
     def get_command_name(cmdcls):
         if hasattr(cmdcls, 'command_name'):
             return cmdcls.command_name
         else:
             return cmdcls.__name__
 
-    packages = filter_packages(find_packages(srcdir))
+    packages = find_packages(srcdir)
     dist = get_dummy_distribution()
 
     hooks = collections.defaultdict(dict)
 
     for setuppkg in iter_setup_packages(srcdir, packages):
         for name, obj in vars(setuppkg).items():
             match = hook_re.match(name)
@@ -334,16 +380,15 @@
     ``setup.py`` for example usage and the Astropy development docs
     for more details.
 
     This function obtains that information by iterating through all
     packages in ``srcdir`` and locating a ``setup_package.py`` module.
     This module can contain the following functions:
     ``get_extensions()``, ``get_package_data()``,
-    ``get_build_options()``, ``get_external_libraries()``,
-    and ``requires_2to3()``.
+    ``get_build_options()``, and ``get_external_libraries()``.
 
     Each of those functions take no arguments.
 
     - ``get_extensions`` returns a list of
       `distutils.extension.Extension` objects.
 
     - ``get_package_data()`` returns a dict formatted as required by
@@ -351,31 +396,39 @@
 
     - ``get_build_options()`` returns a list of tuples describing the
       extra build options to add.
 
     - ``get_external_libraries()`` returns
       a list of libraries that can optionally be built using external
       dependencies.
-
-    - ``get_entry_points()`` returns a dict formatted as required by
-      the ``entry_points`` argument to ``setup()``.
-
-    - ``requires_2to3()`` should return `True` when the source code
-      requires `2to3` processing to run on Python 3.x.  If
-      ``requires_2to3()`` is missing, it is assumed to return `True`.
-
     """
     ext_modules = []
     packages = []
-    package_data = {}
     package_dir = {}
-    skip_2to3 = []
+
+    # Read in existing package data, and add to it below
+    setup_cfg = os.path.join(srcdir, 'setup.cfg')
+    if os.path.exists(setup_cfg):
+        conf = read_configuration(setup_cfg)
+        if 'options' in conf and 'package_data' in conf['options']:
+            package_data = conf['options']['package_data']
+        else:
+            package_data = {}
+    else:
+        package_data = {}
+
+    if exclude:
+        warnings.warn(
+            "Use of the exclude parameter is no longer supported since it does "
+            "not work as expected. Use add_exclude_packages instead. Note that "
+            "it must be called prior to any other calls from setup helpers.",
+            AstropyDeprecationWarning)
 
     # Use the find_packages tool to locate all packages and modules
-    packages = filter_packages(find_packages(srcdir, exclude=exclude))
+    packages = find_packages(srcdir, exclude=exclude)
 
     # Update package_dir if the package lies in a subdirectory
     if srcdir != '.':
         package_dir[''] = srcdir
 
     # For each of the setup_package.py modules, extract any
     # information that is needed to install them.  The build options
@@ -386,21 +439,14 @@
             options = setuppkg.get_build_options()
             for option in options:
                 add_command_option('build', *option)
         if hasattr(setuppkg, 'get_external_libraries'):
             libraries = setuppkg.get_external_libraries()
             for library in libraries:
                 add_external_library(library)
-        if hasattr(setuppkg, 'requires_2to3'):
-            requires_2to3 = setuppkg.requires_2to3()
-        else:
-            requires_2to3 = True
-        if not requires_2to3:
-            skip_2to3.append(
-                os.path.dirname(setuppkg.__file__))
 
     for setuppkg in iter_setup_packages(srcdir, packages):
         # get_extensions must include any Cython extensions by their .pyx
         # filename.
         if hasattr(setuppkg, 'get_extensions'):
             ext_modules.extend(setuppkg.get_extensions())
         if hasattr(setuppkg, 'get_package_data'):
@@ -426,15 +472,14 @@
             ext.extra_link_args.append('/MANIFEST')
 
     return {
         'ext_modules': ext_modules,
         'packages': packages,
         'package_dir': package_dir,
         'package_data': package_data,
-        'skip_2to3': skip_2to3
         }
 
 
 def iter_setup_packages(srcdir, packages):
     """ A generator that finds and imports all of the ``setup_package.py``
     modules in the source packages.
 
@@ -678,37 +723,34 @@
 def find_packages(where='.', exclude=(), invalidate_cache=False):
     """
     This version of ``find_packages`` caches previous results to speed up
     subsequent calls.  Use ``invalide_cache=True`` to ignore cached results
     from previous ``find_packages`` calls, and repeat the package search.
     """
 
+    if exclude:
+        warnings.warn(
+            "Use of the exclude parameter is no longer supported since it does "
+            "not work as expected. Use add_exclude_packages instead. Note that "
+            "it must be called prior to any other calls from setup helpers.",
+            AstropyDeprecationWarning)
+
+    # Calling add_exclude_packages after this point will have no effect
+    _module_state['excludes_too_late'] = True
+
     if not invalidate_cache and _module_state['package_cache'] is not None:
         return _module_state['package_cache']
 
-    packages = _find_packages(where=where, exclude=exclude)
+    packages = _find_packages(
+        where=where, exclude=list(_module_state['exclude_packages']))
     _module_state['package_cache'] = packages
 
     return packages
 
 
-def filter_packages(packagenames):
-    """
-    Removes some packages from the package list that shouldn't be
-    installed on the current version of Python.
-    """
-
-    if PY3:
-        exclude = '_py2'
-    else:
-        exclude = '_py3'
-
-    return [x for x in packagenames if not x.endswith(exclude)]
-
-
 class FakeBuildSphinx(Command):
     """
     A dummy build_sphinx command that is called if Sphinx is not
     installed and displays a relevant error message
     """
 
     # user options inherited from sphinx.setup_command.BuildDoc
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/version.py` & `speclite-0.9/astropy_helpers/astropy_helpers/version.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers/version_helpers.py` & `speclite-0.9/astropy_helpers/astropy_helpers/version_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,31 +14,32 @@
 
 or::
 
     from astropy import __version__
 
 """
 
-from __future__ import division
-
 import datetime
-import imp
 import os
 import pkgutil
 import sys
+import time
+import warnings
 
 from distutils import log
+from configparser import ConfigParser
 
 import pkg_resources
 
 from . import git_helpers
 from .distutils_helpers import is_distutils_display_option
-from .utils import invalidate_caches
+from .git_helpers import get_git_devstr
+from .utils import AstropyDeprecationWarning, import_file
 
-PY3 = sys.version_info[0] == 3
+__all__ = ['generate_version_py']
 
 
 def _version_split(version):
     """
     Split a version string into major, minor, and bugfix numbers.  If any of
     those numbers are missing the default is zero.  Any pre/post release
     modifiers are ignored.
@@ -82,43 +83,37 @@
     return tuple(parts[:3])
 
 
 # This is used by setup.py to create a new version.py - see that file for
 # details. Note that the imports have to be absolute, since this is also used
 # by affiliated packages.
 _FROZEN_VERSION_PY_TEMPLATE = """
-# Autogenerated by {packagetitle}'s setup.py on {timestamp!s}
-from __future__ import unicode_literals
+# Autogenerated by {packagetitle}'s setup.py on {timestamp!s} UTC
 import datetime
 
 {header}
 
 major = {major}
 minor = {minor}
 bugfix = {bugfix}
 
+version_info = (major, minor, bugfix)
+
 release = {rel}
 timestamp = {timestamp!r}
 debug = {debug}
 
-try:
-    from ._compiler import compiler
-except ImportError:
-    compiler = "unknown"
-
-try:
-    from .cython_version import cython_version
-except ImportError:
-    cython_version = "unknown"
+astropy_helpers_version = "{ahver}"
 """[1:]
 
 
 _FROZEN_VERSION_PY_WITH_GIT_HEADER = """
 {git_helpers}
 
+
 _packagename = "{packagename}"
 _last_generated_version = "{verstr}"
 _last_githash = "{githash}"
 
 # Determine where the source code for this module
 # lives.  If __file__ is not a filesystem path then
 # it is assumed not to live in a git repo at all.
@@ -138,15 +133,21 @@
 version = "{verstr}"
 githash = "{githash}"
 """[1:]
 
 
 def _get_version_py_str(packagename, version, githash, release, debug,
                         uses_git=True):
-    timestamp = datetime.datetime.now()
+    try:
+        from astropy_helpers import __version__ as ahver
+    except ImportError:
+        ahver = "unknown"
+
+    epoch = int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
+    timestamp = datetime.datetime.utcfromtimestamp(epoch)
     major, minor, bugfix = _version_split(version)
 
     if packagename.lower() == 'astropy':
         packagetitle = 'Astropy'
     else:
         packagetitle = 'Astropy-affiliated package ' + packagename
 
@@ -167,14 +168,15 @@
 
     return _FROZEN_VERSION_PY_TEMPLATE.format(packagetitle=packagetitle,
                                               timestamp=timestamp,
                                               header=header,
                                               major=major,
                                               minor=minor,
                                               bugfix=bugfix,
+                                              ahver=ahver,
                                               rel=release, debug=debug)
 
 
 def _generate_git_header(packagename, version, githash):
     """
     Generates a header to the version.py module that includes utilities for
     probing the git repository for updates (to the current git hash, etc.)
@@ -194,36 +196,106 @@
 
     idx = 0
     for idx, line in enumerate(source_lines):
         if line.startswith('# BEGIN'):
             break
     git_helpers_py = '\n'.join(source_lines[idx + 1:])
 
-    if PY3:
-        verstr = version
-    else:
-        # In Python 2 don't pass in a unicode string; otherwise verstr will
-        # be represented with u'' syntax which breaks on Python 3.x with x
-        # < 3.  This is only an issue when developing on multiple Python
-        # versions at once
-        verstr = version.encode('utf8')
+    verstr = version
 
     new_githash = git_helpers.get_git_devstr(sha=True, show_warning=False)
 
     if new_githash:
         githash = new_githash
 
     return _FROZEN_VERSION_PY_WITH_GIT_HEADER.format(
                 git_helpers=git_helpers_py, packagename=packagename,
                 verstr=verstr, githash=githash)
 
 
-def generate_version_py(packagename, version, release=None, debug=None,
-                        uses_git=True, srcdir='.'):
-    """Regenerate the version.py module if necessary."""
+def generate_version_py(packagename=None, version=None, release=None, debug=None,
+                        uses_git=None, srcdir='.'):
+    """
+    Generate a version.py file in the package with version information, and
+    update developer version strings.
+
+    This function should normally be called without any arguments. In this case
+    the package name and version is read in from the ``setup.cfg`` file (from
+    the ``name`` or ``package_name`` entry and the ``version`` entry in the
+    ``[metadata]`` section).
+
+    If the version is a developer version (of the form ``3.2.dev``), the
+    version string will automatically be expanded to include a sequential
+    number as a suffix (e.g. ``3.2.dev13312``), and the updated version string
+    will be returned by this function.
+
+    Based on this updated version string, a ``version.py`` file will be
+    generated inside the package, containing the version string as well as more
+    detailed information (for example the major, minor, and bugfix version
+    numbers, a ``release`` flag indicating whether the current version is a
+    stable or developer version, and so on.
+    """
+
+    if packagename is not None:
+        warnings.warn('The packagename argument to generate_version_py has '
+                      'been deprecated and will be removed in future. Specify '
+                      'the package name in setup.cfg instead', AstropyDeprecationWarning)
+
+    if version is not None:
+        warnings.warn('The version argument to generate_version_py has '
+                      'been deprecated and will be removed in future. Specify '
+                      'the version number in setup.cfg instead', AstropyDeprecationWarning)
+
+    if release is not None:
+        warnings.warn('The release argument to generate_version_py has '
+                      'been deprecated and will be removed in future. We now '
+                      'use the presence of the "dev" string in the version to '
+                      'determine whether this is a release', AstropyDeprecationWarning)
+
+    # We use ConfigParser instead of read_configuration here because the latter
+    # only reads in keys recognized by setuptools, but we need to access
+    # package_name below.
+    conf = ConfigParser()
+    conf.read('setup.cfg')
+
+    if conf.has_option('metadata', 'name'):
+        packagename = conf.get('metadata', 'name')
+    elif conf.has_option('metadata', 'package_name'):
+        # The package-template used package_name instead of name for a while
+        warnings.warn('Specifying the package name using the "package_name" '
+                      'option in setup.cfg is deprecated - use the "name" '
+                      'option instead.', AstropyDeprecationWarning)
+        packagename = conf.get('metadata', 'package_name')
+    elif packagename is not None:  # deprecated
+        pass
+    else:
+        sys.stderr.write('ERROR: Could not read package name from setup.cfg\n')
+        sys.exit(1)
+
+    if conf.has_option('metadata', 'version'):
+        version = conf.get('metadata', 'version')
+        add_git_devstr = True
+    elif version is not None:  # deprecated
+        add_git_devstr = False
+    else:
+        sys.stderr.write('ERROR: Could not read package version from setup.cfg\n')
+        sys.exit(1)
+
+    if release is None:
+        release = 'dev' not in version
+
+    if not release and add_git_devstr:
+        version += get_git_devstr(False)
+
+    if uses_git is None:
+        uses_git = not release
+
+    # In some cases, packages have a - but this is a _ in the module. Since we
+    # are only interested in the module here, we replace - by _
+    packagename = packagename.replace('-', '_')
 
     try:
         version_module = get_pkg_version_module(packagename)
 
         try:
             last_generated_version = version_module._last_generated_version
         except AttributeError:
@@ -247,15 +319,16 @@
         # Keep whatever the current value is, if it exists
         release = bool(current_release)
 
     if debug is None:
         # Likewise, keep whatever the current value is, if it exists
         debug = bool(current_debug)
 
-    version_py = os.path.join(srcdir, packagename, 'version.py')
+    package_srcdir = os.path.join(srcdir, *packagename.split('.'))
+    version_py = os.path.join(package_srcdir, 'version.py')
 
     if (last_generated_version != version or current_release != release or
             current_debug != debug):
         if '-q' not in sys.argv and '--quiet' not in sys.argv:
             log.set_threshold(log.INFO)
 
         if is_distutils_display_option():
@@ -266,33 +339,26 @@
         log.info('Freezing version number to {0}'.format(version_py))
 
         with open(version_py, 'w') as f:
             # This overwrites the actual version.py
             f.write(_get_version_py_str(packagename, version, last_githash,
                                         release, debug, uses_git=uses_git))
 
-        invalidate_caches()
-
-        if version_module:
-            imp.reload(version_module)
+    return version
 
 
 def get_pkg_version_module(packagename, fromlist=None):
     """Returns the package's .version module generated by
     `astropy_helpers.version_helpers.generate_version_py`.  Raises an
     ImportError if the version module is not found.
 
     If ``fromlist`` is an iterable, return a tuple of the members of the
     version module corresponding to the member names given in ``fromlist``.
     Raises an `AttributeError` if any of these module members are not found.
     """
 
-    if not fromlist:
-        # Due to a historical quirk of Python's import implementation,
-        # __import__ will not return submodules of a package if 'fromlist' is
-        # empty.
-        # TODO: For Python 3.1 and up it may be preferable to use importlib
-        # instead of the __import__ builtin
-        return __import__(packagename + '.version', fromlist=[''])
+    version = import_file(os.path.join(packagename, 'version.py'), name='version')
+
+    if fromlist:
+        return tuple(getattr(version, member) for member in fromlist)
     else:
-        mod = __import__(packagename + '.version', fromlist=fromlist)
-        return tuple(getattr(mod, member) for member in fromlist)
+        return version
```

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers.egg-info/PKG-INFO` & `speclite-0.9/astropy_helpers/astropy_helpers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `speclite-0.8/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt` & `speclite-0.9/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `speclite-0.8/astropy_helpers/CHANGES.rst` & `speclite-0.9/astropy_helpers/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,263 @@
 astropy-helpers Changelog
 *************************
 
+4.0.1 (2019-12-16)
+------------------
+
+- Fix pip installation. [#506]
+
+
+4.0 (2019-12-13)
+----------------
+
+- Changed minimum required Python version to 3.6. [#498]
+
+- Changed minimum required Sphinx version to 1.7. [#498]
+
+- Added a --parallel option for build_docs. [#498]
+
+- Fix compatibility with setuptools 42.x. [#504]
+
+
+3.2.2 (2019-10-25)
+------------------
+
+- Correctly handle main package directory inside namespace package. [#486]
+
+
+3.2.1 (2019-06-13)
+------------------
+
+- Reverting issuing deprecation warning for the ``build_sphinx`` command. [#482]
+
+- Make sure that all data files get included in tar file releases. [#485]
+
+
+3.2 (2019-05-29)
+----------------
+
+- Make sure that ``[options.package_data]`` in setup.cfg is taken into account
+  when collecting package data. [#453]
+
+- Simplified the code for the custom build_ext command. [#446]
+
+- Avoid importing the astropy package when trying to get the test command
+  when testing astropy itself. [#450]
+
+- Avoid importing whole package when trying to get version information. Note
+  that this has also introduced a small API change - ``cython_version`` and
+  ``compiler`` can no longer be imported from the ``package.version`` module
+  generated by astropy-helpers. Instead, you can import these from
+  ``package.cython_version`` and ``package.compiler_version`` respectively. [#442]
+
+- Make it possible to call ``generate_version_py`` and ``register_commands``
+  without any arguments, which causes information to be read in from the
+  ``setup.cfg`` file. [#440]
+
+- Simplified setup.py and moved most of the configuration to setup.cfg. [#445]
+
+- Add a new ``astropy_helpers.setup_helpers.setup`` function that does all
+  the default boilerplate in typical ``setup.py`` files that use
+  astropy-helpers. [#443]
+
+- Remove ``deprecated``, ``deprecated_attribute``, and ``minversion`` from
+  ``astropy_helpers.utils``. [#447]
+
+- Updated minimum required version of setuptools to 30.3.0. [#440]
+
+- Remove functionality to adjust compilers if a broken compiler is detected.
+  This is not useful anymore as only a single compiler was previously patched
+  (now unlikely to be used) and this was only to fix a compilation issue in the
+  core astropy package. [#421]
+
+- ``sphinx-astropy`` is now a required dependency to build the docs, the
+  machinery to install it as eggs have been removed. [#474]
+
+
+3.1.1 (2019-02-22)
+------------------
+
+- Moved documentation from README to Sphinx. [#444]
+
+- Fixed broken OpenMP detection when building with ``-coverage``. [#434]
+
+
+3.1 (2018-12-04)
+----------------
+
+- Added extensive documentation about astropy-helpers to the README.rst file. [#416]
+
+- Fixed the compatibility of the build_docs command with Sphinx 1.8 and above. [#413]
+
+- Removing deprecated test_helpers.py file. [#369]
+
+- Removing ez_setup.py file and requiring setuptools 1.0 or later. [#384]
+
+- Remove all sphinx components from ``astropy-helpers``. These are now replaced
+  by the ``sphinx-astropy`` package in conjunction with the ``astropy-theme-sphinx``,
+  ``sphinx-automodapi``, and ``numpydoc`` packages. [#368]
+
+- openmp_helpers.py: Make add_openmp_flags_if_available() work for clang.
+  The necessary include, library, and runtime paths now get added to the C test code
+  used to determine if openmp works.
+  Autogenerator utility added ``openmp_enabled.is_openmp_enabled()``
+  which can be called post build to determine state of OpenMP support.
+  [#382]
+
+- Add version_info tuple to autogenerated version.py. Allows for simple
+  version checking, i.e. version_info > (2,0,1). [#385]
+
+
+3.0.2 (2018-06-01)
+------------------
+
+- Nothing changed.
+
+
+3.0.1 (2018-02-22)
+------------------
+
+- Nothing changed.
+
+
+3.0 (2018-02-09)
+----------------
+
+- Removing Python 2 support, including 2to3. Packages wishing to keep Python
+  2 support should NOT update to this version. [#340]
+
+- Removing deprecated _test_compat making astropy a hard dependency for
+  packages wishing to use the astropy tests machinery. [#314]
+
+- Removing unused 'register' command since packages should be uploaded
+  with twine and get registered automatically. [#332]
+
+
+2.0.11 (2019-10-25)
+-------------------
+
+- Fixed deprecation warning in sphinx theme. [#493]
+
+- Fixed an issue that caused pytest to crash if it tried to collect
+  tests. [#488]
+
+
+2.0.10 (2019-05-29)
+-------------------
+
+- Removed ``tocdepthfix`` sphinx extension that worked around a big in
+  Sphinx that has been long fixed. [#475]
+
+- Allow Python dev versions to pass the python version check. [#476]
+
+- Updated bundled version of sphinx-automodapi to v0.11. [#478]
+
+
+2.0.9 (2019-02-22)
+------------------
+
+- Updated bundled version of sphinx-automodapi to v0.10. [#439]
+
+- Updated bundled sphinx extensions version to sphinx-astropy v1.1.1. [#454]
+
+- Include package name in error message for Python version in
+  ``ah_bootstrap.py``. [#441]
+
+
+2.0.8 (2018-12-04)
+------------------
+
+- Fixed compatibility with Sphinx 1.8+. [#428]
+
+- Fixed error that occurs when installing a package in an environment where
+  ``numpy`` is not already installed. [#404]
+
+- Updated bundled version of sphinx-automodapi to v0.9. [#422]
+
+- Updated bundled version of numpydoc to v0.8.0. [#423]
+
+
+2.0.7 (2018-06-01)
+------------------
+
+- Removing ez_setup.py file and requiring setuptools 1.0 or later. [#384]
+
+
+2.0.6 (2018-02-24)
+------------------
+
+- Avoid deprecation warning due to ``exclude=`` keyword in ``setup.py``. [#379]
+
+
+2.0.5 (2018-02-22)
+------------------
+
+- Fix segmentation faults that occurred when the astropy-helpers submodule
+  was first initialized in packages that also contained Cython code. [#375]
+
+
+2.0.4 (2018-02-09)
+------------------
+
+- Support dotted package names as namespace packages in generate_version_py.
+  [#370]
+
+- Fix compatibility with setuptools 36.x and above. [#372]
+
+- Fix false negative in add_openmp_flags_if_available when measuring code
+  coverage with gcc. [#374]
+
+
+2.0.3 (2018-01-20)
+------------------
+
+- Make sure that astropy-helpers 3.x.x is not downloaded on Python 2. [#362, #363]
+
+- The bundled version of sphinx-automodapi has been updated to v0.7. [#365]
+
+- Add --auto-use and --no-auto-use command-line flags to match the
+  ``auto_use`` configuration option, and add an alias
+  ``--use-system-astropy-helpers`` for ``--no-auto-use``. [#366]
+
+
+2.0.2 (2017-10-13)
+------------------
+
+- Added new helper function add_openmp_flags_if_available that can add
+  OpenMP compilation flags to a C/Cython extension if needed. [#346]
+
+- Update numpydoc to v0.7. [#343]
+
+- The function ``get_git_devstr`` now returns ``'0'`` instead of ``None`` when
+  no git repository is present. This allows generation of development version
+  strings that are in a format that ``setuptools`` expects (e.g. "1.1.3.dev0"
+  instead of "1.1.3.dev"). [#330]
+
+- It is now possible to override generated timestamps to make builds
+  reproducible by setting the ``SOURCE_DATE_EPOCH`` environment variable [#341]
+
+- Mark Sphinx extensions as parallel-safe. [#344]
+
+- Switch to using mathjax instead of imgmath for local builds. [#342]
+
+- Deprecate ``exclude`` parameter of various functions in setup_helpers since
+  it could not work as intended. Add new function ``add_exclude_packages`` to
+  provide intended behavior. [#331]
+
+- Allow custom Sphinx doctest extension to recognize and process standard
+  doctest directives ``testsetup`` and ``doctest``. [#335]
+
+
 2.0.1 (2017-07-28)
 ------------------
 
 - Fix compatibility with Sphinx <1.5. [#326]
 
+
 2.0 (2017-07-06)
 ----------------
 
 - Add support for package that lies in a subdirectory. [#249]
 
 - Removing ``compat.subprocess``. [#298]
```

### Comparing `speclite-0.8/astropy_helpers/LICENSE.rst` & `speclite-0.9/astropy_helpers/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `speclite-0.8/CHANGES.rst` & `speclite-0.9/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.9 (unreleased)
+----------------
+
+- No changes yet.
+
 0.8 (2018-09-11)
 ----------------
 
 - Add MzLS-z, BASS-g, BASS-r filters used by DESI imaging surveys.
 - Update astropy-helpers to v2.0.6.
 
 0.7 (2017-10-03)
```

### Comparing `speclite-0.8/docs/_static/bessell.png` & `speclite-0.9/docs/_static/bessell.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/custom.png` & `speclite-0.9/docs/_static/custom.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/decam2014.png` & `speclite-0.9/docs/_static/decam2014.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/desi_imaging.png` & `speclite-0.9/docs/_static/desi_imaging.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/hsc2017.png` & `speclite-0.9/docs/_static/hsc2017.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/lsst2016.png` & `speclite-0.9/docs/_static/lsst2016.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/sampling.png` & `speclite-0.9/docs/_static/sampling.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/sdss2010.png` & `speclite-0.9/docs/_static/sdss2010.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/_static/wise2010.png` & `speclite-0.9/docs/_static/wise2010.png`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/conf.py` & `speclite-0.9/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # Building from inside the docs/ directory?
     if os.path.basename(os.getcwd()) == 'docs':
         a_h_path = os.path.abspath(os.path.join('..', 'astropy_helpers'))
         if os.path.isdir(a_h_path):
             sys.path.insert(1, a_h_path)
 
 # Load all of the global Astropy configuration
-from astropy_helpers.sphinx.conf import *
+from sphinx_astropy.conf import *
 
 # Get configuration information from setup.cfg
 try:
     from ConfigParser import ConfigParser
 except ImportError:
     from configparser import ConfigParser
 conf = ConfigParser()
@@ -71,25 +71,25 @@
 # be used globally.
 rst_epilog += """
 """
 
 # -- Project information ------------------------------------------------------
 
 # This does not *have* to match the package name, but typically does
-project = setup_cfg['package_name']
+project = setup_cfg['name']
 author = setup_cfg['author']
 copyright = '{0}, {1}'.format(
     datetime.datetime.now().year, setup_cfg['author'])
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
-__import__(setup_cfg['package_name'])
-package = sys.modules[setup_cfg['package_name']]
+__import__(setup_cfg['name'])
+package = sys.modules[setup_cfg['name']]
 
 # The short X.Y version.
 version = package.__version__.split('-', 1)[0]
 # The full version, including alpha/beta/rc tags.
 release = package.__version__
 
 
@@ -158,17 +158,17 @@
 man_pages = [('index', project.lower(), project + u' Documentation',
               [author], 1)]
 
 
 # -- Options for the edit_on_github extension ---------------------------------
 
 if eval(setup_cfg.get('edit_on_github')):
-    extensions += ['astropy_helpers.sphinx.ext.edit_on_github']
+    extensions += ['sphinx_astropy.ext.edit_on_github']
 
-    versionmod = __import__(setup_cfg['package_name'] + '.version')
+    versionmod = __import__(setup_cfg['name'] + '.version')
     edit_on_github_project = setup_cfg['github_project']
     if versionmod.version.release:
         edit_on_github_branch = "v" + versionmod.version.version
     else:
         edit_on_github_branch = "master"
 
     edit_on_github_source_root = ""
```

### Comparing `speclite-0.8/docs/filters.rst` & `speclite-0.9/docs/filters.rst`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,30 @@
 
     desi_imaging = speclite.filters.load_filters('BASS-g', 'BASS-r', 'MzLS-z')
     speclite.filters.plot_filters(desi_imaging)
 
 .. image:: _static/desi_imaging.png
     :alt: DESI imaging filter curves
 
+.. _euclid-filters:
+
+Euclid Filters
+--------------
+
+The current best end-of-life estimates for the "VIS", "Y", "H", and "J" total throughputs for Euclid,
+i.e., "Y", "H", and "J" have been convolved by the "NISP" throughput. The original tables can be found
+[here](http://euclid.esac.esa.int/epdb/db/SC456Draft/). The group name ``Euclid`` is used
+to identify these curves in ``speclite``.
+The command below produces the figure::
+
+    euclid = speclite.filters.load_filters('Euclid-VIS', 'Euclid-Y', 'Euclid-H', 'Euclid-J')
+    speclite.filters.plot_filters(euclid)
+
+.. image:: _static/euclid.png
+    :alt: Euclid filter curves
 .. _custom-filters:
 
 Custom Filters
 --------------
 
 In addition to the standard filters included with the ``speclite`` code
 distribution, you can create and read your own custom filters.  For example
```

### Comparing `speclite-0.8/docs/make.bat` & `speclite-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/Makefile` & `speclite-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `speclite-0.8/docs/overview.rst` & `speclite-0.9/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `speclite-0.8/licenses/LICENSE.rst` & `speclite-0.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `speclite-0.8/README.rst` & `speclite-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `speclite-0.8/setup.cfg` & `speclite-0.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 # E901 - SyntaxError or IndentationError
 # E902 - IOError
 select = E101,W191,W291,W292,W293,W391,E111,E112,E113,E901,E902
 exclude = extern,sphinx,*parsetab.py
 
 [metadata]
 package_name = speclite
+name = speclite
 description = Lightweight utilities for working with spectroscopic data
 long_description = This package provides a set of lightweight utilities for working with spectroscopic data in astronomy. Based on the astropy affiliated package template.
 author = Speclite Developers
 author_email = dkirkby@uci.edu
 license = BSD
 url = http://speclite.readthedocs.io/
 edit_on_github = True
 github_project = dkirkby/speclite
 install_requires = astropy scipy pyyaml
 # version should be PEP440 compatible, e.g. 0.8 or 0.8dev (http://www.python.org/dev/peps/pep-0440)
-version = 0.8
+version = 0.9
 
 [entry_points]
 speclite_benchmark = speclite.benchmark:main
```

### Comparing `speclite-0.8/setup.py` & `speclite-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,15 @@
 
 # Populate the dict of setup command overrides; this should be done before
 # invoking any other functionality from distutils since it can potentially
 # modify distutils' behavior.
 cmdclassd = register_commands(PACKAGENAME, VERSION, RELEASE)
 
 # Freeze build information in version.py
-generate_version_py(PACKAGENAME, VERSION, RELEASE,
-                    get_debug_option(PACKAGENAME))
+generate_version_py()
 
 # Treat everything in scripts except README* as a script to be installed
 scripts = [fname for fname in glob.glob(os.path.join('scripts', '*'))
            if not os.path.basename(fname).startswith('README')]
 
 
 # Get configuration information from all of the various subpackages.
```

### Comparing `speclite-0.8/speclite/__init__.py` & `speclite-0.9/speclite/__init__.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/_astropy_init.py` & `speclite-0.9/speclite/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/accumulate.py` & `speclite-0.9/speclite/accumulate.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/benchmark.py` & `speclite-0.9/speclite/benchmark.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/conftest.py` & `speclite-0.9/speclite/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # this contains imports plugins that configure py.test for astropy tests.
 # by importing them here in conftest.py they are discoverable by py.test
 # no matter how it is invoked within the source tree.
 
-from astropy.tests.pytest_plugins import *
+from astropy.version import version as astropy_version
+if astropy_version < '3.0':
+    # With older versions of Astropy, we actually need to import the pytest
+    # plugins themselves in order to make them discoverable by pytest.
+    from astropy.tests.pytest_plugins import *
+else:
+    # As of Astropy 3.0, the pytest plugins provided by Astropy are
+    # automatically made available when Astropy is installed. This means it's
+    # not necessary to import them here, but we still need to import global
+    # variables that are used for configuration.
+    from astropy.tests.plugins.display import PYTEST_HEADER_MODULES, TESTED_VERSIONS
+
+from astropy.tests.helper import enable_deprecations_as_exceptions
 
 ## Uncomment the following line to treat all DeprecationWarnings as
 ## exceptions
 # enable_deprecations_as_exceptions()
 
 ## Uncomment and customize the following lines to add/remove entries from
 ## the list of packages for which version numbers are displayed when running
```

### Comparing `speclite-0.8/speclite/data/filters/BASS-g.ecsv` & `speclite-0.9/speclite/data/filters/BASS-g.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/BASS-r.ecsv` & `speclite-0.9/speclite/data/filters/BASS-r.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/bessell-B.ecsv` & `speclite-0.9/speclite/data/filters/bessell-B.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/bessell-I.ecsv` & `speclite-0.9/speclite/data/filters/bessell-I.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/bessell-R.ecsv` & `speclite-0.9/speclite/data/filters/bessell-R.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/bessell-U.ecsv` & `speclite-0.9/speclite/data/filters/bessell-U.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/bessell-V.ecsv` & `speclite-0.9/speclite/data/filters/bessell-V.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-g.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-g.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-i.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-i.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-r.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-r.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-u.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-u.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-Y.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-Y.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/decam2014-z.ecsv` & `speclite-0.9/speclite/data/filters/decam2014-z.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/hsc2017-g.ecsv` & `speclite-0.9/speclite/data/filters/hsc2017-g.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/hsc2017-i.ecsv` & `speclite-0.9/speclite/data/filters/hsc2017-i.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/hsc2017-r.ecsv` & `speclite-0.9/speclite/data/filters/hsc2017-r.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/hsc2017-y.ecsv` & `speclite-0.9/speclite/data/filters/hsc2017-y.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/hsc2017-z.ecsv` & `speclite-0.9/speclite/data/filters/hsc2017-z.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-g.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-g.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-i.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-i.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-r.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-r.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-u.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-u.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-y.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-y.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/lsst2016-z.ecsv` & `speclite-0.9/speclite/data/filters/lsst2016-z.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/MzLS-z.ecsv` & `speclite-0.9/speclite/data/filters/MzLS-z.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/sdss2010-g.ecsv` & `speclite-0.9/speclite/data/filters/sdss2010-g.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/sdss2010-i.ecsv` & `speclite-0.9/speclite/data/filters/sdss2010-i.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/sdss2010-r.ecsv` & `speclite-0.9/speclite/data/filters/sdss2010-r.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/sdss2010-u.ecsv` & `speclite-0.9/speclite/data/filters/sdss2010-u.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/sdss2010-z.ecsv` & `speclite-0.9/speclite/data/filters/sdss2010-z.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/wise2010-W1.ecsv` & `speclite-0.9/speclite/data/filters/wise2010-W1.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/wise2010-W2.ecsv` & `speclite-0.9/speclite/data/filters/wise2010-W2.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/wise2010-W3.ecsv` & `speclite-0.9/speclite/data/filters/wise2010-W3.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/data/filters/wise2010-W4.ecsv` & `speclite-0.9/speclite/data/filters/wise2010-W4.ecsv`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/downsample.py` & `speclite-0.9/speclite/downsample.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/filters.py` & `speclite-0.9/speclite/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 See :doc:`/filters` for information about the standard filters included with
 this code distribution and instructions for adding your own filters. Filter
 names have two components, a group name and a band name, which are combined
 with a hyphen, e.g. "sdss2010-r".  The group names included with this package
 are:
 
     >>> filter_group_names
-    ['sdss2010', 'decam2014', 'wise2010', 'hsc2017', 'lsst2016', 'bessell', 'BASS', 'MzLS']
+    ['sdss2010', 'decam2014', 'wise2010', 'hsc2017', 'lsst2016', 'bessell', 'BASS', 'MzLS', 'Euclid']
 
 List the band names associated with any group using, for example:
 
     >>> load_filters('sdss2010-*').names
     ['sdss2010-u', 'sdss2010-g', 'sdss2010-r', 'sdss2010-i', 'sdss2010-z']
 
 Here is a brief example of calculating SDSS r,i and Bessell V magnitudes for a
@@ -222,15 +222,15 @@
     List of filter group names included with this package.
 default_wavelength_unit : :class:`astropy.units.Unit`
     The default wavelength units assumed when units are not specified.
     The same units are used to store wavelength values in internal arrays.
 default_flux_unit : :class:`astropy.units.Unit`
     The default units for spectral flux density per unit wavelength.
 """
-from __future__ import print_function, division
+from __future__ import print_function, division # pragma: no cover
 
 import os
 import os.path
 import glob
 import re
 import collections
 
@@ -242,15 +242,15 @@
 import astropy.table
 import astropy.units
 import astropy.utils.data
 
 
 filter_group_names = [
     'sdss2010', 'decam2014', 'wise2010', 'hsc2017', 'lsst2016', 'bessell',
-    'BASS', 'MzLS']
+    'BASS', 'MzLS', 'Euclid']
 
 default_wavelength_unit = astropy.units.Angstrom
 
 default_flux_unit = (astropy.units.erg / astropy.units.cm**2 /
                      astropy.units.s / default_wavelength_unit)
 
 # Constant spectral flux density per unit frequency for a zero magnitude
@@ -1301,15 +1301,15 @@
     quad_weight : :class:`astropy.units.Quantity` or None
         Array of weights corresponding to each ``quad_wavelength``.  Will be
         None if the parameter ``photon_weighted = False``.
     """
     def __init__(self, response, wavelength,
                  photon_weighted=True, interpolate=False, units=None):
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             self._response = load_filter(response)
         else:
             self._response = response
         self._wavelength = validate_wavelength_array(wavelength, min_length=2)
         self.num_wavelength = len(self._wavelength)
 
         # Check if extrapolation would be required.
@@ -1459,15 +1459,15 @@
         # the filter we are convolving with.
         if values_no_units.shape[axis] != self.num_wavelength:
             raise ValueError(
                 'Expected {0} values along axis {1}.'
                 .format(len(self._wavelength), axis))
         values_slice = [slice(None)] * len(values_no_units.shape)
         values_slice[axis] = self._response_slice
-        values_no_units = values_no_units[values_slice]
+        values_no_units = values_no_units[tuple(values_slice)]
 
         if plot:
             if len(values_no_units.shape) != 1:
                 raise ValueError(
                     'Cannot plot convolution of multidimensional values.')
             import matplotlib.pyplot as plt
             ##fig, left_axis = plt.subplots()
@@ -1513,15 +1513,15 @@
                 interpolated_values *
                 self.interpolate_response.reshape(response_shape))
             # Update the integrand with the interpolated values.
             integrand = np.concatenate(
                 (integrand, interpolated_integrand), axis=axis)
             # Resort by wavelength.
             values_slice[axis] = self.interpolate_sort_order
-            integrand = integrand[values_slice]
+            integrand = integrand[tuple(values_slice)]
 
         if plot:
             # Plot integrand before applying weights, so we can re-use
             # the right-hand axis scale.
             plt.fill_between(
                 self.quad_wavelength, integrand,
                 color='g', lw=0, alpha=0.25)
```

### Comparing `speclite-0.8/speclite/redshift.py` & `speclite-0.9/speclite/redshift.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/resample.py` & `speclite-0.9/speclite/resample.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 """Resample spectra using interpolation.
 """
 from __future__ import print_function, division
 
 import numpy as np
 import numpy.ma as ma
 import scipy.interpolate
+import pkg_resources as pkgr
 
+if pkgr.parse_version(np.__version__)  >= pkgr.parse_version('1.16'):
+    import numpy.lib.recfunctions as rfn
 
 def resample(data_in, x_in, x_out, y, data_out=None, kind='linear'):
     """Resample the data of one spectrum using interpolation.
 
     Dependent variables y1, y2, ... in the input data are resampled in the
     independent variable x using interpolation models y1(x), y2(x), ...
     evaluated on a new grid of x values. The independent variable will
@@ -161,18 +164,25 @@
     if ma.isMA(data_in):
         # Copy the structured 1D array into a 2D unstructured array
         # and set masked values to NaN.
         y_in = np.zeros(data_in.shape + y_shape, y_type)
         for i,y in enumerate(y_names):
             y_in[:,i] = data_in[y].filled(np.nan)
     else:
-        y_in = data_in[y_names]
-        # View the structured 1D array as a 2D unstructured array (without
-        # copying any memory).
-        y_in = y_in.view(y_type).reshape(data_in.shape + y_shape)
+        if pkgr.parse_version(np.__version__)  >= pkgr.parse_version('1.16'):
+            # The slicing does not work in numpy 1.16 and above
+            # we use structured_to_unstructured to get the slice that we care about
+            y_in = rfn.structured_to_unstructured(
+                       data_in[y_names]).reshape(data_in.shape + y_shape)
+        else:
+            y_in = data_in[y_names]
+            # View the structured 1D array as a 2D unstructured array (without
+            # copying any memory).
+            y_in = y_in.view(y_type).reshape(data_in.shape + y_shape)
+       
     # interp1d will only propagate NaNs correctly for certain values of `kind`.
     # With numpy = 1.6 or 1.7, only 'nearest' and 'linear' work.
     # With numpy = 1.8 or 1.9, 'slinear' and kind = 0 or 1 also work.
     if np.any(np.isnan(y_in)):
         if kind not in ('nearest', 'linear'):
             raise ValueError(
                 'Interpolation kind not supported for masked data: {0}.'
```

### Comparing `speclite-0.8/speclite/tests/coveragerc` & `speclite-0.9/speclite/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/tests/test_accumulate.py` & `speclite-0.9/speclite/tests/test_accumulate.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/tests/test_downsample.py` & `speclite-0.9/speclite/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/tests/test_filters.py` & `speclite-0.9/speclite/tests/test_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,21 @@
     eps = 1e-6
     wlen = [0.1 - eps, 0.3 + eps] * u.nm
     flux = [1., 1.] * default_flux_unit
     m1 = r.get_ab_maggies(flux, wlen)
     m2 = r.get_ab_maggies(flux, wlen)
     assert m1 == m2
 
+def test_wavelength_property():
+    # Check that the wavelength property is working
+    wlen = [1, 2, 3] * u.Angstrom
+    meta = dict(group_name='g', band_name='b')
+    r = FilterResponse(wlen, [0,1,0], meta)
+    assert np.allclose(r.wavelength, r._wavelength) 
+    assert np.allclose(r.wavelength, validate_wavelength_array(wlen))
 
 def test_mag_flux_units():
     # Check that non-default flux units are handled correctly.
     wlen = [1, 2, 3] * u.Angstrom
     meta = dict(group_name='g', band_name='b')
     r = FilterResponse(wlen, [0, 1, 0], meta)
```

### Comparing `speclite-0.8/speclite/tests/test_redshift.py` & `speclite-0.9/speclite/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `speclite-0.8/speclite/tests/test_resample.py` & `speclite-0.9/speclite/tests/test_resample.py`

 * *Files identical despite different names*

