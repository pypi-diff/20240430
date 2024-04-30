# Comparing `tmp/skilleter_thingy-0.0.27.tar.gz` & `tmp/skilleter_thingy-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.27.tar", last modified: Fri Apr 26 08:31:33 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.28.tar", last modified: Tue Apr 30 15:35:29 2024, max compression
```

## Comparing `skilleter_thingy-0.0.27.tar` & `skilleter_thingy-0.0.28.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-26 08:31:33.284222 skilleter_thingy-0.0.27/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-26 08:31:33.284222 skilleter_thingy-0.0.27/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-04-26 08:31:15.000000 skilleter_thingy-0.0.27/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-26 08:31:33.284222 skilleter_thingy-0.0.27/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-26 08:31:33.276222 skilleter_thingy-0.0.27/skilleter_thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/__init__.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/addpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/borger.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/colour.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/console_colours.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/dc_curses.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/dc_defaults.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/dc_util.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/dircolors.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/diskspacecheck.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/docker.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/docker_purge.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/ffind.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/files.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/ggit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/ggrep.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    37887 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git2.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_br.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_ca.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_cleanup.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_co.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_common.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_hold.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_mr.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_parent.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    51566 2024-04-26 08:14:08.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_review.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_update.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/git_wt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/gitcmp_helper.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/gitlab.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/gitprompt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/gl.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/gphotosync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/linecount.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/logger.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/moviemover.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/path.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-04-22 10:33:30.000000 skilleter_thingy-0.0.27/skilleter_thingy/photodupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/phototidier.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/popup.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/process.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/py_audit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     9487 2024-04-26 08:30:25.000000 skilleter_thingy-0.0.27/skilleter_thingy/readable.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/remdir.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/rmdupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/rpylint.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/run.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/splitpics.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/strreplace.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/sysmon.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/tfm.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/tfm_pane.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/tfparse.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/tidy.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/trimpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/window_rename.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/xchmod.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.27/skilleter_thingy/yamlcheck.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-26 08:31:33.284222 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     1960 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-26 08:31:33.000000 skilleter_thingy-0.0.27/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-04-30 15:33:43.000000 skilleter_thingy-0.0.28/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/skilleter_thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/__init__.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/addpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/borger.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/colour.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/console_colours.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_curses.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_defaults.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_util.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dircolors.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/diskspacecheck.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/docker.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/docker_purge.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ffind.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/files.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ggit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ggrep.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    38049 2024-04-30 15:33:22.000000 skilleter_thingy-0.0.28/skilleter_thingy/git.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git2.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_br.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_ca.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_cleanup.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_co.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_common.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_hold.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_mr.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_parent.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    51796 2024-04-30 15:35:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_review.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_update.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_wt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitcmp_helper.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitlab.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitprompt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gl.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gphotosync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/linecount.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/logger.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/moviemover.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/path.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-04-22 10:33:30.000000 skilleter_thingy-0.0.28/skilleter_thingy/photodupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/phototidier.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/popup.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/process.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/py_audit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9487 2024-04-26 08:30:25.000000 skilleter_thingy-0.0.28/skilleter_thingy/readable.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/remdir.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/rmdupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/rpylint.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/run.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/splitpics.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/strreplace.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/sysmon.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfm.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfm_pane.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfparse.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tidy.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/trimpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/window_rename.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/xchmod.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/yamlcheck.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1960 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/top_level.txt
```

### Comparing `skilleter_thingy-0.0.27/LICENSE` & `skilleter_thingy-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/PKG-INFO` & `skilleter_thingy-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.27
+Version: 0.0.28
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.27/README.md` & `skilleter_thingy-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/pyproject.toml` & `skilleter_thingy-0.0.28/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skilleter_thingy"
 
 # Version must be incremented to install updated Thingy
 
-version = "0.0.27"
+version = "0.0.28"
 
 authors = [
     {name="John Skilleter", email="john@skilleter.org.uk"},
 ]
 
 description = "A collection of useful utilities, mainly aimed at making Git more friendly"
```

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/addpath.py` & `skilleter_thingy-0.0.28/skilleter_thingy/addpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/borger.py` & `skilleter_thingy-0.0.28/skilleter_thingy/borger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/colour.py` & `skilleter_thingy-0.0.28/skilleter_thingy/colour.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/console_colours.py` & `skilleter_thingy-0.0.28/skilleter_thingy/console_colours.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/dc_curses.py` & `skilleter_thingy-0.0.28/skilleter_thingy/dc_curses.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/dc_defaults.py` & `skilleter_thingy-0.0.28/skilleter_thingy/dc_defaults.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/dc_util.py` & `skilleter_thingy-0.0.28/skilleter_thingy/dc_util.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/dircolors.py` & `skilleter_thingy-0.0.28/skilleter_thingy/dircolors.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/diskspacecheck.py` & `skilleter_thingy-0.0.28/skilleter_thingy/diskspacecheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/docker.py` & `skilleter_thingy-0.0.28/skilleter_thingy/docker.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/docker_purge.py` & `skilleter_thingy-0.0.28/skilleter_thingy/docker_purge.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/ffind.py` & `skilleter_thingy-0.0.28/skilleter_thingy/ffind.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/files.py` & `skilleter_thingy-0.0.28/skilleter_thingy/files.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/ggit.py` & `skilleter_thingy-0.0.28/skilleter_thingy/ggit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/ggrep.py` & `skilleter_thingy-0.0.28/skilleter_thingy/ggrep.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,16 +527,18 @@
 
         p = re.fullmatch(r'(-|\d+)\s+(-|\d+)\s+(.*)', result)
 
         lines_ins = 0 if p.group(1) == '-' else int(p.group(1))
         lines_del = 0 if p.group(2) == '-' else int(p.group(2))
 
         if ' => ' in p.group(3):
+            filepath = p.group(3).split('{')[0]
             filename = p.group(3).split(' => ')[1]
             filename = filename.replace('}', '')
+            filename = os.path.join(filepath, filename)
         else:
             filename = p.group(3)
 
         return filename, lines_ins, lines_del
 
     # Either get changes between the two commits, or changes in the specified commit
 
@@ -577,14 +579,15 @@
             filestatus, filename = result.split('\t')
             info[filename] = {'status': filestatus[0], 'oldname': filename}
 
     # Add the diff stats, if requested
 
     if diff_stats:
         # Run git diff to get stats, and add them to the info
+        # TODO: Need to extract old name of renamed files
 
         results = git(['diff', '--numstat'] + params)
 
         for result in results:
             filename, lines_ins, lines_del = parse_diff_output(result)
 
             info[filename]['deleted'] = lines_del
```

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git2.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git2.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_br.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_br.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_ca.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_ca.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_cleanup.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_cleanup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_co.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_co.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_common.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_common.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_hold.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_hold.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_mr.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_mr.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_parent.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_parent.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_review.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         * Think that maintaining the list of files as a dictionary may be better than a list
         * Filter in/out new/deleted files
         * Universal filter dialog replace individual optins and allow selection of:
             * Show:  all / deleted / updated files
             * Show:  all / wildcard match / wildcard non-match
             * Show:  all / reviewed / unreviewed files
         * Tag files for group operations (reset, delete, add, commit)
+        * Handle renamed files properly - need to show old and new names, but need to return this info from git.commit_info()
 
     BUGS:
-        * Fails to handle renamed files -thinks it a file called 'oldname => newname'
         * If console window is too small, popups aren't displayed - should handle this better - scrollable popup?
         * Switching between hiding reviewed files and not does not maintain cursor position
         * In hide mode, ins should not move down
         * "r" resets reviewed status for all files to False
         * If all reviewed then hidden, then move cursor around empty screen then unhide first redraw has blank line at the top.
         * Need better way of handling panels - does not cope with resize when one is active - help sort-of does,
           but doesn't pass the refrefsh down when closing - need flag for it
@@ -1269,25 +1269,31 @@
 
     parser = argparse.ArgumentParser(description='Menu-driven Git code review tool')
 
     parser.add_argument('-c', '--commit', type=str, help='Compare the specified commit with its parent')
     parser.add_argument('-b', '--branch', type=str, help='Compare the specified commit to branch point on specified branch')
     parser.add_argument('-C', '--change', action='store_true', help='Compare the current commit with its parent')
     parser.add_argument('-d', '--debug', action='store_true', help='Start a debug session over Telnet using pudb')
+    parser.add_argument('--dir', action='store', help='Work in the specified directory')
     parser.add_argument('--difftool', type=str, default=None, help='Override the default git diff tool')
 
     parser.add_argument('commits', nargs='*', help='Commit(s) or paths to compare')
 
     args = parser.parse_args()
 
     args.paths = None
 
     if args.debug:
         from pudb.remote import set_trace
         set_trace()
+        
+    # Move to a new directory, if required
+    
+    if args.dir:
+        os.chdir(args.dir)
 
     # Make sure that we're actually in a git working tree
 
     if not git.working_tree():
         colour.error(f'[RED:ERROR] Not a git repository')
 
     # -C/--change is shorthand for '--commit HEAD^'
```

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_update.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_update.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/git_wt.py` & `skilleter_thingy-0.0.28/skilleter_thingy/git_wt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/gitcmp_helper.py` & `skilleter_thingy-0.0.28/skilleter_thingy/gitcmp_helper.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/gitlab.py` & `skilleter_thingy-0.0.28/skilleter_thingy/gitlab.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/gitprompt.py` & `skilleter_thingy-0.0.28/skilleter_thingy/gitprompt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/gl.py` & `skilleter_thingy-0.0.28/skilleter_thingy/gl.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/gphotosync.py` & `skilleter_thingy-0.0.28/skilleter_thingy/gphotosync.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/linecount.py` & `skilleter_thingy-0.0.28/skilleter_thingy/linecount.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/logger.py` & `skilleter_thingy-0.0.28/skilleter_thingy/logger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/moviemover.py` & `skilleter_thingy-0.0.28/skilleter_thingy/moviemover.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/path.py` & `skilleter_thingy-0.0.28/skilleter_thingy/path.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/photodupe.py` & `skilleter_thingy-0.0.28/skilleter_thingy/photodupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/phototidier.py` & `skilleter_thingy-0.0.28/skilleter_thingy/phototidier.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/popup.py` & `skilleter_thingy-0.0.28/skilleter_thingy/popup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/process.py` & `skilleter_thingy-0.0.28/skilleter_thingy/process.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/py_audit.py` & `skilleter_thingy-0.0.28/skilleter_thingy/py_audit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/readable.py` & `skilleter_thingy-0.0.28/skilleter_thingy/readable.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/remdir.py` & `skilleter_thingy-0.0.28/skilleter_thingy/remdir.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/rmdupe.py` & `skilleter_thingy-0.0.28/skilleter_thingy/rmdupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/rpylint.py` & `skilleter_thingy-0.0.28/skilleter_thingy/rpylint.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/run.py` & `skilleter_thingy-0.0.28/skilleter_thingy/run.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/splitpics.py` & `skilleter_thingy-0.0.28/skilleter_thingy/splitpics.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/strreplace.py` & `skilleter_thingy-0.0.28/skilleter_thingy/strreplace.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/sysmon.py` & `skilleter_thingy-0.0.28/skilleter_thingy/sysmon.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/tfm.py` & `skilleter_thingy-0.0.28/skilleter_thingy/tfm.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/tfm_pane.py` & `skilleter_thingy-0.0.28/skilleter_thingy/tfm_pane.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/tfparse.py` & `skilleter_thingy-0.0.28/skilleter_thingy/tfparse.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/tidy.py` & `skilleter_thingy-0.0.28/skilleter_thingy/tidy.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/trimpath.py` & `skilleter_thingy-0.0.28/skilleter_thingy/trimpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/window_rename.py` & `skilleter_thingy-0.0.28/skilleter_thingy/window_rename.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/xchmod.py` & `skilleter_thingy-0.0.28/skilleter_thingy/xchmod.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy/yamlcheck.py` & `skilleter_thingy-0.0.28/skilleter_thingy/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.27
+Version: 0.0.28
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy.egg-info/SOURCES.txt` & `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.27/skilleter_thingy.egg-info/entry_points.txt` & `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/entry_points.txt`

 * *Files identical despite different names*

