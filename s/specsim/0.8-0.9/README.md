# Comparing `tmp/specsim-0.8.tar.gz` & `tmp/specsim-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/specsim-0.8.tar", last modified: Sat Mar 25 16:30:30 2017, max compression
+gzip compressed data, was "dist/specsim-0.9.tar", last modified: Thu May 11 20:40:26 2017, max compression
```

## Comparing `specsim-0.8.tar` & `specsim-0.9.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:30.000000 specsim-0.8/
--rw-r--r--   0 david      (501) staff       (20)    36162 2017-01-10 00:52:54.000000 specsim-0.8/ah_bootstrap.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/
--rw-r--r--   0 david      (501) staff       (20)    36162 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/
--rw-r--r--   0 david      (501) staff       (20)     1836 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 david      (501) staff       (20)        0 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2940 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 david      (501) staff       (20)    11701 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/_test_compat.py
--rw-r--r--   0 david      (501) staff       (20)    19503 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 david      (501) staff       (20)     1454 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/build_py.py
--rw-r--r--   0 david      (501) staff       (20)    10020 2017-03-20 19:28:52.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-r--r--   0 david      (501) staff       (20)      486 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/install.py
--rw-r--r--   0 david      (501) staff       (20)      512 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/install_lib.py
--rw-r--r--   0 david      (501) staff       (20)     2407 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/register.py
--rw-r--r--   0 david      (501) staff       (20)      120 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 david      (501) staff       (20)     3033 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 david      (501) staff       (20)     1356 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/commands/test.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/compat/
--rw-r--r--   0 david      (501) staff       (20)      368 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/compat/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/compat/_subprocess_py2/
--rw-r--r--   0 david      (501) staff       (20)     1306 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/compat/_subprocess_py2/__init__.py
--rw-r--r--   0 david      (501) staff       (20)      551 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/compat/subprocess.py
--rw-r--r--   0 david      (501) staff       (20)     7917 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/distutils_helpers.py
--rw-r--r--   0 david      (501) staff       (20)     6104 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 david      (501) staff       (20)    26333 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 david      (501) staff       (20)      268 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    12370 2017-03-20 19:28:52.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/conf.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/
--rw-r--r--   0 david      (501) staff       (20)       94 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     4527 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/astropyautosummary.py
--rw-r--r--   0 david      (501) staff       (20)     4802 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/autodoc_enhancements.py
--rw-r--r--   0 david      (501) staff       (20)    14495 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/automodapi.py
--rw-r--r--   0 david      (501) staff       (20)    25020 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/automodsumm.py
--rw-r--r--   0 david      (501) staff       (20)     2832 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
--rw-r--r--   0 david      (501) staff       (20)     5417 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/comment_eater.py
--rw-r--r--   0 david      (501) staff       (20)    24740 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/compiler_unparse.py
--rw-r--r--   0 david      (501) staff       (20)    18074 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/docscrape.py
--rw-r--r--   0 david      (501) staff       (20)     9527 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/docscrape_sphinx.py
--rw-r--r--   0 david      (501) staff       (20)     1310 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
--rw-r--r--   0 david      (501) staff       (20)     5898 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
--rw-r--r--   0 david      (501) staff       (20)     6693 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/numpydoc.py
--rw-r--r--   0 david      (501) staff       (20)     5854 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/phantom_import.py
--rw-r--r--   0 david      (501) staff       (20)     3712 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/smart_resolver.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/
--rw-r--r--   0 david      (501) staff       (20)      170 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/base.rst
--rw-r--r--   0 david      (501) staff       (20)     1161 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/class.rst
--rw-r--r--   0 david      (501) staff       (20)      703 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/module.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/
--rw-r--r--   0 david      (501) staff       (20)     1817 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1699 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_autodoc_enhancements.py
--rw-r--r--   0 david      (501) staff       (20)     7870 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodapi.py
--rw-r--r--   0 david      (501) staff       (20)     2434 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodsumm.py
--rw-r--r--   0 david      (501) staff       (20)    18153 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_docscrape.py
--rw-r--r--   0 david      (501) staff       (20)      996 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_utils.py
--rw-r--r--   0 david      (501) staff       (20)      677 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
--rw-r--r--   0 david      (501) staff       (20)     4310 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/traitsdoc.py
--rw-r--r--   0 david      (501) staff       (20)     6179 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/utils.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/
--rw-r--r--   0 david      (501) staff       (20)      562 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
--rw-r--r--   0 david      (501) staff       (20)     1638 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
--rw-r--r--   0 david      (501) staff       (20)      658 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
--rw-r--r--   0 david      (501) staff       (20)     2820 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
--rw-r--r--   0 david      (501) staff       (20)      325 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/setup_package.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
--rw-r--r--   0 david      (501) staff       (20)       73 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
--rw-r--r--   0 david      (501) staff       (20)     3433 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
--rw-r--r--   0 david      (501) staff       (20)       34 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
--rw-r--r--   0 david      (501) staff       (20)      272 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
--rw-r--r--   0 david      (501) staff       (20)     5201 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
--rw-r--r--   0 david      (501) staff       (20)     1725 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
--rw-r--r--   0 david      (501) staff       (20)    32988 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
--rw-r--r--   0 david      (501) staff       (20)     4634 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
--rw-r--r--   0 david      (501) staff       (20)     1884 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
--rw-r--r--   0 david      (501) staff       (20)    12067 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
--rw-r--r--   0 david      (501) staff       (20)     2769 2017-03-20 19:28:52.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
--rw-r--r--   0 david      (501) staff       (20)     4971 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
--rw-r--r--   0 david      (501) staff       (20)      192 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
--rw-r--r--   0 david      (501) staff       (20)      507 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/test_helpers.py
--rw-r--r--   0 david      (501) staff       (20)    27953 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 david      (501) staff       (20)      546 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 david      (501) staff       (20)     9639 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 david      (501) staff       (20)        1 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 david      (501) staff       (20)     2970 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     3366 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)       16 2015-09-06 17:00:35.000000 specsim-0.8/astropy_helpers/astropy_helpers.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)    14120 2017-03-20 19:28:52.000000 specsim-0.8/astropy_helpers/CHANGES.rst
--rw-r--r--   0 david      (501) staff       (20)    12746 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/ez_setup.py
--rw-r--r--   0 david      (501) staff       (20)     1491 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/LICENSE.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/astropy_helpers/licenses/
--rw-r--r--   0 david      (501) staff       (20)     2505 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
--rw-r--r--   0 david      (501) staff       (20)     5959 2015-09-06 17:00:34.000000 specsim-0.8/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
--rw-r--r--   0 david      (501) staff       (20)     1833 2017-01-10 00:52:12.000000 specsim-0.8/astropy_helpers/README.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/cextern/
--rw-r--r--   0 david      (501) staff       (20)      298 2015-09-06 01:24:09.000000 specsim-0.8/cextern/README.rst
--rw-r--r--   0 david      (501) staff       (20)     3420 2017-03-25 16:29:55.000000 specsim-0.8/CHANGES.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/docs/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/docs/_static/
--rw-r--r--   0 david      (501) staff       (20)   205443 2016-03-09 04:07:13.000000 specsim-0.8/docs/_static/desi_ab22.png
--rw-r--r--   0 david      (501) staff       (20)    85717 2016-02-24 18:21:04.000000 specsim-0.8/docs/_static/desi_atmosphere.png
--rw-r--r--   0 david      (501) staff       (20)    82453 2016-02-24 18:21:04.000000 specsim-0.8/docs/_static/desi_bright_atmosphere.png
--rw-r--r--   0 david      (501) staff       (20)    76022 2016-02-20 01:15:47.000000 specsim-0.8/docs/_static/desi_instrument.png
--rw-r--r--   0 david      (501) staff       (20)    78276 2016-02-24 18:21:04.000000 specsim-0.8/docs/_static/desi_scattered_moon.png
--rw-r--r--   0 david      (501) staff       (20)    44134 2016-02-20 01:15:47.000000 specsim-0.8/docs/_static/overview.pdf
--rw-r--r--   0 david      (501) staff       (20)    80680 2016-02-20 01:15:47.000000 specsim-0.8/docs/_static/overview.png
--rw-r--r--   0 david      (501) staff       (20)    25195 2016-02-24 18:21:04.000000 specsim-0.8/docs/_static/test_atmosphere.png
--rw-r--r--   0 david      (501) staff       (20)    52855 2016-02-20 01:15:47.000000 specsim-0.8/docs/_static/test_instrument.png
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/docs/_templates/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/docs/_templates/autosummary/
--rw-r--r--   0 david      (501) staff       (20)      250 2015-09-06 01:24:09.000000 specsim-0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 david      (501) staff       (20)      251 2015-09-06 01:24:09.000000 specsim-0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 david      (501) staff       (20)      252 2015-09-06 01:24:09.000000 specsim-0.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 david      (501) staff       (20)     2036 2017-03-14 21:48:08.000000 specsim-0.8/docs/api.rst
--rw-r--r--   0 david      (501) staff       (20)     2814 2017-03-14 21:48:08.000000 specsim-0.8/docs/cmdline.rst
--rw-r--r--   0 david      (501) staff       (20)     6497 2017-03-25 16:25:43.000000 specsim-0.8/docs/conf.py
--rw-r--r--   0 david      (501) staff       (20)    10735 2016-08-28 17:05:39.000000 specsim-0.8/docs/config.rst
--rw-r--r--   0 david      (501) staff       (20)     4597 2017-03-17 17:10:35.000000 specsim-0.8/docs/fiberloss.rst
--rw-r--r--   0 david      (501) staff       (20)     7564 2017-03-25 14:58:54.000000 specsim-0.8/docs/guide.rst
--rw-r--r--   0 david      (501) staff       (20)     1611 2016-02-24 18:21:04.000000 specsim-0.8/docs/history.rst
--rw-r--r--   0 david      (501) staff       (20)      467 2017-03-25 14:58:54.000000 specsim-0.8/docs/index.rst
--rw-r--r--   0 david      (501) staff       (20)     2945 2017-03-25 14:58:54.000000 specsim-0.8/docs/install.rst
--rw-r--r--   0 david      (501) staff       (20)     4513 2015-09-06 01:24:09.000000 specsim-0.8/docs/make.bat
--rw-r--r--   0 david      (501) staff       (20)     4581 2016-08-23 23:10:48.000000 specsim-0.8/docs/Makefile
--rw-r--r--   0 david      (501) staff       (20)     6476 2017-03-25 14:58:54.000000 specsim-0.8/docs/output.rst
--rw-r--r--   0 david      (501) staff       (20)       48 2015-09-07 18:12:51.000000 specsim-0.8/docs/rtd-pip-requirements
--rw-r--r--   0 david      (501) staff       (20)    12385 2016-08-23 23:10:48.000000 specsim-0.8/ez_setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/licenses/
--rw-r--r--   0 david      (501) staff       (20)     1508 2015-11-03 13:28:41.000000 specsim-0.8/licenses/LICENSE.rst
--rw-r--r--   0 david      (501) staff       (20)      162 2015-09-06 01:24:09.000000 specsim-0.8/licenses/README.rst
--rw-r--r--   0 david      (501) staff       (20)      303 2017-03-25 16:30:30.000000 specsim-0.8/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      874 2016-09-16 15:47:06.000000 specsim-0.8/README.rst
--rw-r--r--   0 david      (501) staff       (20)     1368 2017-03-25 16:29:55.000000 specsim-0.8/setup.cfg
--rwxr-xr-x   0 david      (501) staff       (20)     4837 2017-03-25 16:25:43.000000 specsim-0.8/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/specsim/
--rw-r--r--   0 david      (501) staff       (20)      512 2016-08-23 21:22:33.000000 specsim-0.8/specsim/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     5273 2015-09-06 01:24:09.000000 specsim-0.8/specsim/_astropy_init.py
--rw-r--r--   0 david      (501) staff       (20)    27521 2017-03-25 14:58:54.000000 specsim-0.8/specsim/atmosphere.py
--rw-r--r--   0 david      (501) staff       (20)    17235 2017-03-25 14:58:54.000000 specsim-0.8/specsim/camera.py
--rw-r--r--   0 david      (501) staff       (20)    26292 2017-03-16 01:28:05.000000 specsim-0.8/specsim/config.py
--rw-r--r--   0 david      (501) staff       (20)     1435 2016-08-23 23:10:48.000000 specsim-0.8/specsim/conftest.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/specsim/data/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/specsim/data/config/
--rw-r--r--   0 david      (501) staff       (20)    15812 2017-03-14 21:48:08.000000 specsim-0.8/specsim/data/config/desi.yaml
--rw-r--r--   0 david      (501) staff       (20)     7884 2017-03-25 14:58:54.000000 specsim-0.8/specsim/data/config/test.yaml
--rw-r--r--   0 david      (501) staff       (20)      523 2016-08-23 23:10:48.000000 specsim-0.8/specsim/data/README.rst
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/specsim/data/test/
--rw-r--r--   0 david      (501) staff       (20)     5482 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_extinction.ecsv
--rw-r--r--   0 david      (501) staff       (20)      244 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_fiberloss.ecsv
--rw-r--r--   0 david      (501) staff       (20)      434 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_psf.ecsv
--rw-r--r--   0 david      (501) staff       (20)     5982 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_sky.ecsv
--rw-r--r--   0 david      (501) staff       (20)     4948 2016-02-24 18:21:04.000000 specsim-0.8/specsim/data/test/test_solar.ecsv
--rw-r--r--   0 david      (501) staff       (20)      274 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_source.ecsv
--rw-r--r--   0 david      (501) staff       (20)      282 2016-02-20 01:15:47.000000 specsim-0.8/specsim/data/test/test_throughput.ecsv
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:29.000000 specsim-0.8/specsim/extern/
--rw-r--r--   0 david      (501) staff       (20)      397 2015-09-06 01:24:09.000000 specsim-0.8/specsim/extern/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    21320 2017-03-25 14:58:54.000000 specsim-0.8/specsim/fiberloss.py
--rw-r--r--   0 david      (501) staff       (20)    31008 2017-03-25 14:58:54.000000 specsim-0.8/specsim/instrument.py
--rw-r--r--   0 david      (501) staff       (20)     8888 2017-03-25 14:58:54.000000 specsim-0.8/specsim/observation.py
--rw-r--r--   0 david      (501) staff       (20)     4327 2017-03-14 21:48:08.000000 specsim-0.8/specsim/quickfiberloss.py
--rw-r--r--   0 david      (501) staff       (20)     6620 2017-03-25 14:58:54.000000 specsim-0.8/specsim/quickspecsim.py
--rw-r--r--   0 david      (501) staff       (20)    30758 2017-03-25 14:58:54.000000 specsim-0.8/specsim/simulator.py
--rw-r--r--   0 david      (501) staff       (20)    16158 2017-03-14 21:48:08.000000 specsim-0.8/specsim/source.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:30.000000 specsim-0.8/specsim/tests/
--rw-r--r--   0 david      (501) staff       (20)      121 2015-09-06 01:24:09.000000 specsim-0.8/specsim/tests/__init__.py
--rw-r--r--   0 david      (501) staff       (20)      768 2015-09-06 01:24:09.000000 specsim-0.8/specsim/tests/coveragerc
--rw-r--r--   0 david      (501) staff       (20)       96 2015-09-06 01:24:09.000000 specsim-0.8/specsim/tests/setup_package.py
--rw-r--r--   0 david      (501) staff       (20)     3393 2017-03-25 14:58:54.000000 specsim-0.8/specsim/tests/test_atmosphere.py
--rw-r--r--   0 david      (501) staff       (20)     1208 2016-10-16 19:20:23.000000 specsim-0.8/specsim/tests/test_camera.py
--rw-r--r--   0 david      (501) staff       (20)     2922 2016-08-28 17:05:39.000000 specsim-0.8/specsim/tests/test_config.py
--rw-r--r--   0 david      (501) staff       (20)     1038 2017-03-25 14:58:54.000000 specsim-0.8/specsim/tests/test_fiberloss.py
--rw-r--r--   0 david      (501) staff       (20)      568 2016-08-28 17:05:39.000000 specsim-0.8/specsim/tests/test_instrument.py
--rw-r--r--   0 david      (501) staff       (20)      914 2017-03-14 21:48:08.000000 specsim-0.8/specsim/tests/test_observation.py
--rw-r--r--   0 david      (501) staff       (20)      266 2017-03-14 21:48:08.000000 specsim-0.8/specsim/tests/test_quickspecsim.py
--rw-r--r--   0 david      (501) staff       (20)     2963 2017-03-25 14:58:54.000000 specsim-0.8/specsim/tests/test_simulator.py
--rw-r--r--   0 david      (501) staff       (20)     2214 2016-02-24 18:21:04.000000 specsim-0.8/specsim/tests/test_source.py
--rw-r--r--   0 david      (501) staff       (20)    12680 2017-01-17 19:28:16.000000 specsim-0.8/specsim/tests/test_transform.py
--rw-r--r--   0 david      (501) staff       (20)    25767 2017-03-09 18:24:08.000000 specsim-0.8/specsim/transform.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2017-03-25 16:30:30.000000 specsim-0.8/specsim/utils/
--rw-r--r--   0 david      (501) staff       (20)      199 2015-09-06 01:24:09.000000 specsim-0.8/specsim/utils/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     6955 2017-03-25 16:30:23.000000 specsim-0.8/specsim/version.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/
+-rw-r--r--   0 david      (501) staff       (20)    36162 2017-01-10 00:52:54.000000 specsim-0.9/ah_bootstrap.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/
+-rw-r--r--   0 david      (501) staff       (20)    36162 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/ah_bootstrap.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/
+-rw-r--r--   0 david      (501) staff       (20)     1836 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/
+-rw-r--r--   0 david      (501) staff       (20)        0 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2940 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/_dummy.py
+-rw-r--r--   0 david      (501) staff       (20)    11701 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/_test_compat.py
+-rw-r--r--   0 david      (501) staff       (20)    19503 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/build_ext.py
+-rw-r--r--   0 david      (501) staff       (20)     1454 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/build_py.py
+-rw-r--r--   0 david      (501) staff       (20)    10020 2017-03-20 19:28:52.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/build_sphinx.py
+-rw-r--r--   0 david      (501) staff       (20)      486 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/install.py
+-rw-r--r--   0 david      (501) staff       (20)      512 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/install_lib.py
+-rw-r--r--   0 david      (501) staff       (20)     2407 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/register.py
+-rw-r--r--   0 david      (501) staff       (20)      120 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/setup_package.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/src/
+-rw-r--r--   0 david      (501) staff       (20)     3033 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/src/compiler.c
+-rw-r--r--   0 david      (501) staff       (20)     1356 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/commands/test.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/compat/
+-rw-r--r--   0 david      (501) staff       (20)      368 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/compat/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/compat/_subprocess_py2/
+-rw-r--r--   0 david      (501) staff       (20)     1306 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/compat/_subprocess_py2/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      551 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/compat/subprocess.py
+-rw-r--r--   0 david      (501) staff       (20)     7917 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/distutils_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)     6104 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/git_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)    26333 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/setup_helpers.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/
+-rw-r--r--   0 david      (501) staff       (20)      268 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    12370 2017-03-20 19:28:52.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/conf.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/
+-rw-r--r--   0 david      (501) staff       (20)       94 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     4527 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/astropyautosummary.py
+-rw-r--r--   0 david      (501) staff       (20)     4802 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/autodoc_enhancements.py
+-rw-r--r--   0 david      (501) staff       (20)    14495 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/automodapi.py
+-rw-r--r--   0 david      (501) staff       (20)    25020 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/automodsumm.py
+-rw-r--r--   0 david      (501) staff       (20)     2832 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
+-rw-r--r--   0 david      (501) staff       (20)     5417 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/comment_eater.py
+-rw-r--r--   0 david      (501) staff       (20)    24740 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/compiler_unparse.py
+-rw-r--r--   0 david      (501) staff       (20)    18074 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/docscrape.py
+-rw-r--r--   0 david      (501) staff       (20)     9527 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/docscrape_sphinx.py
+-rw-r--r--   0 david      (501) staff       (20)     1310 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
+-rw-r--r--   0 david      (501) staff       (20)     5898 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
+-rw-r--r--   0 david      (501) staff       (20)     6693 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/numpydoc.py
+-rw-r--r--   0 david      (501) staff       (20)     5854 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/phantom_import.py
+-rw-r--r--   0 david      (501) staff       (20)     3712 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/smart_resolver.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/
+-rw-r--r--   0 david      (501) staff       (20)      170 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/base.rst
+-rw-r--r--   0 david      (501) staff       (20)     1161 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/class.rst
+-rw-r--r--   0 david      (501) staff       (20)      703 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/module.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/
+-rw-r--r--   0 david      (501) staff       (20)     1817 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1699 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_autodoc_enhancements.py
+-rw-r--r--   0 david      (501) staff       (20)     7870 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodapi.py
+-rw-r--r--   0 david      (501) staff       (20)     2434 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodsumm.py
+-rw-r--r--   0 david      (501) staff       (20)    18153 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_docscrape.py
+-rw-r--r--   0 david      (501) staff       (20)      996 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_utils.py
+-rw-r--r--   0 david      (501) staff       (20)      677 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
+-rw-r--r--   0 david      (501) staff       (20)     4310 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/traitsdoc.py
+-rw-r--r--   0 david      (501) staff       (20)     6179 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/utils.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/
+-rw-r--r--   0 david      (501) staff       (20)      562 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
+-rw-r--r--   0 david      (501) staff       (20)     1638 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
+-rw-r--r--   0 david      (501) staff       (20)      658 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
+-rw-r--r--   0 david      (501) staff       (20)     2820 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
+-rw-r--r--   0 david      (501) staff       (20)      325 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/setup_package.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
+-rw-r--r--   0 david      (501) staff       (20)       73 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
+-rw-r--r--   0 david      (501) staff       (20)     3433 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
+-rw-r--r--   0 david      (501) staff       (20)       34 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
+-rw-r--r--   0 david      (501) staff       (20)      272 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
+-rw-r--r--   0 david      (501) staff       (20)     5201 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
+-rw-r--r--   0 david      (501) staff       (20)     1725 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
+-rw-r--r--   0 david      (501) staff       (20)    32988 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
+-rw-r--r--   0 david      (501) staff       (20)     4634 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
+-rw-r--r--   0 david      (501) staff       (20)     1884 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
+-rw-r--r--   0 david      (501) staff       (20)    12067 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
+-rw-r--r--   0 david      (501) staff       (20)     2769 2017-03-20 19:28:52.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
+-rw-r--r--   0 david      (501) staff       (20)     4971 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
+-rw-r--r--   0 david      (501) staff       (20)      192 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
+-rw-r--r--   0 david      (501) staff       (20)      507 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/test_helpers.py
+-rw-r--r--   0 david      (501) staff       (20)    27953 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/utils.py
+-rw-r--r--   0 david      (501) staff       (20)      546 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers/version.py
+-rw-r--r--   0 david      (501) staff       (20)     9639 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/astropy_helpers/version_helpers.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)        1 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 david      (501) staff       (20)     2970 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     3366 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)       16 2015-09-06 17:00:35.000000 specsim-0.9/astropy_helpers/astropy_helpers.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)    14120 2017-03-20 19:28:52.000000 specsim-0.9/astropy_helpers/CHANGES.rst
+-rw-r--r--   0 david      (501) staff       (20)    12746 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/ez_setup.py
+-rw-r--r--   0 david      (501) staff       (20)     1491 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/LICENSE.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/astropy_helpers/licenses/
+-rw-r--r--   0 david      (501) staff       (20)     2505 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
+-rw-r--r--   0 david      (501) staff       (20)     5959 2015-09-06 17:00:34.000000 specsim-0.9/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
+-rw-r--r--   0 david      (501) staff       (20)     1833 2017-01-10 00:52:12.000000 specsim-0.9/astropy_helpers/README.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/cextern/
+-rw-r--r--   0 david      (501) staff       (20)      298 2015-09-06 01:24:09.000000 specsim-0.9/cextern/README.rst
+-rw-r--r--   0 david      (501) staff       (20)     3779 2017-05-11 20:39:25.000000 specsim-0.9/CHANGES.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/docs/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/docs/_static/
+-rw-r--r--   0 david      (501) staff       (20)   205443 2016-03-09 04:07:13.000000 specsim-0.9/docs/_static/desi_ab22.png
+-rw-r--r--   0 david      (501) staff       (20)    85717 2016-02-24 18:21:04.000000 specsim-0.9/docs/_static/desi_atmosphere.png
+-rw-r--r--   0 david      (501) staff       (20)    82453 2016-02-24 18:21:04.000000 specsim-0.9/docs/_static/desi_bright_atmosphere.png
+-rw-r--r--   0 david      (501) staff       (20)    76022 2016-02-20 01:15:47.000000 specsim-0.9/docs/_static/desi_instrument.png
+-rw-r--r--   0 david      (501) staff       (20)    78276 2016-02-24 18:21:04.000000 specsim-0.9/docs/_static/desi_scattered_moon.png
+-rw-r--r--   0 david      (501) staff       (20)    44134 2016-02-20 01:15:47.000000 specsim-0.9/docs/_static/overview.pdf
+-rw-r--r--   0 david      (501) staff       (20)    80680 2016-02-20 01:15:47.000000 specsim-0.9/docs/_static/overview.png
+-rw-r--r--   0 david      (501) staff       (20)    25195 2016-02-24 18:21:04.000000 specsim-0.9/docs/_static/test_atmosphere.png
+-rw-r--r--   0 david      (501) staff       (20)    52855 2016-02-20 01:15:47.000000 specsim-0.9/docs/_static/test_instrument.png
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/docs/_templates/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/docs/_templates/autosummary/
+-rw-r--r--   0 david      (501) staff       (20)      250 2015-09-06 01:24:09.000000 specsim-0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 david      (501) staff       (20)      251 2015-09-06 01:24:09.000000 specsim-0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 david      (501) staff       (20)      252 2015-09-06 01:24:09.000000 specsim-0.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 david      (501) staff       (20)     2036 2017-03-14 21:48:08.000000 specsim-0.9/docs/api.rst
+-rw-r--r--   0 david      (501) staff       (20)     2814 2017-03-14 21:48:08.000000 specsim-0.9/docs/cmdline.rst
+-rw-r--r--   0 david      (501) staff       (20)     6497 2017-03-25 16:25:43.000000 specsim-0.9/docs/conf.py
+-rw-r--r--   0 david      (501) staff       (20)    10735 2016-08-28 17:05:39.000000 specsim-0.9/docs/config.rst
+-rw-r--r--   0 david      (501) staff       (20)     4597 2017-03-17 17:10:35.000000 specsim-0.9/docs/fiberloss.rst
+-rw-r--r--   0 david      (501) staff       (20)     7564 2017-03-25 14:58:54.000000 specsim-0.9/docs/guide.rst
+-rw-r--r--   0 david      (501) staff       (20)     1611 2016-02-24 18:21:04.000000 specsim-0.9/docs/history.rst
+-rw-r--r--   0 david      (501) staff       (20)      467 2017-03-25 14:58:54.000000 specsim-0.9/docs/index.rst
+-rw-r--r--   0 david      (501) staff       (20)     2945 2017-03-25 14:58:54.000000 specsim-0.9/docs/install.rst
+-rw-r--r--   0 david      (501) staff       (20)     4513 2015-09-06 01:24:09.000000 specsim-0.9/docs/make.bat
+-rw-r--r--   0 david      (501) staff       (20)     4581 2016-08-23 23:10:48.000000 specsim-0.9/docs/Makefile
+-rw-r--r--   0 david      (501) staff       (20)     7068 2017-05-09 13:46:50.000000 specsim-0.9/docs/output.rst
+-rw-r--r--   0 david      (501) staff       (20)       48 2015-09-07 18:12:51.000000 specsim-0.9/docs/rtd-pip-requirements
+-rw-r--r--   0 david      (501) staff       (20)    12385 2016-08-23 23:10:48.000000 specsim-0.9/ez_setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/licenses/
+-rw-r--r--   0 david      (501) staff       (20)     1508 2015-11-03 13:28:41.000000 specsim-0.9/licenses/LICENSE.rst
+-rw-r--r--   0 david      (501) staff       (20)      162 2015-09-06 01:24:09.000000 specsim-0.9/licenses/README.rst
+-rw-r--r--   0 david      (501) staff       (20)      303 2017-05-11 20:40:26.000000 specsim-0.9/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      874 2016-09-16 15:47:06.000000 specsim-0.9/README.rst
+-rw-r--r--   0 david      (501) staff       (20)     1373 2017-05-11 20:39:25.000000 specsim-0.9/setup.cfg
+-rwxr-xr-x   0 david      (501) staff       (20)     4837 2017-03-25 16:25:43.000000 specsim-0.9/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/
+-rw-r--r--   0 david      (501) staff       (20)      512 2016-08-23 21:22:33.000000 specsim-0.9/specsim/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     5273 2015-09-06 01:24:09.000000 specsim-0.9/specsim/_astropy_init.py
+-rw-r--r--   0 david      (501) staff       (20)    27521 2017-03-25 14:58:54.000000 specsim-0.9/specsim/atmosphere.py
+-rw-r--r--   0 david      (501) staff       (20)    18640 2017-05-09 13:46:50.000000 specsim-0.9/specsim/camera.py
+-rw-r--r--   0 david      (501) staff       (20)    26292 2017-03-16 01:28:05.000000 specsim-0.9/specsim/config.py
+-rw-r--r--   0 david      (501) staff       (20)     1435 2016-08-23 23:10:48.000000 specsim-0.9/specsim/conftest.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/data/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/data/config/
+-rw-r--r--   0 david      (501) staff       (20)    15812 2017-03-14 21:48:08.000000 specsim-0.9/specsim/data/config/desi.yaml
+-rw-r--r--   0 david      (501) staff       (20)     7884 2017-03-25 14:58:54.000000 specsim-0.9/specsim/data/config/test.yaml
+-rw-r--r--   0 david      (501) staff       (20)      523 2016-08-23 23:10:48.000000 specsim-0.9/specsim/data/README.rst
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/data/test/
+-rw-r--r--   0 david      (501) staff       (20)     5482 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_extinction.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      244 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_fiberloss.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      434 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_psf.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     5982 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_sky.ecsv
+-rw-r--r--   0 david      (501) staff       (20)     4948 2016-02-24 18:21:04.000000 specsim-0.9/specsim/data/test/test_solar.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      274 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_source.ecsv
+-rw-r--r--   0 david      (501) staff       (20)      282 2016-02-20 01:15:47.000000 specsim-0.9/specsim/data/test/test_throughput.ecsv
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/extern/
+-rw-r--r--   0 david      (501) staff       (20)      397 2015-09-06 01:24:09.000000 specsim-0.9/specsim/extern/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    21320 2017-03-25 14:58:54.000000 specsim-0.9/specsim/fiberloss.py
+-rw-r--r--   0 david      (501) staff       (20)    31373 2017-05-09 13:46:50.000000 specsim-0.9/specsim/instrument.py
+-rw-r--r--   0 david      (501) staff       (20)     8888 2017-03-25 14:58:54.000000 specsim-0.9/specsim/observation.py
+-rw-r--r--   0 david      (501) staff       (20)     4327 2017-03-14 21:48:08.000000 specsim-0.9/specsim/quickfiberloss.py
+-rw-r--r--   0 david      (501) staff       (20)     6642 2017-05-09 13:46:50.000000 specsim-0.9/specsim/quickspecsim.py
+-rw-r--r--   0 david      (501) staff       (20)    38962 2017-05-09 13:46:50.000000 specsim-0.9/specsim/simulator.py
+-rw-r--r--   0 david      (501) staff       (20)    16158 2017-03-14 21:48:08.000000 specsim-0.9/specsim/source.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/tests/
+-rw-r--r--   0 david      (501) staff       (20)      121 2015-09-06 01:24:09.000000 specsim-0.9/specsim/tests/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      768 2015-09-06 01:24:09.000000 specsim-0.9/specsim/tests/coveragerc
+-rw-r--r--   0 david      (501) staff       (20)       96 2015-09-06 01:24:09.000000 specsim-0.9/specsim/tests/setup_package.py
+-rw-r--r--   0 david      (501) staff       (20)     3393 2017-03-25 14:58:54.000000 specsim-0.9/specsim/tests/test_atmosphere.py
+-rw-r--r--   0 david      (501) staff       (20)     2680 2017-05-09 13:46:50.000000 specsim-0.9/specsim/tests/test_camera.py
+-rw-r--r--   0 david      (501) staff       (20)     2922 2016-08-28 17:05:39.000000 specsim-0.9/specsim/tests/test_config.py
+-rw-r--r--   0 david      (501) staff       (20)     1038 2017-03-25 14:58:54.000000 specsim-0.9/specsim/tests/test_fiberloss.py
+-rw-r--r--   0 david      (501) staff       (20)      692 2017-05-09 13:46:50.000000 specsim-0.9/specsim/tests/test_instrument.py
+-rw-r--r--   0 david      (501) staff       (20)      914 2017-03-14 21:48:08.000000 specsim-0.9/specsim/tests/test_observation.py
+-rw-r--r--   0 david      (501) staff       (20)      266 2017-03-14 21:48:08.000000 specsim-0.9/specsim/tests/test_quickspecsim.py
+-rw-r--r--   0 david      (501) staff       (20)     4556 2017-05-09 13:46:50.000000 specsim-0.9/specsim/tests/test_simulator.py
+-rw-r--r--   0 david      (501) staff       (20)     2214 2016-02-24 18:21:04.000000 specsim-0.9/specsim/tests/test_source.py
+-rw-r--r--   0 david      (501) staff       (20)    12680 2017-01-17 19:28:16.000000 specsim-0.9/specsim/tests/test_transform.py
+-rw-r--r--   0 david      (501) staff       (20)    25767 2017-03-09 18:24:08.000000 specsim-0.9/specsim/transform.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2017-05-11 20:40:26.000000 specsim-0.9/specsim/utils/
+-rw-r--r--   0 david      (501) staff       (20)      199 2015-09-06 01:24:09.000000 specsim-0.9/specsim/utils/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     6956 2017-05-11 20:39:57.000000 specsim-0.9/specsim/version.py
```

### Comparing `specsim-0.8/ah_bootstrap.py` & `specsim-0.9/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/ah_bootstrap.py` & `specsim-0.9/astropy_helpers/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/__init__.py` & `specsim-0.9/astropy_helpers/astropy_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/_dummy.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/_dummy.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/_test_compat.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/_test_compat.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/build_ext.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/build_ext.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/build_py.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/build_py.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/build_sphinx.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/build_sphinx.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/install_lib.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/install_lib.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/register.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/register.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/src/compiler.c` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/src/compiler.c`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/commands/test.py` & `specsim-0.9/astropy_helpers/astropy_helpers/commands/test.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/compat/_subprocess_py2/__init__.py` & `specsim-0.9/astropy_helpers/astropy_helpers/compat/_subprocess_py2/__init__.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/compat/subprocess.py` & `specsim-0.9/astropy_helpers/astropy_helpers/compat/subprocess.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/distutils_helpers.py` & `specsim-0.9/astropy_helpers/astropy_helpers/distutils_helpers.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/git_helpers.py` & `specsim-0.9/astropy_helpers/astropy_helpers/git_helpers.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/setup_helpers.py` & `specsim-0.9/astropy_helpers/astropy_helpers/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/conf.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/astropyautosummary.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/astropyautosummary.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/autodoc_enhancements.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/autodoc_enhancements.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/automodapi.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/automodapi.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/automodsumm.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/automodsumm.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/comment_eater.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/comment_eater.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/compiler_unparse.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/compiler_unparse.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/docscrape.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/docscrape.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/docscrape_sphinx.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/numpydoc.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/numpydoc.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/phantom_import.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/phantom_import.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/smart_resolver.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/smart_resolver.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/class.rst` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/class.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/module.rst` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/templates/autosummary_core/module.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_autodoc_enhancements.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_autodoc_enhancements.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodapi.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodapi.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodsumm.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_automodsumm.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_docscrape.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_docscrape.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_utils.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/traitsdoc.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/traitsdoc.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/ext/utils.py` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/ext/utils.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js` & `specsim-0.9/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/utils.py` & `specsim-0.9/astropy_helpers/astropy_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/version.py` & `specsim-0.9/astropy_helpers/astropy_helpers/version.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers/version_helpers.py` & `specsim-0.9/astropy_helpers/astropy_helpers/version_helpers.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers.egg-info/PKG-INFO` & `specsim-0.9/astropy_helpers/astropy_helpers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt` & `specsim-0.9/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/CHANGES.rst` & `specsim-0.9/astropy_helpers/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/ez_setup.py` & `specsim-0.9/astropy_helpers/ez_setup.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/LICENSE.rst` & `specsim-0.9/astropy_helpers/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst` & `specsim-0.9/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst` & `specsim-0.9/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/astropy_helpers/README.rst` & `specsim-0.9/astropy_helpers/README.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/CHANGES.rst` & `specsim-0.9/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.9 (2017-05-11)
+----------------
+
+- Fix Simulator output table units with astropy 1.3.2 (#62).
+- Add support for simulating calibration exposures (#54).
+- Add wavelength min/max options to Simulator.plot().
+- Better support for alternate simulation wavelength grids (PR #60).
+- Add Simulator option to not create and fill per-camera output tables (PR #67).
+
 0.8 (2017-03-25)
 ----------------
 
 This version adds the ability to specify per-fiber positions and source
 properties.  Fiber acceptance fractions can now be calculated on the fly
 (using GalSim) to simulate realistic throughput variations across the
 focal plane.
```

### Comparing `specsim-0.8/docs/_static/desi_ab22.png` & `specsim-0.9/docs/_static/desi_ab22.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/desi_atmosphere.png` & `specsim-0.9/docs/_static/desi_atmosphere.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/desi_bright_atmosphere.png` & `specsim-0.9/docs/_static/desi_bright_atmosphere.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/desi_instrument.png` & `specsim-0.9/docs/_static/desi_instrument.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/desi_scattered_moon.png` & `specsim-0.9/docs/_static/desi_scattered_moon.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/overview.pdf` & `specsim-0.9/docs/_static/overview.pdf`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/overview.png` & `specsim-0.9/docs/_static/overview.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/test_atmosphere.png` & `specsim-0.9/docs/_static/test_atmosphere.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/_static/test_instrument.png` & `specsim-0.9/docs/_static/test_instrument.png`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/api.rst` & `specsim-0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/cmdline.rst` & `specsim-0.9/docs/cmdline.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/conf.py` & `specsim-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/config.rst` & `specsim-0.9/docs/config.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/fiberloss.rst` & `specsim-0.9/docs/fiberloss.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/guide.rst` & `specsim-0.9/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/history.rst` & `specsim-0.9/docs/history.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/install.rst` & `specsim-0.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/make.bat` & `specsim-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/Makefile` & `specsim-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `specsim-0.8/docs/output.rst` & `specsim-0.9/docs/output.rst`

 * *Files 5% similar despite different names*

```diff
@@ -53,23 +53,33 @@
 | ``num_sky_electrons_*``    | Number of sky electrons recorded by the CCD    |
 +----------------------------+------------------------------------------------+
 | ``num_dark_electrons_*``   | Number of dark current electrons in the CCD    |
 +----------------------------+------------------------------------------------+
 | ``read_noise_electrons_*`` | RMS read noise in electrons for the CCD        |
 +----------------------------+------------------------------------------------+
 
+Note that the ``num_source_electrons_*`` and ``num_sky_electrons_*`` arrays are
+normally convolved with the appropriate camera resolution, but this convolution
+is not performed by a :class:`specsim.simulator.Simulator` initialized using the
+option ``camera_output = False``.  This can be useful when specsim is
+being used to calculate inputs to a more detailed pixel-level simulation.
+
 Camera Output Tables
 --------------------
 
 The table below defines the columns of each table listed in
 :attr:`camera_output <specsim.simulator.Simulator.camera_output>`.
 The initial ``wavelength``
 column has shape (nwlen_out) and the remaining columns all have shape
 (nwlen_out, nfibers).
 
+These tables can require a lot of memory so, if they are not needed,
+initialize your :class:`specsim.simulator.Simulator` using the option
+``camera_output = False`` to save space and speed up simulations.
+
 +----------------------------+------------------------------------------------+
 | Column Name                | Description                                    |
 +============================+================================================+
 | ``wavelength``             | Central wavelength of each output pixel        |
 +----------------------------+------------------------------------------------+
 | ``num_source_electrons``   | Number of source electrons recorded by the CCD |
 +----------------------------+------------------------------------------------+
```

### Comparing `specsim-0.8/ez_setup.py` & `specsim-0.9/ez_setup.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/licenses/LICENSE.rst` & `specsim-0.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/README.rst` & `specsim-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/setup.cfg` & `specsim-0.9/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 build-dir = docs/_build
 all_files = 1
 
 [upload_docs]
 upload-dir = docs/_build/html
 show-response = 1
 
-[pytest]
+[tool:pytest]
 minversion = 2.2
 norecursedirs = build docs/_build
 doctest_plus = enabled
 
 [ah_bootstrap]
 auto_use = True
 
@@ -43,12 +43,12 @@
 author_email = dkirkby@uci.edu
 license = BSD
 url = https://github.com/desihub/specsim
 edit_on_github = True
 github_project = desihub/specsim
 install_requires = astropy scipy pyyaml speclite
 # version should be PEP440 compatible (http://www.python.org/dev/peps/pep-0440)
-version = 0.8
+version = 0.9
 
 [entry_points]
 quickspecsim = specsim.quickspecsim:main
 quickfiberloss = specsim.quickfiberloss:main
```

### Comparing `specsim-0.8/setup.py` & `specsim-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/__init__.py` & `specsim-0.9/specsim/__init__.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/_astropy_init.py` & `specsim-0.9/specsim/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/atmosphere.py` & `specsim-0.9/specsim/atmosphere.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/camera.py` & `specsim-0.9/specsim/camera.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,28 +60,34 @@
     num_sigmas_clip : float
         Number of sigmas where the resolution should be clipped when building
         a sparse resolution matrix.
     output_pixel_size : astropy.units.Quantity
         Size of output pixels for this camera.  Units are required, e.g.
         Angstrom. Must be a multiple of the the spacing of the wavelength
         input parameter.
+    allow_convolution : bool
+        Set True to precompute the sparse resolution matrix needed by
+        :meth:`get_output_resolution_matrix`, :meth:`apply_resolution` and
+        :meth:`downsample`.
     """
     def __init__(self, name, wavelength, throughput, row_size,
                  fwhm_resolution, neff_spatial, read_noise, dark_current,
-                 gain, num_sigmas_clip, output_pixel_size):
+                 gain, num_sigmas_clip, output_pixel_size,
+                 allow_convolution=True):
         self.name = name
         self._wavelength = wavelength.to(self._wavelength_unit).value
         self.throughput = throughput
         self._row_size = row_size.to(self._wavelength_unit / u.pixel).value
         self._fwhm_resolution = fwhm_resolution.to(self._wavelength_unit).value
         self._neff_spatial = neff_spatial.to(u.pixel).value
         self.read_noise = read_noise
         self.dark_current = dark_current
         self.gain = gain
         self.num_sigmas_clip = num_sigmas_clip
+        self.allow_convolution = allow_convolution
 
         # The arrays defining the CCD properties must all have identical
         # wavelength coverage.
         ccd_nonzero = np.where(self._row_size > 0)[0]
         ccd_start, ccd_stop = ccd_nonzero[0], ccd_nonzero[-1] + 1
         if (np.any(self._fwhm_resolution[:ccd_start] != 0) or
             np.any(self._fwhm_resolution[ccd_stop:] != 0)):
@@ -171,14 +177,19 @@
 
         # The columns of the resolution matrix are clipped to the CCD coverage.
         column_start = np.maximum(eval_start, ccd_start)
         column_stop = np.minimum(eval_stop, ccd_stop)
         column_size = column_stop - column_start
         assert np.all(column_size > 0)
 
+        # The remaining steps are only necessary to support convolution
+        # and downsampling.
+        if not self.allow_convolution:
+            return
+
         # Prepare start, stop values for slicing eval -> column.
         trim_start = column_start - eval_start
         trim_stop = column_stop - eval_start
         assert np.all(trim_stop > trim_start)
 
         # Prepare a sparse resolution matrix in compressed column format.
         matrix_size = np.sum(column_size)
@@ -217,40 +228,44 @@
         self._output_pixel_size = (
             output_pixel_size.to(self._wavelength_unit).value)
         # Check that we can downsample simulation pixels to obtain
         # output pixels.  This check will only work if the simulation
         # grid is equally spaced, but no other part of the Camera class
         # class currently requires this.
         wavelength_step = self._wavelength[1] - self._wavelength[0]
+        if not np.allclose(np.diff(self._wavelength), wavelength_step):
+            raise RuntimeError(
+                'Non-uniform simulation wavelength grid not supported yet.')
         self._downsampling = int(round(
             self._output_pixel_size / wavelength_step))
-        num_downsampled = int(
-            (self._wavelength_max - self._wavelength_min) //
-            self._output_pixel_size)
+        if not np.allclose(self._downsampling * wavelength_step,
+                           self._output_pixel_size):
+            raise ValueError(
+                'Invalid output_pixel_size {0} for {1} camera: '
+                .format(output_pixel_size, self.name) +
+                'must be multiple of {0} {1}.'
+                .format(wavelength_step, self._wavelength_unit))
+        # The self._wavelength array stores the centers of fixed-width bins.
+        # Calculate the edges of the downsampled output pixels. Trim
+        # any partial output pixel on the high end.
+        output_min = self._wavelength_min - 0.5 * wavelength_step
+        output_max = self._wavelength_max + 0.5 * wavelength_step
+        num_downsampled = int(np.floor(
+            (output_max - output_min) / self._output_pixel_size))
         pixel_edges = (
-            self._wavelength_min - 0.5 * wavelength_step +
+            output_min +
             np.arange(num_downsampled + 1) * self._output_pixel_size)
-        sim_edges = (
-            self._wavelength[self.ccd_slice][::self._downsampling] -
-             0.5 * wavelength_step)
-        if not np.allclose(
-            pixel_edges, sim_edges, rtol=0., atol=1e-6 * wavelength_step):
-            raise ValueError(
-                'Cannot downsample {0}-camera pixels from {1:f} to {2} {3}.'
-                .format(self.name, wavelength_step, self._output_pixel_size,
-                        self._wavelength_unit))
         # Save the centers of each output pixel.
         self._output_wavelength = 0.5 * (pixel_edges[1:] + pixel_edges[:-1])
         # Initialize the parameters used by the downsample() method.
         self._output_slice = slice(
             self.ccd_slice.start,
             self.ccd_slice.start + num_downsampled * self._downsampling)
         self._downsampled_shape = (num_downsampled, self._downsampling)
 
-
     def get_output_resolution_matrix(self):
         """Return the output resolution matrix in DIA sparse format.
 
         The output resolution is calculated by summing output pixel
         blocks of the full resolution matrix.  This is equivalent to
         the convolution of our resolution with a boxcar representing
         an output pixel. Edge effects are not handled very gracefully
@@ -263,14 +278,16 @@
 
         Returns
         -------
         :class:`scipy.sparse.dia_matrix`
             Square array of resolution matrix elements in the DIA
             sparse format.
         """
+        if not self.allow_convolution:
+            raise RuntimeError('Camera created with allow_convolution False.')
         n = len(self._output_wavelength)
         m = self._downsampling
         i0 = self.ccd_slice.start - self.response_slice.start
         output_slice = slice(i0, i0 + n * m)
         # Initialize CSR format arrays for building the output matrix.
         indptr_out = np.empty((n + 1,), int)
         indices_out = []
@@ -311,89 +328,87 @@
 
         # Build the output matrix in CSR format.
         R = scipy.sparse.csr_matrix((data_out, indices_out, indptr_out), (n, n))
 
         # Convert to DIA format and return.
         return R.todia()
 
-
     def downsample(self, data, method=np.sum):
         """Downsample data tabulated on the simulation grid to output pixels.
         """
+        if not self.allow_convolution:
+            raise RuntimeError('Camera created with allow_convolution False.')
         data = np.asanyarray(data)
         if data.shape[-1] != len(self._wavelength):
             raise ValueError(
                 'Invalid data shape for downsampling: {0}.'.format(data.shape))
 
         output = data[..., self._output_slice]
         new_shape = output.shape[:-1] + self._downsampled_shape
         return method(output.reshape(new_shape), axis=-1)
 
-
     def apply_resolution(self, flux):
         """
         Input should be on the simulation wavelength grid.
 
         Any throughput should already be applied.
         """
+        if not self.allow_convolution:
+            raise RuntimeError('Camera created with allow_convolution False.')
         flux = np.asarray(flux)
         dispersed = np.zeros_like(flux)
 
         dispersed[..., self.ccd_slice] = self._resolution_matrix.dot(
             flux[..., self.response_slice].T).T
 
         return dispersed
 
-
     # Canonical wavelength unit used for all internal arrays.
     _wavelength_unit = u.Angstrom
 
-
     @property
     def wavelength_min(self):
         """Minimum wavelength covered by this camera's CCD.
         """
         return self._wavelength_min * self._wavelength_unit
 
-
     @property
     def wavelength_max(self):
         """Maximum wavelength covered by this camera's CCD.
         """
         return self._wavelength_max * self._wavelength_unit
 
-
     @property
     def rms_resolution(self):
         """Array of RMS resolution values.
         """
         return self._rms_resolution * self._wavelength_unit
 
-
     @property
     def row_size(self):
         """Array of row sizes in the dispersion direction.
         """
         return self._row_size * self._wavelength_unit / u.pixel
 
-
     @property
     def neff_spatial(self):
         """Array of effective pixel dimensions in the spatial (fiber) direction.
         """
         return self._neff_spatial * u.pixel
 
-
     @property
     def output_pixel_size(self):
         """Size of output pixels.
 
         Must be a multiple of the simulation wavelength grid.
         """
+        if not self.allow_convolution:
+            raise RuntimeError('Camera created with allow_convolution False.')
         return self._output_pixel_size * self._wavelength_unit
 
-
     @property
     def output_wavelength(self):
         """Output pixel central wavelengths.
         """
+        if not self.allow_convolution:
+            raise RuntimeError('Camera created with allow_convolution False.')
         return self._output_wavelength * self._wavelength_unit
```

### Comparing `specsim-0.8/specsim/config.py` & `specsim-0.9/specsim/config.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/conftest.py` & `specsim-0.9/specsim/conftest.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/config/desi.yaml` & `specsim-0.9/specsim/data/config/desi.yaml`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/config/test.yaml` & `specsim-0.9/specsim/data/config/test.yaml`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/README.rst` & `specsim-0.9/specsim/data/README.rst`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/test/test_extinction.ecsv` & `specsim-0.9/specsim/data/test/test_extinction.ecsv`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/test/test_sky.ecsv` & `specsim-0.9/specsim/data/test/test_sky.ecsv`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/data/test/test_solar.ecsv` & `specsim-0.9/specsim/data/test/test_solar.ecsv`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/fiberloss.py` & `specsim-0.9/specsim/fiberloss.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/instrument.py` & `specsim-0.9/specsim/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 import specsim.camera
 
 
 class Instrument(object):
     """Model the instrument response of a fiber spectrograph.
 
     A spectrograph can have multiple :mod:`cameras <specsim.camera>` with
-    different wavelength coverages.
+    different wavelength coverages. Objects representing each camera are
+    contained in a list accessible from our ``cameras`` attribute, which will
+    be in order of increasing effective wavelength.
 
     No instrument attributes can be changed after an instrument has been
-    created. File a github issue if you would like to change this.
+    created. Create a github issue if you would like to change this.
 
     Parameters
     ----------
     name : str
         Descriptive name of this instrument.
     wavelength : astropy.units.Quantity
         Array of wavelength bin centers where the instrument response is
@@ -565,24 +567,27 @@
         ax2.set_ylabel('RMS Resolution, Row Size [{0}]'.format(wave_unit))
         ax2_rhs.set_ylim(0., None)
         ax2_rhs.set_ylabel('Effective Column Size [pixels]')
         ax2.set_xlabel('Wavelength [{0}]'.format(wave_unit))
         ax2.set_xlim(wave[0], wave[-1])
 
 
-def initialize(config):
+def initialize(config, camera_output=True):
     """Initialize the instrument model from configuration parameters.
 
     This method is responsible for creating a new :class:`Instrument` as
     well as the :class:`Cameras <specsim.camera.Camera>` it includes.
 
     Parameters
     ----------
     config : :class:`specsim.config.Configuration`
         The configuration parameters to use.
+    camera_output : bool
+        Initialize support for resolution convolution and downsampling for
+        each camera when True.
 
     Returns
     -------
     Instrument
         An initialized instrument model including one or more
         :class:`cameras <specsim.camera.Camera>`.
     """
@@ -599,15 +604,16 @@
             ['read_noise', 'dark_current', 'gain', 'num_sigmas_clip',
              'output_pixel_size'])
         initialized_cameras.append(specsim.camera.Camera(
             camera_name, config.wavelength, throughput,
             ccd['row_size'], ccd['fwhm_resolution'],
             ccd['neff_spatial'], constants['read_noise'],
             constants['dark_current'], constants['gain'],
-            constants['num_sigmas_clip'], constants['output_pixel_size']))
+            constants['num_sigmas_clip'], constants['output_pixel_size'],
+            allow_convolution=camera_output))
 
     constants = config.get_constants(
         config.instrument,
         ['primary_mirror_diameter', 'obscuration_diameter',
          'support_width', 'fiber_diameter', 'field_radius'])
 
     try:
```

### Comparing `specsim-0.8/specsim/observation.py` & `specsim-0.9/specsim/observation.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/quickfiberloss.py` & `specsim-0.9/specsim/quickfiberloss.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/quickspecsim.py` & `specsim-0.9/specsim/quickspecsim.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     config.source.z_in = args.z_in
     config.source.z_out = args.z_out
     config.source.filter_name = args.filter
     config.source.ab_magnitude_out = args.ab_mag
 
     # Initialize the simulator.
     try:
-        simulator = specsim.simulator.Simulator(config)
+        simulator = specsim.simulator.Simulator(config, verbose=args.verbose)
     except RuntimeError as e:
         print(e)
         return -1
 
     # Set parameters after configuration.
     try:
         simulator.observation.exposure_time = specsim.config.parse_quantity(
```

### Comparing `specsim-0.8/specsim/simulator.py` & `specsim-0.9/specsim/simulator.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,25 +49,34 @@
 
     Parameters
     ----------
     config : specsim.config.Configuration or str
         A configuration object or configuration name.
     num_fibers : int
         Number of fibers to simulate.
+    camera_output : bool
+        Include per-camera output tables in simulation results when True.
+        When this is False, our ``camera_output`` attribute will return an
+        empty list and the ``num_source_electrons_*`` columns in our
+        ``simulated`` table will not be resolution convolved.
+        Setting this parameter to False will save memory and time when
+        per-camera outputs are not needed.
+    verbose : bool
+        Print information about the simulation progress.
     """
-    def __init__(self, config, num_fibers=2, verbose=False):
+    def __init__(self, config, num_fibers=2, camera_output=True, verbose=False):
 
         if specsim.config.is_string(config):
             config = specsim.config.load_config(config)
         config.verbose = verbose
         self.verbose = verbose
 
         # Initalize our component models.
         self.atmosphere = specsim.atmosphere.initialize(config)
-        self.instrument = specsim.instrument.initialize(config)
+        self.instrument = specsim.instrument.initialize(config, camera_output)
         self.source = specsim.source.initialize(config)
         self.observation = specsim.observation.initialize(config)
 
         self._num_fibers = int(num_fibers)
         if self._num_fibers < 1:
             raise ValueError('Must have num_fibers >= 1.')
 
@@ -103,84 +112,99 @@
             self._simulated.add_column(astropy.table.Column(
                 name='num_sky_electrons_{0}'.format(name), **column_args))
             self._simulated.add_column(astropy.table.Column(
                 name='num_dark_electrons_{0}'.format(name), **column_args))
             self._simulated.add_column(astropy.table.Column(
                 name='read_noise_electrons_{0}'.format(name), **column_args))
 
+        # Count the number of bytes used in the simulated table.
+        self.table_bytes = 0
+        for name in self._simulated.colnames:
+            d = self._simulated[name].data
+            self.table_bytes += np.prod(d.shape) * d.dtype.itemsize
+
         # Initialize each camera's table of results downsampled to
-        # output pixels.
+        # output pixels, if requested.
         self._camera_output = []
-        for camera in self.instrument.cameras:
-            meta = dict(
-                name=camera.name, num_fibers=self.num_fibers,
-                pixel_size=camera.output_pixel_size)
-            table = astropy.table.Table(meta=meta)
-            column_args['length'] = len(camera.output_wavelength)
-            table.add_column(astropy.table.Column(
-                name='wavelength', data=camera.output_wavelength))
-            table.add_column(astropy.table.Column(
-                name='num_source_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='num_sky_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='num_dark_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='read_noise_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='random_noise_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='variance_electrons', **column_args))
-            table.add_column(astropy.table.Column(
-                name='flux_calibration', **column_args))
-            table.add_column(astropy.table.Column(
-                name='observed_flux', unit=flux_unit, **column_args))
-            table.add_column(astropy.table.Column(
-                name='flux_inverse_variance', unit=flux_unit ** -2,
-                **column_args))
-            self._camera_output.append(table)
-
+        if camera_output:
+            for camera in self.instrument.cameras:
+                meta = dict(
+                    name=camera.name, num_fibers=self.num_fibers,
+                    pixel_size=camera.output_pixel_size)
+                table = astropy.table.Table(meta=meta)
+                column_args['length'] = len(camera.output_wavelength)
+                table.add_column(astropy.table.Column(
+                    name='wavelength', data=camera.output_wavelength))
+                table.add_column(astropy.table.Column(
+                    name='num_source_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='num_sky_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='num_dark_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='read_noise_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='random_noise_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='variance_electrons', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='flux_calibration', **column_args))
+                table.add_column(astropy.table.Column(
+                    name='observed_flux', unit=flux_unit, **column_args))
+                table.add_column(astropy.table.Column(
+                    name='flux_inverse_variance', unit=flux_unit ** -2,
+                    **column_args))
+                # Add bytes used in this table to our running total.
+                for name in table.colnames:
+                    d = table[name].data
+                    self.table_bytes += np.prod(d.shape) * d.dtype.itemsize
+
+                self._camera_output.append(table)
+
+        if self.verbose:
+            print('Allocated {0:.1f}Mb of table data.'
+                  .format(self.table_bytes / (2. ** 20)))
 
     @property
     def num_fibers(self):
         """Number of fibers being simulated.
         """
         return self._num_fibers
 
-
     @property
     def simulated(self):
         """astropy.table.Table: Table of high-resolution simulation results.
 
         This table is tabulated using the high-resolution wavelength used for
         internal calclulations and overwritten during each call to
         :meth:`simulate`.  See :doc:`/output` for details of this table's
         contents.
         """
         return self._simulated
 
-
     @property
     def camera_output(self):
         """list: List of per-camera simulation output tables.
 
         Tables are listed in order of increasing wavelength and tabulated
         using the output pixels defined for each camera.  Tables are overwritten
         during each call to :meth:`simulate`.  See :doc:`/output` for details
         of the contents of each table in this list.
+
+        Returns an empty list if this Simulator was initialized with
+        ``camera_output`` False.
         """
         return self._camera_output
 
-
     def simulate(self, sky_positions=None, focal_positions=None,
                  fiber_acceptance_fraction=None,
                  source_fluxes=None, source_types=None, source_fraction=None,
                  source_half_light_radius=None,
                  source_minor_major_axis_ratio=None, source_position_angle=None,
-                 save_fiberloss=None):
+                 calibration_surface_brightness=None, save_fiberloss=None):
         """Simulate a single exposure.
 
         Simulation results are written to internal tables that are overwritten
         each time this method is called.  Some metadata is also saved as
         attributes of this object: `focal_x`, `focal_y`, `fiber_area`.
 
         The positions and properties of each source can optionally be specified
@@ -196,14 +220,22 @@
         - ``source.location.constants.focal_x,y`` config data.
         - ``source.location.sky`` config data.
         When config data is used, it is duplicated for all fibers. Use the
         verbose mode to see details on how fibers are being positioned. Note
         that the observing airmass will be calculated when positioning with
         sky coordinates, and then available via ``self.observation.airmass``.
 
+        Calibration exposures can be simulated by providing an array of
+        ``calibration_surface_brightness`` values to use.  In this case,
+        the source and fiberloss inputs are ignored, and no atmospheric
+        emission or extinction are applied.
+
+        Per-camera output tables will not be filled if this Simulator was
+        initialized with ``camera_output`` False.
+
         Parameters
         ----------
         sky_positions : astropy.units.Quantity or None
             Sky positions of each object. Must have a length equal to
             num_fibers.  Defaults to ``source.location.sky`` when None.
         focal_positions : astropy.units.Quantity or None
             Focal-plane coordinates of each object relative to the plate
@@ -236,14 +268,20 @@
             axis ratios, in the range (0,1]. Defaults to values in
             ``source.profile.disk,bulge_shape`` when None.
         source_position_angle : array or None
             Array of shape (num_fibers, 2) giving the disk and bulge major
             axis alignments, expressed as a clockwise rotation from the +x
             axis, with angular units. Defaults to values in
             ``source.profile.disk,bulge_shape`` when None.
+        calibration_surface_brightness : array or None
+            Array of shape (num_fibers, num_wlen) giving the calibration
+            source surface brightness illuminating each fiber. When this is
+            set, all source parameters (those beginning with ``source_``)
+            and ``fiber_acceptance_fraction`` are ignored and this is assumed
+            to be a calibration exposure.
         save_fiberloss : str or None
             Basename for saving FITS images and tabulated fiberloss.
             Ignored unless instrument.fiberloss.method is galsim.
         """
         # Get references to our results columns. Since table rows index
         # wavelength, the shape of each column is (nwlen, nfiber) and
         # therefore some transposes are necessary to match with the shape
@@ -255,14 +293,17 @@
         fiberloss = self.simulated['fiberloss']
         source_fiber_flux = self.simulated['source_fiber_flux']
         sky_fiber_flux = self.simulated['sky_fiber_flux']
         num_source_photons = self.simulated['num_source_photons']
         num_sky_photons = self.simulated['num_sky_photons']
         nwlen = len(wavelength)
 
+        # Is this a calibration exposure?
+        calibrating = calibration_surface_brightness is not None
+
         # Position each fiber.
         if focal_positions is not None:
             if len(focal_positions) != self.num_fibers:
                 raise ValueError(
                     'Expected {0:d} focal_positions.'.format(self.num_fibers))
             try:
                 focal_positions = focal_positions.to(u.mm)
@@ -294,15 +335,15 @@
             self.focal_y = np.tile(focal_y, [self.num_fibers])
             on_sky = True
             if self.verbose:
                 print('All fibers positioned at config (ra,dec).')
         else:
             raise RuntimeError('No fiber positioning info available.')
 
-        if on_sky:
+        if not calibrating and on_sky:
             # Set the observing airmass in the atmosphere model using
             # Eqn.3 of Krisciunas & Schaefer 1991.
             obs_zenith = 90 * u.deg - self.observation.boresight_altaz.alt
             obs_airmass = (1 - 0.96 * np.sin(obs_zenith) ** 2) ** -0.5
             self.atmosphere.airmass = obs_airmass
             if self.verbose:
                 print('Calculated alt={0:.1f} az={1:.1f} airmass={2:.3f}'
@@ -321,61 +362,104 @@
             0.5 * self.instrument.fiber_diameter /
             self.instrument.radial_scale(focal_r))
         azimuthal_fiber_size = (
             0.5 * self.instrument.fiber_diameter /
             self.instrument.azimuthal_scale(focal_r))
         self.fiber_area = np.pi * radial_fiber_size * azimuthal_fiber_size
 
-        # Get the source fluxes incident on the atmosphere.
-        if source_fluxes is None:
-            source_fluxes = self.source.flux_out.to(
-                source_flux.unit)[np.newaxis, :]
-        elif source_fluxes.shape != (self.num_fibers, nwlen):
-            raise ValueError('Invalid shape for source_fluxes.')
-        try:
-            source_flux[:] = source_fluxes.to(source_flux.unit).T
-        except u.UnitConversionError as e:
-            raise ValueError('Invalid units for source_fluxes.')
-
-        # Calculate fraction of source illumination entering the fiber.
-        if save_fiberloss is not None:
-            saved_images_file = save_fiberloss + '.fits'
-            saved_table_file = save_fiberloss + '.ecsv'
-        else:
-            saved_images_file, saved_table_file = None, None
-
-        if fiber_acceptance_fraction is None:
-            # Calculate fiberloss using the method specified in
-            # instrument.fiberloss_method.
-            fiber_acceptance_fraction =\
-                specsim.fiberloss.calculate_fiber_acceptance_fraction(
-                    self.focal_x, self.focal_y, wavelength.quantity,
-                    self.source, self.atmosphere, self.instrument, source_types,
-                    source_fraction, source_half_light_radius,
-                    source_minor_major_axis_ratio, source_position_angle,
-                    saved_images_file=saved_images_file,
-                    saved_table_file=saved_table_file)
+        if calibrating:
+            # Convert surface brightness to flux entering each fiber.
+            if calibration_surface_brightness.shape != (self.num_fibers, nwlen):
+                raise ValueError(
+                    'Invalid shape for calibration_surface_brightness.')
+            try:
+                source_flux[:] = (
+                    calibration_surface_brightness.T * self.fiber_area).to(
+                        source_flux.unit)
+            except AttributeError:
+                raise ValueError(
+                    'Missing units for calibration_surface_brightness.')
+            except u.UnitConversionError:
+                raise ValueError(
+                    'Invalid units for calibration_surface_brightness.')
+            # Fiberloss is one.
+            fiberloss[:] = 1.
+            # No atmospheric extinction of calibration sources.
+            source_fiber_flux[:] = source_flux.to(source_fiber_flux.unit)
+            # No sky emission added to calibration sources.
+            sky_fiber_flux[:] = 0.
+            # Calibration from constant source flux entering the fiber to
+            # number of source photons entering the fiber.
+            source_flux_to_photons = (
+                self.instrument.photons_per_bin[:, np.newaxis] *
+                self.observation.exposure_time
+                ).to(source_flux.unit ** -1).value
         else:
-            fiber_acceptance_fraction = np.asarray(fiber_acceptance_fraction)
-            if fiber_acceptance_fraction.shape != (self.num_fibers, nwlen):
-                raise ValueError('Invalid shape for fiber_acceptance_fraction.')
-        fiberloss[:] = fiber_acceptance_fraction.T
-
-        # Calculate the source flux entering a fiber.
-        source_fiber_flux[:] = (
-            source_flux *
-            self.atmosphere.extinction[:, np.newaxis] *
-            fiberloss
-            ).to(source_fiber_flux.unit)
-
-        # Calculate the sky flux entering a fiber.
-        sky_fiber_flux[:] = (
-            self.atmosphere.surface_brightness[:, np.newaxis] *
-            self.fiber_area
-            ).to(sky_fiber_flux.unit)
+            # Get the source fluxes incident on the atmosphere.
+            if source_fluxes is None:
+                source_fluxes = self.source.flux_out.to(
+                    source_flux.unit)[np.newaxis, :]
+            elif source_fluxes.shape != (self.num_fibers, nwlen):
+                raise ValueError('Invalid shape for source_fluxes.')
+            try:
+                source_flux[:] = source_fluxes.to(source_flux.unit).T
+            except AttributeError:
+                raise ValueError('Missing units for source_fluxes.')
+            except u.UnitConversionError:
+                raise ValueError('Invalid units for source_fluxes.')
+
+            # Calculate fraction of source illumination entering the fiber.
+            if save_fiberloss is not None:
+                saved_images_file = save_fiberloss + '.fits'
+                saved_table_file = save_fiberloss + '.ecsv'
+            else:
+                saved_images_file, saved_table_file = None, None
+
+            if fiber_acceptance_fraction is None:
+                # Calculate fiberloss using the method specified in
+                # instrument.fiberloss_method.
+                fiber_acceptance_fraction =\
+                    specsim.fiberloss.calculate_fiber_acceptance_fraction(
+                        self.focal_x, self.focal_y, wavelength.quantity,
+                        self.source, self.atmosphere, self.instrument,
+                        source_types, source_fraction, source_half_light_radius,
+                        source_minor_major_axis_ratio, source_position_angle,
+                        saved_images_file=saved_images_file,
+                        saved_table_file=saved_table_file)
+            else:
+                fiber_acceptance_fraction = np.asarray(
+                    fiber_acceptance_fraction)
+                if fiber_acceptance_fraction.shape != (self.num_fibers, nwlen):
+                    raise ValueError(
+                        'Invalid shape for fiber_acceptance_fraction.')
+            fiberloss[:] = fiber_acceptance_fraction.T
+
+            # Calculate the source flux entering a fiber.
+            source_fiber_flux[:] = (
+                source_flux *
+                self.atmosphere.extinction[:, np.newaxis] *
+                fiberloss
+                ).to(source_fiber_flux.unit)
+
+            # Calculate the sky flux entering a fiber.
+            sky_fiber_flux[:] = (
+                self.atmosphere.surface_brightness[:, np.newaxis] *
+                self.fiber_area
+                ).to(sky_fiber_flux.unit)
+
+            # Calculate the calibration from constant unit source flux above
+            # the atmosphere to number of source photons entering the fiber.
+            # We use this below to calculate the flux inverse variance in
+            # each camera.
+            source_flux_to_photons = (
+                self.atmosphere.extinction[:, np.newaxis] *
+                fiberloss *
+                self.instrument.photons_per_bin[:, np.newaxis] *
+                self.observation.exposure_time
+                ).to(source_flux.unit ** -1).value
 
         # Calculate the mean number of source photons entering the fiber
         # per simulation bin.
         num_source_photons[:] = (
             source_fiber_flux *
             self.instrument.photons_per_bin[:, np.newaxis] *
             self.observation.exposure_time
@@ -385,89 +469,103 @@
         # per simulation bin.
         num_sky_photons[:] = (
             sky_fiber_flux *
             self.instrument.photons_per_bin[:, np.newaxis] *
             self.observation.exposure_time
             ).to(1).value
 
-        # Calculate the calibration from constant unit source flux above
-        # the atmosphere to number of source photons entering the fiber.
-        # We use this below to calculate the flux inverse variance in
-        # each camera.
-        source_flux_to_photons = (
-            self.atmosphere.extinction[:, np.newaxis] *
-            fiberloss *
-            self.instrument.photons_per_bin[:, np.newaxis] *
-            self.observation.exposure_time
-            ).to(source_flux.unit ** -1).value
-
-        # Loop over cameras to calculate their individual responses.
-        for output, camera in zip(self.camera_output, self.instrument.cameras):
-
+        # Calculate the high-resolution inputs to each camera.
+        for camera in self.instrument.cameras:
             # Get references to this camera's columns.
             num_source_electrons = self.simulated[
                 'num_source_electrons_{0}'.format(camera.name)]
             num_sky_electrons = self.simulated[
                 'num_sky_electrons_{0}'.format(camera.name)]
             num_dark_electrons = self.simulated[
                 'num_dark_electrons_{0}'.format(camera.name)]
             read_noise_electrons = self.simulated[
                 'read_noise_electrons_{0}'.format(camera.name)]
 
-            # Calculate the mean number of source electrons detected in the CCD.
-            num_source_electrons[:] = camera.apply_resolution(
-                num_source_photons.T * camera.throughput).T
-
-            # Calculate the mean number of sky electrons detected in the CCD.
-            num_sky_electrons[:] = camera.apply_resolution(
-                num_sky_photons.T * camera.throughput).T
+            # Calculate the mean number of source electrons detected in the CCD
+            # without any resolution applied.
+            num_source_electrons[:] = (
+                num_source_photons * camera.throughput[:, np.newaxis])
+
+            # Calculate the mean number of sky electrons detected in the CCD
+            # without any resolution applied.
+            num_sky_electrons[:] = (
+                num_sky_photons * camera.throughput[:, np.newaxis])
 
             # Calculate the mean number of dark current electrons in the CCD.
             num_dark_electrons[:] = (
                 camera.dark_current_per_bin[:, np.newaxis] *
                 self.observation.exposure_time).to(u.electron).value
 
             # Copy the read noise in units of electrons.
             read_noise_electrons[:] = (
                 camera.read_noise_per_bin[:, np.newaxis].to(u.electron).value)
 
+        if not self.camera_output:
+            # All done since no camera output was requested.
+            return
+
+        # Loop over cameras to calculate their individual responses
+        # with resolution applied and downsampling to output pixels.
+        for output, camera in zip(self.camera_output, self.instrument.cameras):
+
+            # Get references to this camera's columns.
+            num_source_electrons = self.simulated[
+                'num_source_electrons_{0}'.format(camera.name)]
+            num_sky_electrons = self.simulated[
+                'num_sky_electrons_{0}'.format(camera.name)]
+            num_dark_electrons = self.simulated[
+                'num_dark_electrons_{0}'.format(camera.name)]
+            read_noise_electrons = self.simulated[
+                'read_noise_electrons_{0}'.format(camera.name)]
+
+            # Apply resolution to the source and sky detected electrons on
+            # the high-resolution grid.
+            num_source_electrons[:] = camera.apply_resolution(
+                num_source_electrons.T).T
+            num_sky_electrons[:] = camera.apply_resolution(
+                num_sky_electrons.T).T
+
             # Calculate the corresponding downsampled output quantities.
-            output['num_source_electrons'] = (
+            output['num_source_electrons'][:] = (
                 camera.downsample(num_source_electrons.T)).T
-            output['num_sky_electrons'] = (
+            output['num_sky_electrons'][:] = (
                 camera.downsample(num_sky_electrons.T)).T
-            output['num_dark_electrons'] = (
+            output['num_dark_electrons'][:] = (
                 camera.downsample(num_dark_electrons.T)).T
-            output['read_noise_electrons'] = np.sqrt(
+            output['read_noise_electrons'][:] = np.sqrt(
                 camera.downsample(read_noise_electrons.T ** 2)).T
-            output['variance_electrons'] = (
+            output['variance_electrons'][:] = (
                 output['num_source_electrons'] +
                 output['num_sky_electrons'] +
                 output['num_dark_electrons'] +
                 output['read_noise_electrons'] ** 2)
 
             # Calculate the effective calibration from detected electrons to
             # source flux above the atmosphere, downsampled to output pixels.
-            output['flux_calibration'] = 1.0 / camera.downsample(
+            output['flux_calibration'][:] = 1.0 / camera.downsample(
                 camera.apply_resolution(
                     source_flux_to_photons.T * camera.throughput)).T
 
             # Calculate the calibrated flux in this camera.
-            output['observed_flux'] = (
+            output['observed_flux'][:] = (
                 output['flux_calibration'] * output['num_source_electrons'])
 
             # Calculate the corresponding flux inverse variance.
-            output['flux_inverse_variance'] = (
+            output['flux_inverse_variance'][:] = (
                 output['flux_calibration'] ** -2 *
                 output['variance_electrons'] ** -1)
 
             # Zero our random noise realization column.
             output['random_noise_electrons'][:] = 0.
 
-
     def generate_random_noise(self, random_state=None):
         """Generate a random noise realization for the most recent simulation.
 
         Fills the "random_noise_electrons" column in each camera's output
         table, which is zeroed after each call to :meth:`simulate`. Can be
         called repeatedly for the same simulated response to generate different
         noise realizations.
@@ -484,26 +582,28 @@
         Parameters
         ----------
         random_state : numpy.random.RandomState or None
             The random number generation state to use for reproducible noise
             realizations. A new state will be created with a randomized seed
             if None is specified.
         """
+        if not self.camera_output:
+            raise RuntimeError('Simulator initialized with no camera output.')
+
         if random_state is None:
             random_state = np.random.RandomState()
 
         for output in self.camera_output:
             mean_electrons = (
                 output['num_source_electrons'] +
                 output['num_sky_electrons'] + output['num_dark_electrons'])
             output['random_noise_electrons'] = (
                 random_state.poisson(mean_electrons) - mean_electrons +
                 random_state.normal(scale=output['read_noise_electrons']))
 
-
     def save(self, filename, clobber=True):
         """Save results of the last simulation to a FITS file.
 
         Parameters
         ----------
         filename : str
             Name of the file where results should be saved.  Must use the
@@ -525,43 +625,49 @@
         for output in self.camera_output:
             hdus.append(astropy.io.fits.BinTableHDU(
                 name=output.meta['name'], data=output.as_array()))
         # Write the file.
         hdus.writeto(filename, clobber=clobber)
         hdus.close()
 
-
-    def plot(self, fiber=0, title=None):
+    def plot(self, fiber=0, wavelength_min=None, wavelength_max=None,
+             title=None, min_electrons=2.5):
         """Plot results of the last simulation for a single fiber.
 
         Uses the contents of the :attr:`simulated` and :attr:`camera_output`
         astropy tables to plot the results of the last call to :meth:`simulate`.
         See :func:`plot_simulation` for details.
 
         Parameters
         ----------
         fiber : int
             Fiber index to plot.  Must be less than `self.num_fibers`.
+        wavelength_min : quantity or None
+            Clip the plot below this wavelength, or show the full extent.
+        wavelength_max : quantity or None
+            Clip the plot above this wavelength, or show the full extent.
         title : str or None
             Plot title to use.  If None is specified, a title will be
             automatically generated using the source name, airmass and
             exposure time.
         """
         if fiber < 0 or fiber >= self.num_fibers:
             raise ValueError('Requested fiber is out of range.')
         if title is None:
             title = (
                 'Fiber={0}, X={1}, t={2}'
                 .format(fiber, self.atmosphere.airmass,
                         self.observation.exposure_time))
-        plot_simulation(self.simulated, self.camera_output, fiber, title)
+        plot_simulation(self.simulated, self.camera_output, fiber,
+                        wavelength_min, wavelength_max, title, min_electrons)
 
 
-def plot_simulation(simulated, camera_output, fiber=0, title=None,
-                    min_electrons=2.5, figsize=(11, 8.5), label_size='medium'):
+def plot_simulation(simulated, camera_output, fiber=0, wavelength_min=None,
+                    wavelength_max=None, title=None, min_electrons=2.5,
+                    figsize=(11, 8.5), label_size='medium'):
     """Plot simulation output tables for a single fiber.
 
     This function is normally called via :meth:`Simulator.plot` but is provided
     separately so that plots can be generated from results saved to a file.
 
     Use :meth:`show <matplotlib.pyplot.show` and :meth:`savefig
     <matplotlib.pyplot.savefig>` to show or save the resulting plot.
@@ -575,14 +681,18 @@
     simulated : astropy.table.Table
         Simulation results on the high-resolution simulation wavelength grid.
     camera_output : list
         Lists of tables of per-camera simulation results tabulated on each
         camera's output pixel grid.
     fiber : int
         Fiber index to plot.
+    wavelength_min : quantity or None
+        Clip the plot below this wavelength, or show the full extent.
+    wavelength_max : quantity or None
+        Clip the plot above this wavelength, or show the full extent.
     title : str or None
         Descriptive title to use for the plot.
     min_electrons : float
         Minimum y-axis value for displaying numbers of detected electrons.
     figsize : tuple
         Tuple (width, height) specifying the figure size to use in inches.
         See :meth:`matplotlib.pyplot.subplots` for details.
@@ -590,26 +700,70 @@
     import matplotlib.pyplot as plt
     from matplotlib.patches import Rectangle
 
     fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=figsize, sharex=True)
     if title is not None:
         ax1.set_title(title)
 
-    wave = simulated['wavelength']
-    dwave = np.gradient(wave)
-    waveunit = '{0:Generic}'.format(wave.unit)
+    waveunit = '{0:Generic}'.format(simulated['wavelength'].unit)
     fluxunit = '{0:Generic}'.format(simulated['source_flux'].unit)
+    wave = simulated['wavelength'].data
+    dwave = np.gradient(wave)
+
+    # Validate the optional wavelength limits and convert to waveunit.
+    def validate(name, limit):
+        if limit is None:
+            return limit
+        try:
+            return limit.to(waveunit).value
+        except AttributeError:
+            raise ValueError('Missing unit for {0}.'.format(name))
+        except u.UnitConversionError:
+            raise ValueError('Invalid unit for {0}.'.format(name))
+    wavelength_min = validate('wavelength_min', wavelength_min)
+    wavelength_max = validate('wavelength_max', wavelength_max)
+    if wavelength_min and wavelength_max and wavelength_min >= wavelength_max:
+        raise ValueError('Expected wavelength_min < wavelength_max.')
+
+    # Create a helper function that returns a slice that limits the
+    # wavelength array w (with units) to wavelenth_min <= w <= wavelength_max.
+    # Returns None if all w < wavelength_min or all w > wavelength_max.
+    def get_slice(w):
+        assert np.all(np.diff(w) > 0)
+        if wavelength_min is None:
+            start = 0
+        elif wavelength_min > w[-1]:
+            return None
+        else:
+            start = np.where(w >= wavelength_min)[0][0]
+        if wavelength_max is None:
+            stop = len(w)
+        elif wavelength_max < w[0]:
+            return None
+        else:
+            stop = np.where(w <= wavelength_max)[0][-1] + 1
+        return slice(start, stop)
+
+    # Trim the full wavelength grid.
+    waves = get_slice(wave)
+    if waves is None:
+        raise ValueError('Wavelength limits do not overlap simulation grid.')
+    wave = wave[waves]
+    dwave = dwave[waves]
 
     # Plot fluxes above the atmosphere and into the fiber.
 
-    src_flux = simulated['source_flux'][:, fiber]
-    src_fiber_flux = simulated['source_fiber_flux'][:, fiber]
-    sky_fiber_flux = simulated['sky_fiber_flux'][:, fiber]
+    src_flux = simulated['source_flux'][waves, fiber]
+    src_fiber_flux = simulated['source_fiber_flux'][waves, fiber]
+    sky_fiber_flux = simulated['sky_fiber_flux'][waves, fiber]
 
     ymin, ymax = 0.1 * np.min(src_flux), 10. * np.max(src_flux)
+    if ymin <= 0:
+        # Need ymin > 0 for log scale.
+        ymin = 1e-3 * ymax
 
     line, = ax1.plot(wave, src_flux, 'r-')
     ax1.fill_between(wave, src_fiber_flux + sky_fiber_flux,
                      ymin, color='b', alpha=0.2, lw=0)
     ax1.fill_between(wave, src_fiber_flux, ymin, color='r', alpha=0.2, lw=0)
 
     # This kludge is because the label arg to fill_between() does not
@@ -623,16 +777,16 @@
 
     ax1.set_ylim(ymin, ymax)
     ax1.set_yscale('log')
     ax1.set_ylabel('Flux [{0}]'.format(fluxunit))
 
     # Plot numbers of photons into the fiber.
 
-    nsky = simulated['num_sky_photons'][:, fiber] / dwave
-    nsrc = simulated['num_source_photons'][:, fiber] / dwave
+    nsky = simulated['num_sky_photons'][waves, fiber] / dwave
+    nsrc = simulated['num_source_photons'][waves, fiber] / dwave
     nmax = np.max(nsrc)
 
     ax2.fill_between(wave, nsky + nsrc, 1e-1 * nmax, color='b', alpha=0.2, lw=0)
     ax2.fill_between(wave, nsrc, 1e-1 * nmax, color='r', alpha=0.2, lw=0)
 
     ax2.legend(
         (sky_fill, src_fill),
@@ -644,47 +798,58 @@
     ax2.set_ylabel('Mean photons / {0}'.format(waveunit))
     ax2.set_xlim(wave[0], wave[-1])
 
     # Plot numbers of electrons detected by each CCD.
 
     for output in camera_output:
 
-        cwave = output['wavelength']
+        cwave = output['wavelength'].data
         dwave = np.gradient(cwave)
-        nsky = output['num_sky_electrons'][:, fiber] / dwave
-        nsrc = output['num_source_electrons'][:, fiber] / dwave
-        ndark = output['num_dark_electrons'][:, fiber] / dwave
-        read_noise = output['read_noise_electrons'][:, fiber] / np.sqrt(dwave)
-        total_noise = np.sqrt(output['variance_electrons'][:, fiber] / dwave)
+        # Trim to requested wavelength range.
+        waves = get_slice(cwave)
+        if waves is None:
+            # Skip any cameras outside the requested wavelength range.
+            continue
+        cwave = cwave[waves]
+        dwave = dwave[waves]
+        nsky = output['num_sky_electrons'][waves, fiber] / dwave
+        nsrc = output['num_source_electrons'][waves, fiber] / dwave
+        ndark = output['num_dark_electrons'][waves, fiber] / dwave
+        read_noise = (
+            output['read_noise_electrons'][waves, fiber] / np.sqrt(dwave))
+        total_noise = (
+            np.sqrt(output['variance_electrons'][waves, fiber] / dwave))
         nmax = max(nmax, np.max(nsrc))
 
         ax3.fill_between(
             cwave, ndark + nsky + nsrc, min_electrons, color='b',
             alpha=0.2, lw=0)
         ax3.fill_between(
             cwave, ndark + nsrc, min_electrons, color='r', alpha=0.2, lw=0)
         ax3.fill_between(
             cwave, ndark, min_electrons, color='k', alpha=0.2, lw=0)
         ax3.scatter(cwave, total_noise, color='k', lw=0., s=0.5, alpha=0.5)
         line2, = ax3.plot(cwave, read_noise, color='k', ls='--', alpha=0.5)
 
-    # This kludge is because the label arg to fill_between() does not
-    # propagate to legend() in matplotlib < 1.5.
-    line1, = ax3.plot([], [], 'k-')
-    dark_fill = Rectangle((0, 0), 1, 1, fc='k', alpha=0.2)
-    ax3.legend(
-        (sky_fill, src_fill, dark_fill, line1, line2),
-        ('Sky detected', 'Source detected', 'Dark current',
-         'RMS total noise', 'RMS read noise'),
-        loc='best', fancybox=True, framealpha=0.5, ncol=5, fontsize=label_size)
-
-    ax3.set_ylim(min_electrons, 2e2 * min_electrons)
-    ax3.set_yscale('log')
-    ax3.set_ylabel('Mean electrons / {0}'.format(waveunit))
-    ax3.set_xlim(wave[0], wave[-1])
-    ax3.set_xlabel('Wavelength [{0}]'.format(waveunit))
+    if camera_output:
+        # This kludge is because the label arg to fill_between() does not
+        # propagate to legend() in matplotlib < 1.5.
+        line1, = ax3.plot([], [], 'k-')
+        dark_fill = Rectangle((0, 0), 1, 1, fc='k', alpha=0.2)
+        ax3.legend(
+            (sky_fill, src_fill, dark_fill, line1, line2),
+            ('Sky detected', 'Source detected', 'Dark current',
+             'RMS total noise', 'RMS read noise'),
+            loc='best', fancybox=True, framealpha=0.5, ncol=5,
+            fontsize=label_size)
+
+        ax3.set_ylim(min_electrons, 2e2 * min_electrons)
+        ax3.set_yscale('log')
+        ax3.set_ylabel('Mean electrons / {0}'.format(waveunit))
+        ax3.set_xlim(wave[0], wave[-1])
+        ax3.set_xlabel('Wavelength [{0}]'.format(waveunit))
 
     # Remove x-axis ticks on the upper panels.
     plt.setp([a.get_xticklabels() for a in fig.axes[:-1]], visible=False)
 
     fig.patch.set_facecolor('white')
     plt.tight_layout()
```

### Comparing `specsim-0.8/specsim/source.py` & `specsim-0.9/specsim/source.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/coveragerc` & `specsim-0.9/specsim/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_atmosphere.py` & `specsim-0.9/specsim/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_config.py` & `specsim-0.9/specsim/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_fiberloss.py` & `specsim-0.9/specsim/tests/test_fiberloss.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_instrument.py` & `specsim-0.9/specsim/tests/test_instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,7 +20,13 @@
     i.plot()
 
 
 def test_distortion_plot():
     c = specsim.config.load_config('test')
     i = initialize(c)
     i.plot_field_distortion()
+
+
+def test_no_cameras():
+    c = specsim.config.load_config('test')
+    i = initialize(c, camera_output=False)
+    i.plot()
```

### Comparing `specsim-0.8/specsim/tests/test_observation.py` & `specsim-0.9/specsim/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_simulator.py` & `specsim-0.9/specsim/tests/test_simulator.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,38 @@
 def test_ctor():
     config = specsim.config.load_config('test')
     sim1 = Simulator(config)
     sim2 = Simulator('test')
     assert sim1.atmosphere.airmass == sim2.atmosphere.airmass
 
 
+def test_alt_wavelengths():
+    config = specsim.config.load_config('test')
+    config.wavelength_grid.step = 0.1
+    config.instrument.cameras.r.constants.output_pixel_size = "1.2 Angstrom"
+    sim = Simulator(config)
+    sim.simulate()
+    assert np.allclose(np.diff(sim.camera_output[0]['wavelength']), 1.2)
+
+    config.instrument.cameras.r.constants.output_pixel_size = "0.4 Angstrom"
+    sim = Simulator(config)
+    sim.simulate()
+    assert np.allclose(np.diff(sim.camera_output[0]['wavelength']), 0.4)
+
+    config.instrument.cameras.r.constants.output_pixel_size = "0.3 Angstrom"
+    sim = Simulator(config)
+    sim.simulate()
+    assert np.allclose(np.diff(sim.camera_output[0]['wavelength']), 0.3)
+
+    config.wavelength_grid.step = 0.2
+    config.instrument.cameras.r.constants.output_pixel_size = "0.2 Angstrom"
+    sim = Simulator(config)
+    sim.simulate()
+    assert np.allclose(np.diff(sim.camera_output[0]['wavelength']), 0.2)
+
 def test_end_to_end():
     sim = Simulator('test')
     sim.simulate()
     nsrc = sim.simulated['num_source_electrons_r'][:, 0].sum()
     assert np.allclose(nsrc, 86996.4478)
 
 
@@ -82,11 +106,33 @@
     assert np.allclose(sim.focal_y.to(u.mm).value, 1.)
     # Check that sky_positions has the next highest priority.
     sim.simulate(sky_positions=sky)
     assert np.allclose(sim.focal_x.to(u.mm).value, 0.)
     assert np.allclose(sim.focal_y.to(u.mm).value, 0.)
 
 
+def test_output_table_units():
+    """Test that units are preserved after calling simulate().
+
+    This test was added in response to issue #62
+    """
+    sim = specsim.simulator.Simulator('test', num_fibers=1)
+    units_before = {}
+    for table in (sim.simulated, sim.camera_output[0]):
+        for name in table.colnames:
+            units_before[name] = table[name].unit
+    sim.simulate()
+    for table in (sim.simulated, sim.camera_output[0]):
+        for name in table.colnames:
+            assert units_before[name] == table[name].unit
+
+
 def test_plot():
     s = Simulator('test')
     s.simulate()
     s.plot()
+
+
+def test_no_cameras():
+    s = Simulator('test', camera_output=False)
+    s.simulate()
+    s.plot()
```

### Comparing `specsim-0.8/specsim/tests/test_source.py` & `specsim-0.9/specsim/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/tests/test_transform.py` & `specsim-0.9/specsim/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/transform.py` & `specsim-0.9/specsim/transform.py`

 * *Files identical despite different names*

### Comparing `specsim-0.8/specsim/version.py` & `specsim-0.9/specsim/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Autogenerated by Astropy-affiliated package specsim's setup.py on 2017-03-25 09:30:23.789054
+# Autogenerated by Astropy-affiliated package specsim's setup.py on 2017-05-11 13:39:57.442508
 from __future__ import unicode_literals
 import datetime
 
 
 import locale
 import os
 import subprocess
@@ -177,16 +177,16 @@
             break
 
         current_dir = os.path.dirname(current_dir)
 
     return None
 
 _packagename = "specsim"
-_last_generated_version = "0.8"
-_last_githash = "80955ee9381cd38812a78a2936ce98fdf6e0e46c"
+_last_generated_version = "0.9"
+_last_githash = "defa3d86a2606ffde181a1bfbf815528d33946eb"
 
 # Determine where the source code for this module
 # lives.  If __file__ is not a filesystem path then
 # it is assumed not to live in a git repo at all.
 if _get_repo_path(__file__, levels=len(_packagename.split('.'))):
     version = update_git_devstr(_last_generated_version, path=__file__)
     githash = get_git_devstr(sha=True, show_warning=False,
@@ -195,19 +195,19 @@
     # The file does not appear to live in a git repo so don't bother
     # invoking git
     version = _last_generated_version
     githash = _last_githash
 
 
 major = 0
-minor = 8
+minor = 9
 bugfix = 0
 
 release = True
-timestamp = datetime.datetime(2017, 3, 25, 9, 30, 23, 789054)
+timestamp = datetime.datetime(2017, 5, 11, 13, 39, 57, 442508)
 debug = False
 
 try:
     from ._compiler import compiler
 except ImportError:
     compiler = "unknown"
```

