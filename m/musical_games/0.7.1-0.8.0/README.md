# Comparing `tmp/musical_games-0.7.1.tar.gz` & `tmp/musical_games-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.7.1.tar` & `musical_games-0.8.0.tar`

### file list

```diff
@@ -1,105 +1,114 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.7.1/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.7.1/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.7.1/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.7.1/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.7.1/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.7.1/.travis.yml
--rw-r--r--   0        0        0     1225 2024-04-19 09:45:47.861062 musical_games-0.7.1/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.7.1/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.7.1/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.7.1/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.7.1/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.7.1/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.7.1/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.7.1/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.7.1/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      624 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2047 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2796 2024-04-18 10:49:11.595361 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3765 2024-04-18 10:49:11.583361 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.7.1/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    44061 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.7.1/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    15379 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.7.1/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.7.1/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.7.1/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-04-19 09:45:26.253062 musical_games-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.7.1/scripts/__init__.py
--rw-r--r--   0        0        0     9431 2024-04-16 05:05:56.478852 musical_games-0.7.1/scripts/copy_bars.py
--rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_stadler_meneut_trio.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.7.1/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.0/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.0/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.0/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.0/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.0/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.0/.travis.yml
+-rw-r--r--   0        0        0     1368 2024-04-30 09:20:18.554865 musical_games-0.8.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.0/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.0/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.0/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.0/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      624 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2386 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6417 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4232 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      814 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1012 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    30414 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2047 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2796 2024-04-18 10:49:11.595361 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3765 2024-04-18 10:49:11.583361 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.0/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    44061 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.0/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    18171 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.0/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.0/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.0/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-04-30 09:20:18.434865 musical_games-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.0/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     3441 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/lilypond_copy2.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.0/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.0/PKG-INFO
```

### Comparing `musical_games-0.7.1/.gitchangelog.rc` & `musical_games-0.8.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/.gitignore` & `musical_games-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/CHANGELOG.rst` & `musical_games-0.8.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 *********
 Changelog
 *********
 
+v0.8.0 (2024-04-30)
+===================
+
+Added
+-----
+- Adds Gerlach's Scottish Dance. Might need some more work concerning the clef changes.
+
+
 v0.7.1 (2024-04-19)
 ===================
 
 Added
 -----
 - Adds functionality for rendering a single dice table element.
 - Adds support for dice games selecting multiple measures per dice throw.
```

### Comparing `musical_games-0.7.1/LICENSE` & `musical_games-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/Makefile` & `musical_games-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/README.rst` & `musical_games-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/Makefile` & `musical_games-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/conf.py` & `musical_games-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/contributing.rst` & `musical_games-0.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/index.rst` & `musical_games-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/make.bat` & `musical_games-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/musical_games.converters.rst` & `musical_games-0.8.0/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.0/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/musical_games.dice_games.rst` & `musical_games-0.8.0/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/docs/musical_games.rst` & `musical_games-0.8.0/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/__version__.py` & `musical_games-0.8.0/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/dice_games/base.py` & `musical_games-0.8.0/musical_games/dice_games/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/dice_games/data_csv.py` & `musical_games-0.8.0/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/dice_games/dice_games.py` & `musical_games-0.8.0/musical_games/dice_games/dice_games.py`

 * *Files 17% similar despite different names*

```diff
@@ -268,7 +268,51 @@
             {'menuet': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'menuet': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
              'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Stadler', 'Menuet and Trio', dice_tables, bar_collections,
                          jinja2_environment, midi_settings)
+
+
+class GerlachScottishDance(SimpleDiceGame):
+
+    def __init__(self):
+        """Implementation of a Scottish dance dice game by Gerlach."""
+        dice_tables = {
+            'dance': SimpleDiceTable.from_lists([
+                [(65, 14), (29, 17), (108, 96), (37, 50), (41, 35), (92, 139), (49, 90), (11, 59)],
+                [(77, 109), (9, 28), (48, 99), (21, 7), (6, 80), (1, 47), (107, 31), (127, 51)],
+                [(15, 87), (55, 95), (144, 74), (104, 120), (130, 100), (71, 150), (111, 69), (72, 102)],
+                [(89, 12), (75, 3), (66, 175), (20, 70), (149, 46), (117, 94), (19, 86), (128, 52)],
+                [(40, 98), (36, 10), (78, 44), (33, 136), (39, 110), (143, 30), (58, 67), (22, 91)],
+                [(8, 88), (101, 32), (60, 4), (106, 93), (105, 45), (112, 27), (61, 119), (103, 48)]]),
+            'trio': SimpleDiceTable.from_lists([
+                [(13, 85), (126, 180), (125, 68), (177, 192), (187, 63), (24, 97), (145, 185), (137, 176)],
+                [(165, 113), (23, 76), (82, 2), (154, 190), (5, 84), (161, 182), (174, 116), (54, 124)],
+                [(43, 57), (135, 188), (56, 18), (189, 163), (25, 38), (166, 122), (179, 123), (169, 53)],
+                [(181, 129), (131, 186), (115, 170), (62, 178), (183, 132), (168, 171), (81, 151), (158, 64)],
+                [(134, 26), (118, 184), (160, 140), (114, 34), (42, 164), (146, 83), (141, 162), (73, 153)],
+                [(79, 191), (121, 155), (138, 156), (16, 173), (133, 167), (142, 172), (147, 159), (152, 157)]]),
+        }
+
+        csv_reader = SimpleBarCollectionCSVReader()
+        bars = csv_reader.read_csv(resources.files('musical_games') /
+                                   'data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv')
+
+        bar_collections = {'dance': bars,
+                           'trio': bars}
+
+        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/gerlach_scottish_dance/lilypond')
+        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
+        jinja2_environment = jinja2.Environment(**env_options)
+
+        midi_settings = SimpleMidiSettings(
+            {'dance': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
+             'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
+            {'dance': {'piano_right_hand': 0, 'piano_left_hand': 0},
+             'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
+            {'dance': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
+             'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
+
+        super().__init__('Gerlach', 'Scottish dance', dice_tables, bar_collections,
+                         jinja2_environment, midi_settings)
```

### Comparing `musical_games-0.7.1/musical_games/external/base.py` & `musical_games-0.8.0/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/external/images.py` & `musical_games-0.8.0/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/external/lilypond.py` & `musical_games-0.8.0/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/external/midi_converters.py` & `musical_games-0.8.0/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/external/utils.py` & `musical_games-0.8.0/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/external/wav_converters.py` & `musical_games-0.8.0/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/musical_games/utils.py` & `musical_games-0.8.0/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/pyproject.toml` & `musical_games-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.7.1"
+version = "0.8.0"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.7.1/scripts/demo_cpe_bach.py` & `musical_games-0.8.0/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.0/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.0/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.0/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/scripts/demo_mozart_waltz.py` & `musical_games-0.8.0/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.0/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/tox.ini` & `musical_games-0.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.1/PKG-INFO` & `musical_games-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.7.1
+Version: 0.8.0
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

