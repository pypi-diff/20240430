# Comparing `tmp/xklb-2.6.9.tar.gz` & `tmp/xklb-2.7.5.tar.gz`

## Comparing `xklb-2.6.9.tar` & `xklb-2.7.5.tar`

### file list

```diff
@@ -1,132 +1,136 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.9/.gitattributes
--rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.9/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/__init__.py
--rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/db_playlists.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/history.py
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/lb.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/media_printer.py
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/readme.py
--rw-r--r--   0        0        0   119411 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/av.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/row_add.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/rss_add.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20339 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    20728 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/__init__.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/sample_hash.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/move_list.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/scatter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/big_dirs.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/christen.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/mount_stats.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/block.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/history.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/search.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/__init__.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/links_open.py
--rw-r--r--   0        0        0    23498 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/media_player.py
--rw-r--r--   0        0        0    19535 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/surf.py
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/extract_text.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/consts.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/devices.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/nums.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/objects.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/printing.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/strings.py
--rw-r--r--   0        0        0    22132 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.9/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.9/pyproject.toml
--rw-r--r--   0        0        0   159958 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/README.md
--rw-r--r--   0        0        0   163719 2020-02-02 00:00:00.000000 xklb-2.6.9/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.5/.gitattributes
+-rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.5/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/__init__.py
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/lb.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/media_printer.py
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/readme.py
+-rw-r--r--   0        0        0   112110 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/av.py
+-rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/rss_add.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/christen.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/big_dirs.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/surf.py
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17730 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/processes.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.5/.gitignore
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0   155846 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/README.md
+-rw-r--r--   0        0        0   159627 2020-02-02 00:00:00.000000 xklb-2.7.5/PKG-INFO
```

### Comparing `xklb-2.6.9/pdm.lock` & `xklb-2.7.5/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "deluxe", "test"]
 strategy = ["cross_platform"]
 lock_version = "4.4.1"
-content_hash = "sha256:b2b7a02304f39d3e9958315a1f0c3230799c9e4cda0d0f411634c2057b9b871a"
+content_hash = "sha256:7d9fa60cd7ac07570e6c3fce0302ead14f375fb6a7b90b4d427c7013a8498ee2"
 
 [[package]]
 name = "aiohttp"
-version = "3.9.4"
+version = "3.9.5"
 requires_python = ">=3.8"
 summary = "Async http client/server framework (asyncio)"
 dependencies = [
     "aiosignal>=1.1.2",
     "async-timeout<5.0,>=4.0; python_version < \"3.11\"",
     "attrs>=17.3.0",
     "frozenlist>=1.1.1",
     "multidict<7.0,>=4.5",
     "yarl<2.0,>=1.0",
 ]
 files = [
-    {file = "aiohttp-3.9.4-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:76d32588ef7e4a3f3adff1956a0ba96faabbdee58f2407c122dd45aa6e34f372"},
-    {file = "aiohttp-3.9.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:56181093c10dbc6ceb8a29dfeea1e815e1dfdc020169203d87fd8d37616f73f9"},
-    {file = "aiohttp-3.9.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c7a5b676d3c65e88b3aca41816bf72831898fcd73f0cbb2680e9d88e819d1e4d"},
-    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d1df528a85fb404899d4207a8d9934cfd6be626e30e5d3a5544a83dbae6d8a7e"},
-    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f595db1bceabd71c82e92df212dd9525a8a2c6947d39e3c994c4f27d2fe15b11"},
-    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9c0b09d76e5a4caac3d27752027fbd43dc987b95f3748fad2b924a03fe8632ad"},
-    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:689eb4356649ec9535b3686200b231876fb4cab4aca54e3bece71d37f50c1d13"},
-    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a3666cf4182efdb44d73602379a66f5fdfd5da0db5e4520f0ac0dcca644a3497"},
-    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:b65b0f8747b013570eea2f75726046fa54fa8e0c5db60f3b98dd5d161052004a"},
-    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a1885d2470955f70dfdd33a02e1749613c5a9c5ab855f6db38e0b9389453dce7"},
-    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:0593822dcdb9483d41f12041ff7c90d4d1033ec0e880bcfaf102919b715f47f1"},
-    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:47f6eb74e1ecb5e19a78f4a4228aa24df7fbab3b62d4a625d3f41194a08bd54f"},
-    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c8b04a3dbd54de6ccb7604242fe3ad67f2f3ca558f2d33fe19d4b08d90701a89"},
-    {file = "aiohttp-3.9.4-cp310-cp310-win32.whl", hash = "sha256:8a78dfb198a328bfb38e4308ca8167028920fb747ddcf086ce706fbdd23b2926"},
-    {file = "aiohttp-3.9.4-cp310-cp310-win_amd64.whl", hash = "sha256:e78da6b55275987cbc89141a1d8e75f5070e577c482dd48bd9123a76a96f0bbb"},
-    {file = "aiohttp-3.9.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:c111b3c69060d2bafc446917534150fd049e7aedd6cbf21ba526a5a97b4402a5"},
-    {file = "aiohttp-3.9.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:efbdd51872cf170093998c87ccdf3cb5993add3559341a8e5708bcb311934c94"},
-    {file = "aiohttp-3.9.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7bfdb41dc6e85d8535b00d73947548a748e9534e8e4fddd2638109ff3fb081df"},
-    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2bd9d334412961125e9f68d5b73c1d0ab9ea3f74a58a475e6b119f5293eee7ba"},
-    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:35d78076736f4a668d57ade00c65d30a8ce28719d8a42471b2a06ccd1a2e3063"},
-    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:824dff4f9f4d0f59d0fa3577932ee9a20e09edec8a2f813e1d6b9f89ced8293f"},
-    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:52b8b4e06fc15519019e128abedaeb56412b106ab88b3c452188ca47a25c4093"},
-    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:eae569fb1e7559d4f3919965617bb39f9e753967fae55ce13454bec2d1c54f09"},
-    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:69b97aa5792428f321f72aeb2f118e56893371f27e0b7d05750bcad06fc42ca1"},
-    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4d79aad0ad4b980663316f26d9a492e8fab2af77c69c0f33780a56843ad2f89e"},
-    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:d6577140cd7db19e430661e4b2653680194ea8c22c994bc65b7a19d8ec834403"},
-    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:9860d455847cd98eb67897f5957b7cd69fbcb436dd3f06099230f16a66e66f79"},
-    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:69ff36d3f8f5652994e08bd22f093e11cfd0444cea310f92e01b45a4e46b624e"},
-    {file = "aiohttp-3.9.4-cp311-cp311-win32.whl", hash = "sha256:e27d3b5ed2c2013bce66ad67ee57cbf614288bda8cdf426c8d8fe548316f1b5f"},
-    {file = "aiohttp-3.9.4-cp311-cp311-win_amd64.whl", hash = "sha256:d6a67e26daa686a6fbdb600a9af8619c80a332556245fa8e86c747d226ab1a1e"},
-    {file = "aiohttp-3.9.4-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:c5ff8ff44825736a4065d8544b43b43ee4c6dd1530f3a08e6c0578a813b0aa35"},
-    {file = "aiohttp-3.9.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d12a244627eba4e9dc52cbf924edef905ddd6cafc6513849b4876076a6f38b0e"},
-    {file = "aiohttp-3.9.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:dcad56c8d8348e7e468899d2fb3b309b9bc59d94e6db08710555f7436156097f"},
-    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4f7e69a7fd4b5ce419238388e55abd220336bd32212c673ceabc57ccf3d05b55"},
-    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4870cb049f10d7680c239b55428916d84158798eb8f353e74fa2c98980dcc0b"},
-    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3b2feaf1b7031ede1bc0880cec4b0776fd347259a723d625357bb4b82f62687b"},
-    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:939393e8c3f0a5bcd33ef7ace67680c318dc2ae406f15e381c0054dd658397de"},
-    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7d2334e387b2adcc944680bebcf412743f2caf4eeebd550f67249c1c3696be04"},
-    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:e0198ea897680e480845ec0ffc5a14e8b694e25b3f104f63676d55bf76a82f1a"},
-    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:e40d2cd22914d67c84824045861a5bb0fb46586b15dfe4f046c7495bf08306b2"},
-    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:aba80e77c227f4234aa34a5ff2b6ff30c5d6a827a91d22ff6b999de9175d71bd"},
-    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:fb68dc73bc8ac322d2e392a59a9e396c4f35cb6fdbdd749e139d1d6c985f2527"},
-    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:f3460a92638dce7e47062cf088d6e7663adb135e936cb117be88d5e6c48c9d53"},
-    {file = "aiohttp-3.9.4-cp312-cp312-win32.whl", hash = "sha256:32dc814ddbb254f6170bca198fe307920f6c1308a5492f049f7f63554b88ef36"},
-    {file = "aiohttp-3.9.4-cp312-cp312-win_amd64.whl", hash = "sha256:63f41a909d182d2b78fe3abef557fcc14da50c7852f70ae3be60e83ff64edba5"},
-    {file = "aiohttp-3.9.4.tar.gz", hash = "sha256:6ff71ede6d9a5a58cfb7b6fffc83ab5d4a63138276c771ac91ceaaddf5459644"},
+    {file = "aiohttp-3.9.5-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:fcde4c397f673fdec23e6b05ebf8d4751314fa7c24f93334bf1f1364c1c69ac7"},
+    {file = "aiohttp-3.9.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:5d6b3f1fabe465e819aed2c421a6743d8debbde79b6a8600739300630a01bf2c"},
+    {file = "aiohttp-3.9.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6ae79c1bc12c34082d92bf9422764f799aee4746fd7a392db46b7fd357d4a17a"},
+    {file = "aiohttp-3.9.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4d3ebb9e1316ec74277d19c5f482f98cc65a73ccd5430540d6d11682cd857430"},
+    {file = "aiohttp-3.9.5-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84dabd95154f43a2ea80deffec9cb44d2e301e38a0c9d331cc4aa0166fe28ae3"},
+    {file = "aiohttp-3.9.5-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c8a02fbeca6f63cb1f0475c799679057fc9268b77075ab7cf3f1c600e81dd46b"},
+    {file = "aiohttp-3.9.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c26959ca7b75ff768e2776d8055bf9582a6267e24556bb7f7bd29e677932be72"},
+    {file = "aiohttp-3.9.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:714d4e5231fed4ba2762ed489b4aec07b2b9953cf4ee31e9871caac895a839c0"},
+    {file = "aiohttp-3.9.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:e7a6a8354f1b62e15d48e04350f13e726fa08b62c3d7b8401c0a1314f02e3558"},
+    {file = "aiohttp-3.9.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:c413016880e03e69d166efb5a1a95d40f83d5a3a648d16486592c49ffb76d0db"},
+    {file = "aiohttp-3.9.5-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:ff84aeb864e0fac81f676be9f4685f0527b660f1efdc40dcede3c251ef1e867f"},
+    {file = "aiohttp-3.9.5-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:ad7f2919d7dac062f24d6f5fe95d401597fbb015a25771f85e692d043c9d7832"},
+    {file = "aiohttp-3.9.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:702e2c7c187c1a498a4e2b03155d52658fdd6fda882d3d7fbb891a5cf108bb10"},
+    {file = "aiohttp-3.9.5-cp310-cp310-win32.whl", hash = "sha256:67c3119f5ddc7261d47163ed86d760ddf0e625cd6246b4ed852e82159617b5fb"},
+    {file = "aiohttp-3.9.5-cp310-cp310-win_amd64.whl", hash = "sha256:471f0ef53ccedec9995287f02caf0c068732f026455f07db3f01a46e49d76bbb"},
+    {file = "aiohttp-3.9.5-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e0ae53e33ee7476dd3d1132f932eeb39bf6125083820049d06edcdca4381f342"},
+    {file = "aiohttp-3.9.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c088c4d70d21f8ca5c0b8b5403fe84a7bc8e024161febdd4ef04575ef35d474d"},
+    {file = "aiohttp-3.9.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:639d0042b7670222f33b0028de6b4e2fad6451462ce7df2af8aee37dcac55424"},
+    {file = "aiohttp-3.9.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f26383adb94da5e7fb388d441bf09c61e5e35f455a3217bfd790c6b6bc64b2ee"},
+    {file = "aiohttp-3.9.5-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:66331d00fb28dc90aa606d9a54304af76b335ae204d1836f65797d6fe27f1ca2"},
+    {file = "aiohttp-3.9.5-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4ff550491f5492ab5ed3533e76b8567f4b37bd2995e780a1f46bca2024223233"},
+    {file = "aiohttp-3.9.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f22eb3a6c1080d862befa0a89c380b4dafce29dc6cd56083f630073d102eb595"},
+    {file = "aiohttp-3.9.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a81b1143d42b66ffc40a441379387076243ef7b51019204fd3ec36b9f69e77d6"},
+    {file = "aiohttp-3.9.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f64fd07515dad67f24b6ea4a66ae2876c01031de91c93075b8093f07c0a2d93d"},
+    {file = "aiohttp-3.9.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:93e22add827447d2e26d67c9ac0161756007f152fdc5210277d00a85f6c92323"},
+    {file = "aiohttp-3.9.5-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:55b39c8684a46e56ef8c8d24faf02de4a2b2ac60d26cee93bc595651ff545de9"},
+    {file = "aiohttp-3.9.5-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:4715a9b778f4293b9f8ae7a0a7cef9829f02ff8d6277a39d7f40565c737d3771"},
+    {file = "aiohttp-3.9.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:afc52b8d969eff14e069a710057d15ab9ac17cd4b6753042c407dcea0e40bf75"},
+    {file = "aiohttp-3.9.5-cp311-cp311-win32.whl", hash = "sha256:b3df71da99c98534be076196791adca8819761f0bf6e08e07fd7da25127150d6"},
+    {file = "aiohttp-3.9.5-cp311-cp311-win_amd64.whl", hash = "sha256:88e311d98cc0bf45b62fc46c66753a83445f5ab20038bcc1b8a1cc05666f428a"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:c7a4b7a6cf5b6eb11e109a9755fd4fda7d57395f8c575e166d363b9fc3ec4678"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:0a158704edf0abcac8ac371fbb54044f3270bdbc93e254a82b6c82be1ef08f3c"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d153f652a687a8e95ad367a86a61e8d53d528b0530ef382ec5aaf533140ed00f"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:82a6a97d9771cb48ae16979c3a3a9a18b600a8505b1115cfe354dfb2054468b4"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:60cdbd56f4cad9f69c35eaac0fbbdf1f77b0ff9456cebd4902f3dd1cf096464c"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8676e8fd73141ded15ea586de0b7cda1542960a7b9ad89b2b06428e97125d4fa"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:da00da442a0e31f1c69d26d224e1efd3a1ca5bcbf210978a2ca7426dfcae9f58"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18f634d540dd099c262e9f887c8bbacc959847cfe5da7a0e2e1cf3f14dbf2daf"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:320e8618eda64e19d11bdb3bd04ccc0a816c17eaecb7e4945d01deee2a22f95f"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:2faa61a904b83142747fc6a6d7ad8fccff898c849123030f8e75d5d967fd4a81"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:8c64a6dc3fe5db7b1b4d2b5cb84c4f677768bdc340611eca673afb7cf416ef5a"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:393c7aba2b55559ef7ab791c94b44f7482a07bf7640d17b341b79081f5e5cd1a"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:c671dc117c2c21a1ca10c116cfcd6e3e44da7fcde37bf83b2be485ab377b25da"},
+    {file = "aiohttp-3.9.5-cp312-cp312-win32.whl", hash = "sha256:5a7ee16aab26e76add4afc45e8f8206c95d1d75540f1039b84a03c3b3800dd59"},
+    {file = "aiohttp-3.9.5-cp312-cp312-win_amd64.whl", hash = "sha256:5ca51eadbd67045396bc92a4345d1790b7301c14d1848feaac1d6a6c9289e888"},
+    {file = "aiohttp-3.9.5.tar.gz", hash = "sha256:edea7d15772ceeb29db4aff55e482d4bcfb6ae160ce144f2682de02f6d693551"},
 ]
 
 [[package]]
 name = "aiosignal"
 version = "1.3.1"
 requires_python = ">=3.7"
 summary = "aiosignal: a list of registered asynchronous callbacks"
@@ -153,20 +153,20 @@
 files = [
     {file = "beautifulsoup4-4.12.3-py3-none-any.whl", hash = "sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed"},
     {file = "beautifulsoup4-4.12.3.tar.gz", hash = "sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051"},
 ]
 
 [[package]]
 name = "blinker"
-version = "1.7.0"
+version = "1.8.1"
 requires_python = ">=3.8"
 summary = "Fast, simple object-to-object and broadcast signaling"
 files = [
-    {file = "blinker-1.7.0-py3-none-any.whl", hash = "sha256:c3f865d4d54db7abc53758a01601cf343fe55b84c1de4e3fa910e420b438d5b9"},
-    {file = "blinker-1.7.0.tar.gz", hash = "sha256:e6820ff6fa4e4d1d8e2747c2283749c3f547e4fee112b98555cdcdae32996182"},
+    {file = "blinker-1.8.1-py3-none-any.whl", hash = "sha256:5f1cdeff423b77c31b89de0565cd03e5275a03028f44b2b15f912632a58cced6"},
+    {file = "blinker-1.8.1.tar.gz", hash = "sha256:da44ec748222dcd0105ef975eed946da197d5bdf8bafb6aa92f5bc89da63fa25"},
 ]
 
 [[package]]
 name = "brotli"
 version = "1.1.0"
 summary = "Python bindings for the Brotli compression library"
 files = [
@@ -619,20 +619,20 @@
 summary = "Python video metadata parser"
 files = [
     {file = "enzyme-0.4.1.tar.gz", hash = "sha256:f2167fa97c24d1103a94d4bf4eb20f00ca76c38a37499821049253b2059c62bb"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [[package]]
 name = "executing"
 version = "2.0.1"
 requires_python = ">=3.5"
 summary = "Get the currently executing AST node of a frame, and other information"
@@ -727,23 +727,23 @@
     {file = "fonttools-4.51.0-cp312-cp312-win_amd64.whl", hash = "sha256:b3c61423f22165541b9403ee39874dcae84cd57a9078b82e1dce8cb06b07fa2e"},
     {file = "fonttools-4.51.0-py3-none-any.whl", hash = "sha256:15c94eeef6b095831067f72c825eb0e2d48bb4cea0647c1b05c981ecba2bf39f"},
     {file = "fonttools-4.51.0.tar.gz", hash = "sha256:dc0673361331566d7a663d7ce0f6fdcbfbdc1f59c6e3ed1165ad7202ca183c68"},
 ]
 
 [[package]]
 name = "freezegun"
-version = "1.4.0"
+version = "1.5.0"
 requires_python = ">=3.7"
 summary = "Let your Python tests travel through time"
 dependencies = [
     "python-dateutil>=2.7",
 ]
 files = [
-    {file = "freezegun-1.4.0-py3-none-any.whl", hash = "sha256:55e0fc3c84ebf0a96a5aa23ff8b53d70246479e9a68863f1fcac5a3e52f19dd6"},
-    {file = "freezegun-1.4.0.tar.gz", hash = "sha256:10939b0ba0ff5adaecf3b06a5c2f73071d9678e507c5eaedb23c761d56ac774b"},
+    {file = "freezegun-1.5.0-py3-none-any.whl", hash = "sha256:ec3f4ba030e34eb6cf7e1e257308aee2c60c3d038ff35996d7475760c9ff3719"},
+    {file = "freezegun-1.5.0.tar.gz", hash = "sha256:200a64359b363aa3653d8aac289584078386c7c3da77339d257e46a01fb5c77c"},
 ]
 
 [[package]]
 name = "frozenlist"
 version = "1.4.1"
 requires_python = ">=3.8"
 summary = "A list-like structure which implements collections.abc.MutableSequence"
@@ -831,27 +831,28 @@
 files = [
     {file = "gallery_dl-1.26.9-py3-none-any.whl", hash = "sha256:cbfce457778a5339e888bca78d339b119318252f0feead6a4cd9b93884738008"},
     {file = "gallery_dl-1.26.9.tar.gz", hash = "sha256:3e06dfa69c890a9805ba90509e0f0c50f8a16c39a2b780bec569d2cc2272bb99"},
 ]
 
 [[package]]
 name = "geopandas"
-version = "0.14.3"
+version = "0.14.4"
 requires_python = ">=3.9"
 summary = "Geographic pandas extensions"
 dependencies = [
     "fiona>=1.8.21",
+    "numpy>=1.22",
     "packaging",
     "pandas>=1.4.0",
     "pyproj>=3.3.0",
     "shapely>=1.8.0",
 ]
 files = [
-    {file = "geopandas-0.14.3-py3-none-any.whl", hash = "sha256:41b31ad39e21bc9e8c4254f78f8dc4ce3d33d144e22e630a00bb336c83160204"},
-    {file = "geopandas-0.14.3.tar.gz", hash = "sha256:748af035d4a068a4ae00cab384acb61d387685c833b0022e0729aa45216b23ac"},
+    {file = "geopandas-0.14.4-py3-none-any.whl", hash = "sha256:3bb6473cb59d51e1a7fe2dbc24a1a063fb0ebdeddf3ce08ddbf8c7ddc99689aa"},
+    {file = "geopandas-0.14.4.tar.gz", hash = "sha256:56765be9d58e2c743078085db3bd07dc6be7719f0dbe1dfdc1d705cb80be7c25"},
 ]
 
 [[package]]
 name = "guessit"
 version = "3.8.0"
 summary = "GuessIt - a library for guessing information from video filenames."
 dependencies = [
@@ -945,33 +946,33 @@
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "ipython"
-version = "8.23.0"
+version = "8.24.0"
 requires_python = ">=3.10"
 summary = "IPython: Productive Interactive Computing"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "decorator",
     "exceptiongroup; python_version < \"3.11\"",
     "jedi>=0.16",
     "matplotlib-inline",
     "pexpect>4.3; sys_platform != \"win32\" and sys_platform != \"emscripten\"",
     "prompt-toolkit<3.1.0,>=3.0.41",
     "pygments>=2.4.0",
     "stack-data",
     "traitlets>=5.13.0",
-    "typing-extensions; python_version < \"3.12\"",
+    "typing-extensions>=4.6; python_version < \"3.12\"",
 ]
 files = [
-    {file = "ipython-8.23.0-py3-none-any.whl", hash = "sha256:07232af52a5ba146dc3372c7bf52a0f890a23edf38d77caef8d53f9cdc2584c1"},
-    {file = "ipython-8.23.0.tar.gz", hash = "sha256:7468edaf4f6de3e1b912e57f66c241e6fd3c7099f2ec2136e239e142e800274d"},
+    {file = "ipython-8.24.0-py3-none-any.whl", hash = "sha256:d7bf2f6c4314984e3e02393213bab8703cf163ede39672ce5918c51fe253a2a3"},
+    {file = "ipython-8.24.0.tar.gz", hash = "sha256:010db3f8a728a578bb641fdd06c063b9fb8e96a9464c63aec6310fbcb5e80501"},
 ]
 
 [[package]]
 name = "jedi"
 version = "0.19.1"
 requires_python = ">=3.6"
 summary = "An autocompletion tool for Python that can be used for text editors."
@@ -1069,14 +1070,110 @@
     {file = "kiwisolver-1.4.5-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:85267bd1aa8880a9c88a8cb71e18d3d64d2751a790e6ca6c27b8ccc724bcd5ad"},
     {file = "kiwisolver-1.4.5-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:210ef2c3a1f03272649aff1ef992df2e724748918c4bc2d5a90352849eb40bea"},
     {file = "kiwisolver-1.4.5-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:11d011a7574eb3b82bcc9c1a1d35c1d7075677fdd15de527d91b46bd35e935ee"},
     {file = "kiwisolver-1.4.5.tar.gz", hash = "sha256:e57e563a57fb22a142da34f38acc2fc1a5c864bc29ca1517a88abc963e60d6ec"},
 ]
 
 [[package]]
+name = "lxml"
+version = "5.2.1"
+requires_python = ">=3.6"
+summary = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
+files = [
+    {file = "lxml-5.2.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1"},
+    {file = "lxml-5.2.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_28_ppc64le.whl", hash = "sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_28_s390x.whl", hash = "sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a"},
+    {file = "lxml-5.2.1-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_2_aarch64.whl", hash = "sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_2_ppc64le.whl", hash = "sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_2_s390x.whl", hash = "sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01"},
+    {file = "lxml-5.2.1-cp310-cp310-musllinux_1_2_x86_64.whl", hash = "sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1"},
+    {file = "lxml-5.2.1-cp310-cp310-win32.whl", hash = "sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5"},
+    {file = "lxml-5.2.1-cp310-cp310-win_amd64.whl", hash = "sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f"},
+    {file = "lxml-5.2.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867"},
+    {file = "lxml-5.2.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_28_ppc64le.whl", hash = "sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_28_s390x.whl", hash = "sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a"},
+    {file = "lxml-5.2.1-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_2_aarch64.whl", hash = "sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_2_ppc64le.whl", hash = "sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_2_s390x.whl", hash = "sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f"},
+    {file = "lxml-5.2.1-cp311-cp311-musllinux_1_2_x86_64.whl", hash = "sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534"},
+    {file = "lxml-5.2.1-cp311-cp311-win32.whl", hash = "sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be"},
+    {file = "lxml-5.2.1-cp311-cp311-win_amd64.whl", hash = "sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102"},
+    {file = "lxml-5.2.1-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851"},
+    {file = "lxml-5.2.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_28_aarch64.whl", hash = "sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_28_ppc64le.whl", hash = "sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_28_s390x.whl", hash = "sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0"},
+    {file = "lxml-5.2.1-cp312-cp312-manylinux_2_28_x86_64.whl", hash = "sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_2_aarch64.whl", hash = "sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_2_ppc64le.whl", hash = "sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_2_s390x.whl", hash = "sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169"},
+    {file = "lxml-5.2.1-cp312-cp312-musllinux_1_2_x86_64.whl", hash = "sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4"},
+    {file = "lxml-5.2.1-cp312-cp312-win32.whl", hash = "sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134"},
+    {file = "lxml-5.2.1-cp312-cp312-win_amd64.whl", hash = "sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-macosx_10_9_x86_64.whl", hash = "sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e"},
+    {file = "lxml-5.2.1-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96"},
+    {file = "lxml-5.2.1-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85"},
+    {file = "lxml-5.2.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246"},
+    {file = "lxml-5.2.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704"},
+    {file = "lxml-5.2.1.tar.gz", hash = "sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306"},
+]
+
+[[package]]
 name = "markdown"
 version = "3.6"
 requires_python = ">=3.8"
 summary = "Python implementation of John Gruber's Markdown."
 files = [
     {file = "Markdown-3.6-py3-none-any.whl", hash = "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f"},
     {file = "Markdown-3.6.tar.gz", hash = "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"},
@@ -1134,23 +1231,23 @@
     {file = "matplotlib-3.8.4-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a0e47eda4eb2614300fc7bb4657fced3e83d6334d03da2173b09e447418d499f"},
     {file = "matplotlib-3.8.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:493e9f6aa5819156b58fce42b296ea31969f2aab71c5b680b4ea7a3cb5c07d94"},
     {file = "matplotlib-3.8.4.tar.gz", hash = "sha256:8aac397d5e9ec158960e31c381c5ffc52ddd52bd9a47717e2a694038167dffea"},
 ]
 
 [[package]]
 name = "matplotlib-inline"
-version = "0.1.6"
-requires_python = ">=3.5"
+version = "0.1.7"
+requires_python = ">=3.8"
 summary = "Inline Matplotlib backend for Jupyter"
 dependencies = [
     "traitlets",
 ]
 files = [
-    {file = "matplotlib-inline-0.1.6.tar.gz", hash = "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"},
-    {file = "matplotlib_inline-0.1.6-py3-none-any.whl", hash = "sha256:f1f41aab5328aa5aaea9b16d083b128102f8712542f819fe7e6a420ff581b311"},
+    {file = "matplotlib_inline-0.1.7-py3-none-any.whl", hash = "sha256:df192d39a4ff8f21b1895d72e6a13f5fcc5099f00fa84384e0ea28c2cc0653ca"},
+    {file = "matplotlib_inline-0.1.7.tar.gz", hash = "sha256:8423b23ec666be3d16e16b60bdd8ac4e86e840ebd1dd11a30b9f117f2fa0ab90"},
 ]
 
 [[package]]
 name = "mdurl"
 version = "0.1.2"
 requires_python = ">=3.7"
 summary = "Markdown URL utilities"
@@ -1304,14 +1401,15 @@
     "numpy>=1.26.0; python_version >= \"3.12\"",
     "python-dateutil>=2.8.2",
     "pytz>=2020.1",
     "tzdata>=2022.7",
 ]
 files = [
     {file = "pandas-2.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:90c6fca2acf139569e74e8781709dccb6fe25940488755716d1d354d6bc58bce"},
+    {file = "pandas-2.2.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c7adfc142dac335d8c1e0dcbd37eb8617eac386596eb9e1a1b77791cf2498238"},
     {file = "pandas-2.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4abfe0be0d7221be4f12552995e58723c7422c80a659da13ca382697de830c08"},
     {file = "pandas-2.2.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8635c16bf3d99040fdf3ca3db669a7250ddf49c55dc4aa8fe0ae0fa8d6dcc1f0"},
     {file = "pandas-2.2.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:40ae1dffb3967a52203105a077415a86044a2bea011b5f321c6aa64b379a3f51"},
     {file = "pandas-2.2.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8e5a0b00e1e56a842f922e7fae8ae4077aee4af0acb5ae3622bd4b4c30aedf99"},
     {file = "pandas-2.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:ddf818e4e6c7c6f4f7c8a12709696d193976b591cc7dc50588d3d1a6b5dc8772"},
     {file = "pandas-2.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:696039430f7a562b74fa45f540aca068ea85fa34c244d0deee539cb6d70aa288"},
     {file = "pandas-2.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8e90497254aacacbc4ea6ae5e7a8cd75629d6ad2b30025a4a8b09aa4faf55151"},
@@ -1416,20 +1514,20 @@
     {file = "pillow-10.3.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a"},
     {file = "pillow-10.3.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591"},
     {file = "pillow-10.3.0.tar.gz", hash = "sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d"},
 ]
 
 [[package]]
 name = "pluggy"
-version = "1.4.0"
+version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
 files = [
-    {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
-    {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [[package]]
 name = "praw"
 version = "7.7.1"
 requires_python = "~=3.7"
 summary = "PRAW, an acronym for \"Python Reddit API Wrapper\", is a Python package that allows for simple access to  Reddit's API."
@@ -1500,19 +1598,19 @@
 files = [
     {file = "pure_eval-0.2.2-py3-none-any.whl", hash = "sha256:01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350"},
     {file = "pure_eval-0.2.2.tar.gz", hash = "sha256:2b45320af6dfaa1750f543d714b6d1c520a1688dec6fd24d339063ce0aaa9ac3"},
 ]
 
 [[package]]
 name = "puremagic"
-version = "1.21"
+version = "1.22"
 summary = "Pure python implementation of magic file detection"
 files = [
-    {file = "puremagic-1.21-py3-none-any.whl", hash = "sha256:8fe85c05800fe1eacdd5aa943b9e7fdbee66bc41a17aacf80efd6c668c63df45"},
-    {file = "puremagic-1.21.tar.gz", hash = "sha256:31ef09b37a6ad2f7f2b09b5bd6b8c4a07187a01af4025f5f1368889bdfc6d779"},
+    {file = "puremagic-1.22-py3-none-any.whl", hash = "sha256:8cf3f0deb8230619ed987976cbbe7c4ebba0d19c3c26516d35085b87d23211df"},
+    {file = "puremagic-1.22.tar.gz", hash = "sha256:e584f00cfcc8096f54b092562df91580c3faa8b1599c36d5f9348e95254f2054"},
 ]
 
 [[package]]
 name = "pyasn1"
 version = "0.6.0"
 requires_python = ">=3.8"
 summary = "Pure-Python implementation of ASN.1 types and DER/BER/CER codecs (X.208)"
@@ -1730,28 +1828,28 @@
 files = [
     {file = "pysubs2-1.6.1-py3-none-any.whl", hash = "sha256:1f96d9dfb5f859a54a00e04621beb20ff21ea1d788821b2f4935c5c0ef8dc68e"},
     {file = "pysubs2-1.6.1.tar.gz", hash = "sha256:0261611e71735ff7763972c519c72593c8063efcb9039c54af65f31b81cec116"},
 ]
 
 [[package]]
 name = "pytest"
-version = "8.1.1"
+version = "8.2.0"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=1.4",
+    "pluggy<2.0,>=1.5",
     "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
-    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [[package]]
 name = "python-dateutil"
 version = "2.9.0.post0"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 summary = "Extensions to the standard Python datetime module"
@@ -1808,65 +1906,65 @@
 files = [
     {file = "rebulk-3.2.0-py3-none-any.whl", hash = "sha256:6bc31ae4b37200623c5827d2f539f9ec3e52b50431322dad8154642a39b0a53e"},
     {file = "rebulk-3.2.0.tar.gz", hash = "sha256:0d30bf80fca00fa9c697185ac475daac9bde5f646ce3338c9ff5d5dc1ebdfebc"},
 ]
 
 [[package]]
 name = "regex"
-version = "2023.12.25"
-requires_python = ">=3.7"
+version = "2024.4.28"
+requires_python = ">=3.8"
 summary = "Alternative regular expression module, to replace re."
 files = [
-    {file = "regex-2023.12.25-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:0694219a1d54336fd0445ea382d49d36882415c0134ee1e8332afd1529f0baa5"},
-    {file = "regex-2023.12.25-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:b014333bd0217ad3d54c143de9d4b9a3ca1c5a29a6d0d554952ea071cff0f1f8"},
-    {file = "regex-2023.12.25-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d865984b3f71f6d0af64d0d88f5733521698f6c16f445bb09ce746c92c97c586"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1e0eabac536b4cc7f57a5f3d095bfa557860ab912f25965e08fe1545e2ed8b4c"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c25a8ad70e716f96e13a637802813f65d8a6760ef48672aa3502f4c24ea8b400"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a9b6d73353f777630626f403b0652055ebfe8ff142a44ec2cf18ae470395766e"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9cc99d6946d750eb75827cb53c4371b8b0fe89c733a94b1573c9dd16ea6c9e4"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:88d1f7bef20c721359d8675f7d9f8e414ec5003d8f642fdfd8087777ff7f94b5"},
-    {file = "regex-2023.12.25-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:cb3fe77aec8f1995611f966d0c656fdce398317f850d0e6e7aebdfe61f40e1cd"},
-    {file = "regex-2023.12.25-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:7aa47c2e9ea33a4a2a05f40fcd3ea36d73853a2aae7b4feab6fc85f8bf2c9704"},
-    {file = "regex-2023.12.25-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:df26481f0c7a3f8739fecb3e81bc9da3fcfae34d6c094563b9d4670b047312e1"},
-    {file = "regex-2023.12.25-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:c40281f7d70baf6e0db0c2f7472b31609f5bc2748fe7275ea65a0b4601d9b392"},
-    {file = "regex-2023.12.25-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:d94a1db462d5690ebf6ae86d11c5e420042b9898af5dcf278bd97d6bda065423"},
-    {file = "regex-2023.12.25-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:ba1b30765a55acf15dce3f364e4928b80858fa8f979ad41f862358939bdd1f2f"},
-    {file = "regex-2023.12.25-cp310-cp310-win32.whl", hash = "sha256:150c39f5b964e4d7dba46a7962a088fbc91f06e606f023ce57bb347a3b2d4630"},
-    {file = "regex-2023.12.25-cp310-cp310-win_amd64.whl", hash = "sha256:09da66917262d9481c719599116c7dc0c321ffcec4b1f510c4f8a066f8768105"},
-    {file = "regex-2023.12.25-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:1b9d811f72210fa9306aeb88385b8f8bcef0dfbf3873410413c00aa94c56c2b6"},
-    {file = "regex-2023.12.25-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d902a43085a308cef32c0d3aea962524b725403fd9373dea18110904003bac97"},
-    {file = "regex-2023.12.25-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d166eafc19f4718df38887b2bbe1467a4f74a9830e8605089ea7a30dd4da8887"},
-    {file = "regex-2023.12.25-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c7ad32824b7f02bb3c9f80306d405a1d9b7bb89362d68b3c5a9be53836caebdb"},
-    {file = "regex-2023.12.25-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:636ba0a77de609d6510235b7f0e77ec494d2657108f777e8765efc060094c98c"},
-    {file = "regex-2023.12.25-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0fda75704357805eb953a3ee15a2b240694a9a514548cd49b3c5124b4e2ad01b"},
-    {file = "regex-2023.12.25-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f72cbae7f6b01591f90814250e636065850c5926751af02bb48da94dfced7baa"},
-    {file = "regex-2023.12.25-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:db2a0b1857f18b11e3b0e54ddfefc96af46b0896fb678c85f63fb8c37518b3e7"},
-    {file = "regex-2023.12.25-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:7502534e55c7c36c0978c91ba6f61703faf7ce733715ca48f499d3dbbd7657e0"},
-    {file = "regex-2023.12.25-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e8c7e08bb566de4faaf11984af13f6bcf6a08f327b13631d41d62592681d24fe"},
-    {file = "regex-2023.12.25-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:283fc8eed679758de38fe493b7d7d84a198b558942b03f017b1f94dda8efae80"},
-    {file = "regex-2023.12.25-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:f44dd4d68697559d007462b0a3a1d9acd61d97072b71f6d1968daef26bc744bd"},
-    {file = "regex-2023.12.25-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:67d3ccfc590e5e7197750fcb3a2915b416a53e2de847a728cfa60141054123d4"},
-    {file = "regex-2023.12.25-cp311-cp311-win32.whl", hash = "sha256:68191f80a9bad283432385961d9efe09d783bcd36ed35a60fb1ff3f1ec2efe87"},
-    {file = "regex-2023.12.25-cp311-cp311-win_amd64.whl", hash = "sha256:7d2af3f6b8419661a0c421584cfe8aaec1c0e435ce7e47ee2a97e344b98f794f"},
-    {file = "regex-2023.12.25-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:8a0ccf52bb37d1a700375a6b395bff5dd15c50acb745f7db30415bae3c2b0715"},
-    {file = "regex-2023.12.25-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:c3c4a78615b7762740531c27cf46e2f388d8d727d0c0c739e72048beb26c8a9d"},
-    {file = "regex-2023.12.25-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ad83e7545b4ab69216cef4cc47e344d19622e28aabec61574b20257c65466d6a"},
-    {file = "regex-2023.12.25-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b7a635871143661feccce3979e1727c4e094f2bdfd3ec4b90dfd4f16f571a87a"},
-    {file = "regex-2023.12.25-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d498eea3f581fbe1b34b59c697512a8baef88212f92e4c7830fcc1499f5b45a5"},
-    {file = "regex-2023.12.25-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:43f7cd5754d02a56ae4ebb91b33461dc67be8e3e0153f593c509e21d219c5060"},
-    {file = "regex-2023.12.25-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:51f4b32f793812714fd5307222a7f77e739b9bc566dc94a18126aba3b92b98a3"},
-    {file = "regex-2023.12.25-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ba99d8077424501b9616b43a2d208095746fb1284fc5ba490139651f971d39d9"},
-    {file = "regex-2023.12.25-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:4bfc2b16e3ba8850e0e262467275dd4d62f0d045e0e9eda2bc65078c0110a11f"},
-    {file = "regex-2023.12.25-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:8c2c19dae8a3eb0ea45a8448356ed561be843b13cbc34b840922ddf565498c1c"},
-    {file = "regex-2023.12.25-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:60080bb3d8617d96f0fb7e19796384cc2467447ef1c491694850ebd3670bc457"},
-    {file = "regex-2023.12.25-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:b77e27b79448e34c2c51c09836033056a0547aa360c45eeeb67803da7b0eedaf"},
-    {file = "regex-2023.12.25-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:518440c991f514331f4850a63560321f833979d145d7d81186dbe2f19e27ae3d"},
-    {file = "regex-2023.12.25-cp312-cp312-win32.whl", hash = "sha256:e2610e9406d3b0073636a3a2e80db05a02f0c3169b5632022b4e81c0364bcda5"},
-    {file = "regex-2023.12.25-cp312-cp312-win_amd64.whl", hash = "sha256:cc37b9aeebab425f11f27e5e9e6cf580be7206c6582a64467a14dda211abc232"},
-    {file = "regex-2023.12.25.tar.gz", hash = "sha256:29171aa128da69afdf4bde412d5bedc335f2ca8fcfe4489038577d05f16181e5"},
+    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd196d056b40af073d95a2879678585f0b74ad35190fac04ca67954c582c6b61"},
+    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8bb381f777351bd534462f63e1c6afb10a7caa9fa2a421ae22c26e796fe31b1f"},
+    {file = "regex-2024.4.28-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:47af45b6153522733aa6e92543938e97a70ce0900649ba626cf5aad290b737b6"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99d6a550425cc51c656331af0e2b1651e90eaaa23fb4acde577cf15068e2e20f"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bf29304a8011feb58913c382902fde3395957a47645bf848eea695839aa101b7"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:92da587eee39a52c91aebea8b850e4e4f095fe5928d415cb7ed656b3460ae79a"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6277d426e2f31bdbacb377d17a7475e32b2d7d1f02faaecc48d8e370c6a3ff31"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:28e1f28d07220c0f3da0e8fcd5a115bbb53f8b55cecf9bec0c946eb9a059a94c"},
+    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:aaa179975a64790c1f2701ac562b5eeb733946eeb036b5bcca05c8d928a62f10"},
+    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6f435946b7bf7a1b438b4e6b149b947c837cb23c704e780c19ba3e6855dbbdd3"},
+    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:19d6c11bf35a6ad077eb23852827f91c804eeb71ecb85db4ee1386825b9dc4db"},
+    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:fdae0120cddc839eb8e3c15faa8ad541cc6d906d3eb24d82fb041cfe2807bc1e"},
+    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:e672cf9caaf669053121f1766d659a8813bd547edef6e009205378faf45c67b8"},
+    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f57515750d07e14743db55d59759893fdb21d2668f39e549a7d6cad5d70f9fea"},
+    {file = "regex-2024.4.28-cp310-cp310-win32.whl", hash = "sha256:a1409c4eccb6981c7baabc8888d3550df518add6e06fe74fa1d9312c1838652d"},
+    {file = "regex-2024.4.28-cp310-cp310-win_amd64.whl", hash = "sha256:1f687a28640f763f23f8a9801fe9e1b37338bb1ca5d564ddd41619458f1f22d1"},
+    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:84077821c85f222362b72fdc44f7a3a13587a013a45cf14534df1cbbdc9a6796"},
+    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b45d4503de8f4f3dc02f1d28a9b039e5504a02cc18906cfe744c11def942e9eb"},
+    {file = "regex-2024.4.28-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:457c2cd5a646dd4ed536c92b535d73548fb8e216ebee602aa9f48e068fc393f3"},
+    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2b51739ddfd013c6f657b55a508de8b9ea78b56d22b236052c3a85a675102dc6"},
+    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:459226445c7d7454981c4c0ce0ad1a72e1e751c3e417f305722bbcee6697e06a"},
+    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:670fa596984b08a4a769491cbdf22350431970d0112e03d7e4eeaecaafcd0fec"},
+    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe00f4fe11c8a521b173e6324d862ee7ee3412bf7107570c9b564fe1119b56fb"},
+    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:36f392dc7763fe7924575475736bddf9ab9f7a66b920932d0ea50c2ded2f5636"},
+    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:23a412b7b1a7063f81a742463f38821097b6a37ce1e5b89dd8e871d14dbfd86b"},
+    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:f1d6e4b7b2ae3a6a9df53efbf199e4bfcff0959dbdb5fd9ced34d4407348e39a"},
+    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:499334ad139557de97cbc4347ee921c0e2b5e9c0f009859e74f3f77918339257"},
+    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:0940038bec2fe9e26b203d636c44d31dd8766abc1fe66262da6484bd82461ccf"},
+    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:66372c2a01782c5fe8e04bff4a2a0121a9897e19223d9eab30c54c50b2ebeb7f"},
+    {file = "regex-2024.4.28-cp311-cp311-win32.whl", hash = "sha256:c77d10ec3c1cf328b2f501ca32583625987ea0f23a0c2a49b37a39ee5c4c4630"},
+    {file = "regex-2024.4.28-cp311-cp311-win_amd64.whl", hash = "sha256:fc0916c4295c64d6890a46e02d4482bb5ccf33bf1a824c0eaa9e83b148291f90"},
+    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:08a1749f04fee2811c7617fdd46d2e46d09106fa8f475c884b65c01326eb15c5"},
+    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b8eb28995771c087a73338f695a08c9abfdf723d185e57b97f6175c5051ff1ae"},
+    {file = "regex-2024.4.28-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:dd7ef715ccb8040954d44cfeff17e6b8e9f79c8019daae2fd30a8806ef5435c0"},
+    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fb0315a2b26fde4005a7c401707c5352df274460f2f85b209cf6024271373013"},
+    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f2fc053228a6bd3a17a9b0a3f15c3ab3cf95727b00557e92e1cfe094b88cc662"},
+    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7fe9739a686dc44733d52d6e4f7b9c77b285e49edf8570754b322bca6b85b4cc"},
+    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74fcf77d979364f9b69fcf8200849ca29a374973dc193a7317698aa37d8b01c"},
+    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:965fd0cf4694d76f6564896b422724ec7b959ef927a7cb187fc6b3f4e4f59833"},
+    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:2fef0b38c34ae675fcbb1b5db760d40c3fc3612cfa186e9e50df5782cac02bcd"},
+    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:bc365ce25f6c7c5ed70e4bc674f9137f52b7dd6a125037f9132a7be52b8a252f"},
+    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:ac69b394764bb857429b031d29d9604842bc4cbfd964d764b1af1868eeebc4f0"},
+    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:144a1fc54765f5c5c36d6d4b073299832aa1ec6a746a6452c3ee7b46b3d3b11d"},
+    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:2630ca4e152c221072fd4a56d4622b5ada876f668ecd24d5ab62544ae6793ed6"},
+    {file = "regex-2024.4.28-cp312-cp312-win32.whl", hash = "sha256:7f3502f03b4da52bbe8ba962621daa846f38489cae5c4a7b5d738f15f6443d17"},
+    {file = "regex-2024.4.28-cp312-cp312-win_amd64.whl", hash = "sha256:0dd3f69098511e71880fb00f5815db9ed0ef62c05775395968299cb400aeab82"},
+    {file = "regex-2024.4.28.tar.gz", hash = "sha256:83ab366777ea45d58f72593adf35d36ca911ea8bd838483c1823b883a121b0e4"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 requires_python = ">=3.7"
 summary = "Python HTTP for Humans."
@@ -1893,35 +1991,35 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.3.7"
+version = "0.4.2"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 files = [
-    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:0e8377cccb2f07abd25e84fc5b2cbe48eeb0fea9f1719cad7caedb061d70e5ce"},
-    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:15a4d1cc1e64e556fa0d67bfd388fed416b7f3b26d5d1c3e7d192c897e39ba4b"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d28bdf3d7dc71dd46929fafeec98ba89b7c3550c3f0978e36389b5631b793663"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:379b67d4f49774ba679593b232dcd90d9e10f04d96e3c8ce4a28037ae473f7bb"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c060aea8ad5ef21cdfbbe05475ab5104ce7827b639a78dd55383a6e9895b7c51"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:ebf8f615dde968272d70502c083ebf963b6781aacd3079081e03b32adfe4d58a"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d48098bd8f5c38897b03604f5428901b65e3c97d40b3952e38637b5404b739a2"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:da8a4fda219bf9024692b1bc68c9cff4b80507879ada8769dc7e985755d662ea"},
-    {file = "ruff-0.3.7-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c44e0149f1d8b48c4d5c33d88c677a4aa22fd09b1683d6a7ff55b816b5d074f"},
-    {file = "ruff-0.3.7-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:3050ec0af72b709a62ecc2aca941b9cd479a7bf2b36cc4562f0033d688e44fa1"},
-    {file = "ruff-0.3.7-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:a29cc38e4c1ab00da18a3f6777f8b50099d73326981bb7d182e54a9a21bb4ff7"},
-    {file = "ruff-0.3.7-py3-none-musllinux_1_2_i686.whl", hash = "sha256:5b15cc59c19edca917f51b1956637db47e200b0fc5e6e1878233d3a938384b0b"},
-    {file = "ruff-0.3.7-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:e491045781b1e38b72c91247cf4634f040f8d0cb3e6d3d64d38dcf43616650b4"},
-    {file = "ruff-0.3.7-py3-none-win32.whl", hash = "sha256:bc931de87593d64fad3a22e201e55ad76271f1d5bfc44e1a1887edd0903c7d9f"},
-    {file = "ruff-0.3.7-py3-none-win_amd64.whl", hash = "sha256:5ef0e501e1e39f35e03c2acb1d1238c595b8bb36cf7a170e7c1df1b73da00e74"},
-    {file = "ruff-0.3.7-py3-none-win_arm64.whl", hash = "sha256:789e144f6dc7019d1f92a812891c645274ed08af6037d11fc65fcbc183b7d59f"},
-    {file = "ruff-0.3.7.tar.gz", hash = "sha256:d5c1aebee5162c2226784800ae031f660c350e7a3402c4d1f8ea4e97e232e3ba"},
+    {file = "ruff-0.4.2-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:8d14dc8953f8af7e003a485ef560bbefa5f8cc1ad994eebb5b12136049bbccc5"},
+    {file = "ruff-0.4.2-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:24016ed18db3dc9786af103ff49c03bdf408ea253f3cb9e3638f39ac9cf2d483"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0e2e06459042ac841ed510196c350ba35a9b24a643e23db60d79b2db92af0c2b"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3afabaf7ba8e9c485a14ad8f4122feff6b2b93cc53cd4dad2fd24ae35112d5c5"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:799eb468ea6bc54b95527143a4ceaf970d5aa3613050c6cff54c85fda3fde480"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:ec4ba9436a51527fb6931a8839af4c36a5481f8c19e8f5e42c2f7ad3a49f5069"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6a2243f8f434e487c2a010c7252150b1fdf019035130f41b77626f5655c9ca22"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8772130a063f3eebdf7095da00c0b9898bd1774c43b336272c3e98667d4fb8fa"},
+    {file = "ruff-0.4.2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6ab165ef5d72392b4ebb85a8b0fbd321f69832a632e07a74794c0e598e7a8376"},
+    {file = "ruff-0.4.2-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:1f32cadf44c2020e75e0c56c3408ed1d32c024766bd41aedef92aa3ca28eef68"},
+    {file = "ruff-0.4.2-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:22e306bf15e09af45ca812bc42fa59b628646fa7c26072555f278994890bc7ac"},
+    {file = "ruff-0.4.2-py3-none-musllinux_1_2_i686.whl", hash = "sha256:82986bb77ad83a1719c90b9528a9dd663c9206f7c0ab69282af8223566a0c34e"},
+    {file = "ruff-0.4.2-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:652e4ba553e421a6dc2a6d4868bc3b3881311702633eb3672f9f244ded8908cd"},
+    {file = "ruff-0.4.2-py3-none-win32.whl", hash = "sha256:7891ee376770ac094da3ad40c116258a381b86c7352552788377c6eb16d784fe"},
+    {file = "ruff-0.4.2-py3-none-win_amd64.whl", hash = "sha256:5ec481661fb2fd88a5d6cf1f83403d388ec90f9daaa36e40e2c003de66751798"},
+    {file = "ruff-0.4.2-py3-none-win_arm64.whl", hash = "sha256:cbd1e87c71bca14792948c4ccb51ee61c3296e164019d2d484f3eaa2d360dfaf"},
+    {file = "ruff-0.4.2.tar.gz", hash = "sha256:33bcc160aee2520664bc0859cfeaebc84bb7323becff3f303b8f1f2d81cb4edc"},
 ]
 
 [[package]]
 name = "scikit-learn"
 version = "1.4.2"
 requires_python = ">=3.9"
 summary = "A set of python modules for machine learning and data mining"
@@ -1992,27 +2090,27 @@
 files = [
     {file = "screeninfo-0.8.1-py3-none-any.whl", hash = "sha256:e97d6b173856edcfa3bd282f81deb528188aff14b11ec3e195584e7641be733c"},
     {file = "screeninfo-0.8.1.tar.gz", hash = "sha256:9983076bcc7e34402a1a9e4d7dabf3729411fd2abb3f3b4be7eba73519cd2ed1"},
 ]
 
 [[package]]
 name = "selenium"
-version = "4.19.0"
+version = "4.20.0"
 requires_python = ">=3.8"
 summary = ""
 dependencies = [
     "certifi>=2021.10.8",
     "trio-websocket~=0.9",
     "trio~=0.17",
     "typing-extensions>=4.9.0",
     "urllib3[socks]<3,>=1.26",
 ]
 files = [
-    {file = "selenium-4.19.0-py3-none-any.whl", hash = "sha256:5b4f49240d61e687a73f7968ae2517d403882aae3550eae2a229c745e619f1d9"},
-    {file = "selenium-4.19.0.tar.gz", hash = "sha256:d9dfd6d0b021d71d0a48b865fe7746490ba82b81e9c87b212360006629eb1853"},
+    {file = "selenium-4.20.0-py3-none-any.whl", hash = "sha256:b1d0c33b38ca27d0499183e48e1dd09ff26973481f5d3ef2983073813ae6588d"},
+    {file = "selenium-4.20.0.tar.gz", hash = "sha256:0bd564ee166980d419a8aaf4ac00289bc152afcf2eadca5efe8c8e36711853fd"},
 ]
 
 [[package]]
 name = "selenium-wire"
 version = "5.1.0"
 requires_python = ">=3.6"
 summary = "Extends Selenium to give you the ability to inspect requests made by the browser."
@@ -2043,43 +2141,43 @@
 summary = "Py3k port of sgmllib."
 files = [
     {file = "sgmllib3k-1.0.0.tar.gz", hash = "sha256:7868fb1c8bfa764c1ac563d3cf369c381d1325d36124933a726f29fcdaa812e9"},
 ]
 
 [[package]]
 name = "shapely"
-version = "2.0.3"
+version = "2.0.4"
 requires_python = ">=3.7"
 summary = "Manipulation and analysis of geometric objects"
 dependencies = [
-    "numpy<2,>=1.14",
+    "numpy<3,>=1.14",
 ]
 files = [
-    {file = "shapely-2.0.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:af7e9abe180b189431b0f490638281b43b84a33a960620e6b2e8d3e3458b61a1"},
-    {file = "shapely-2.0.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:98040462b36ced9671e266b95c326b97f41290d9d17504a1ee4dc313a7667b9c"},
-    {file = "shapely-2.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:71eb736ef2843f23473c6e37f6180f90f0a35d740ab284321548edf4e55d9a52"},
-    {file = "shapely-2.0.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:881eb9dbbb4a6419667e91fcb20313bfc1e67f53dbb392c6840ff04793571ed1"},
-    {file = "shapely-2.0.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f10d2ccf0554fc0e39fad5886c839e47e207f99fdf09547bc687a2330efda35b"},
-    {file = "shapely-2.0.3-cp310-cp310-win32.whl", hash = "sha256:6dfdc077a6fcaf74d3eab23a1ace5abc50c8bce56ac7747d25eab582c5a2990e"},
-    {file = "shapely-2.0.3-cp310-cp310-win_amd64.whl", hash = "sha256:64c5013dacd2d81b3bb12672098a0b2795c1bf8190cfc2980e380f5ef9d9e4d9"},
-    {file = "shapely-2.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:56cee3e4e8159d6f2ce32e421445b8e23154fd02a0ac271d6a6c0b266a8e3cce"},
-    {file = "shapely-2.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:619232c8276fded09527d2a9fd91a7885ff95c0ff9ecd5e3cb1e34fbb676e2ae"},
-    {file = "shapely-2.0.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b2a7d256db6f5b4b407dc0c98dd1b2fcf1c9c5814af9416e5498d0a2e4307a4b"},
-    {file = "shapely-2.0.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e45f0c8cd4583647db3216d965d49363e6548c300c23fd7e57ce17a03f824034"},
-    {file = "shapely-2.0.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13cb37d3826972a82748a450328fe02a931dcaed10e69a4d83cc20ba021bc85f"},
-    {file = "shapely-2.0.3-cp311-cp311-win32.whl", hash = "sha256:9302d7011e3e376d25acd30d2d9e70d315d93f03cc748784af19b00988fc30b1"},
-    {file = "shapely-2.0.3-cp311-cp311-win_amd64.whl", hash = "sha256:6b464f2666b13902835f201f50e835f2f153f37741db88f68c7f3b932d3505fa"},
-    {file = "shapely-2.0.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:e86e7cb8e331a4850e0c2a8b2d66dc08d7a7b301b8d1d34a13060e3a5b4b3b55"},
-    {file = "shapely-2.0.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:c91981c99ade980fc49e41a544629751a0ccd769f39794ae913e53b07b2f78b9"},
-    {file = "shapely-2.0.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:bd45d456983dc60a42c4db437496d3f08a4201fbf662b69779f535eb969660af"},
-    {file = "shapely-2.0.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:882fb1ffc7577e88c1194f4f1757e277dc484ba096a3b94844319873d14b0f2d"},
-    {file = "shapely-2.0.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b9f2d93bff2ea52fa93245798cddb479766a18510ea9b93a4fb9755c79474889"},
-    {file = "shapely-2.0.3-cp312-cp312-win32.whl", hash = "sha256:99abad1fd1303b35d991703432c9481e3242b7b3a393c186cfb02373bf604004"},
-    {file = "shapely-2.0.3-cp312-cp312-win_amd64.whl", hash = "sha256:6f555fe3304a1f40398977789bc4fe3c28a11173196df9ece1e15c5bc75a48db"},
-    {file = "shapely-2.0.3.tar.gz", hash = "sha256:4d65d0aa7910af71efa72fd6447e02a8e5dd44da81a983de9d736d6e6ccbe674"},
+    {file = "shapely-2.0.4-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:011b77153906030b795791f2fdfa2d68f1a8d7e40bce78b029782ade3afe4f2f"},
+    {file = "shapely-2.0.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9831816a5d34d5170aa9ed32a64982c3d6f4332e7ecfe62dc97767e163cb0b17"},
+    {file = "shapely-2.0.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5c4849916f71dc44e19ed370421518c0d86cf73b26e8656192fcfcda08218fbd"},
+    {file = "shapely-2.0.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:841f93a0e31e4c64d62ea570d81c35de0f6cea224568b2430d832967536308e6"},
+    {file = "shapely-2.0.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2b4431f522b277c79c34b65da128029a9955e4481462cbf7ebec23aab61fc58"},
+    {file = "shapely-2.0.4-cp310-cp310-win32.whl", hash = "sha256:92a41d936f7d6743f343be265ace93b7c57f5b231e21b9605716f5a47c2879e7"},
+    {file = "shapely-2.0.4-cp310-cp310-win_amd64.whl", hash = "sha256:30982f79f21bb0ff7d7d4a4e531e3fcaa39b778584c2ce81a147f95be1cd58c9"},
+    {file = "shapely-2.0.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:de0205cb21ad5ddaef607cda9a3191eadd1e7a62a756ea3a356369675230ac35"},
+    {file = "shapely-2.0.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7d56ce3e2a6a556b59a288771cf9d091470116867e578bebced8bfc4147fbfd7"},
+    {file = "shapely-2.0.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:58b0ecc505bbe49a99551eea3f2e8a9b3b24b3edd2a4de1ac0dc17bc75c9ec07"},
+    {file = "shapely-2.0.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:790a168a808bd00ee42786b8ba883307c0e3684ebb292e0e20009588c426da47"},
+    {file = "shapely-2.0.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4310b5494271e18580d61022c0857eb85d30510d88606fa3b8314790df7f367d"},
+    {file = "shapely-2.0.4-cp311-cp311-win32.whl", hash = "sha256:63f3a80daf4f867bd80f5c97fbe03314348ac1b3b70fb1c0ad255a69e3749879"},
+    {file = "shapely-2.0.4-cp311-cp311-win_amd64.whl", hash = "sha256:c52ed79f683f721b69a10fb9e3d940a468203f5054927215586c5d49a072de8d"},
+    {file = "shapely-2.0.4-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:5bbd974193e2cc274312da16b189b38f5f128410f3377721cadb76b1e8ca5328"},
+    {file = "shapely-2.0.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:41388321a73ba1a84edd90d86ecc8bfed55e6a1e51882eafb019f45895ec0f65"},
+    {file = "shapely-2.0.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0776c92d584f72f1e584d2e43cfc5542c2f3dd19d53f70df0900fda643f4bae6"},
+    {file = "shapely-2.0.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c75c98380b1ede1cae9a252c6dc247e6279403fae38c77060a5e6186c95073ac"},
+    {file = "shapely-2.0.4-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c3e700abf4a37b7b8b90532fa6ed5c38a9bfc777098bc9fbae5ec8e618ac8f30"},
+    {file = "shapely-2.0.4-cp312-cp312-win32.whl", hash = "sha256:4f2ab0faf8188b9f99e6a273b24b97662194160cc8ca17cf9d1fb6f18d7fb93f"},
+    {file = "shapely-2.0.4-cp312-cp312-win_amd64.whl", hash = "sha256:03152442d311a5e85ac73b39680dd64a9892fa42bb08fd83b3bab4fe6999bfa0"},
+    {file = "shapely-2.0.4.tar.gz", hash = "sha256:5dc736127fac70009b8d309a0eeb74f3e08979e530cf7017f2f507ef62e6cfb8"},
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
@@ -2204,20 +2302,20 @@
 files = [
     {file = "tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
     {file = "tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
 ]
 
 [[package]]
 name = "threadpoolctl"
-version = "3.4.0"
+version = "3.5.0"
 requires_python = ">=3.8"
 summary = "threadpoolctl"
 files = [
-    {file = "threadpoolctl-3.4.0-py3-none-any.whl", hash = "sha256:8f4c689a65b23e5ed825c8436a92b818aac005e0f3715f6a1664d7c7ee29d262"},
-    {file = "threadpoolctl-3.4.0.tar.gz", hash = "sha256:f11b491a03661d6dd7ef692dd422ab34185d982466c49c8f98c8f716b5c93196"},
+    {file = "threadpoolctl-3.5.0-py3-none-any.whl", hash = "sha256:56c1e26c150397e58c4926da8eeee87533b1e32bef131bd4bf6a2f45f3185467"},
+    {file = "threadpoolctl-3.5.0.tar.gz", hash = "sha256:082433502dd922bf738de0d8bcc4fdcbf0979ff44c42bd40f5af8a282f6fa107"},
 ]
 
 [[package]]
 name = "tinytag"
 version = "1.10.1"
 requires_python = ">=2.7"
 summary = "Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files"
@@ -2234,20 +2332,20 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "traitlets"
-version = "5.14.2"
+version = "5.14.3"
 requires_python = ">=3.8"
 summary = "Traitlets Python configuration system"
 files = [
-    {file = "traitlets-5.14.2-py3-none-any.whl", hash = "sha256:fcdf85684a772ddeba87db2f398ce00b40ff550d1528c03c14dbf6a02003cd80"},
-    {file = "traitlets-5.14.2.tar.gz", hash = "sha256:8cdd83c040dab7d1dee822678e5f5d100b514f7b72b01615b26fc5718916fdf9"},
+    {file = "traitlets-5.14.3-py3-none-any.whl", hash = "sha256:b74e89e397b1ed28cc831db7aea759ba6640cb3de13090ca145426688ff1ac4f"},
+    {file = "traitlets-5.14.3.tar.gz", hash = "sha256:9ed0579d3502c94b4b3732ac120375cda96f923114522847de4b3bb98b96b6b7"},
 ]
 
 [[package]]
 name = "trio"
 version = "0.25.0"
 requires_python = ">=3.8"
 summary = "A friendly Python library for async concurrency and I/O"
@@ -2344,20 +2442,20 @@
 files = [
     {file = "wcwidth-0.2.13-py2.py3-none-any.whl", hash = "sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859"},
     {file = "wcwidth-0.2.13.tar.gz", hash = "sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5"},
 ]
 
 [[package]]
 name = "websocket-client"
-version = "1.7.0"
+version = "1.8.0"
 requires_python = ">=3.8"
 summary = "WebSocket client for Python with low level API options"
 files = [
-    {file = "websocket-client-1.7.0.tar.gz", hash = "sha256:10e511ea3a8c744631d3bd77e61eb17ed09304c413ad42cf6ddfa4c7787e8fe6"},
-    {file = "websocket_client-1.7.0-py3-none-any.whl", hash = "sha256:f4c3d22fec12a2461427a29957ff07d35098ee2d976d3ba244e688b8b4057588"},
+    {file = "websocket_client-1.8.0-py3-none-any.whl", hash = "sha256:17b44cc997f5c498e809b22cdf2d9c7a9e71c02c8cc2b6c56e7c2d1239bfa526"},
+    {file = "websocket_client-1.8.0.tar.gz", hash = "sha256:3239df9f44da632f96012472805d40a23281a991027ce11d2f45a6f24ac4c3da"},
 ]
 
 [[package]]
 name = "websockets"
 version = "12.0"
 requires_python = ">=3.8"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
```

### Comparing `xklb-2.6.9/.github/LICENSE` & `xklb-2.7.5/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.github/Windows.md` & `xklb-2.7.5/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.github/examples/art.avif` & `xklb-2.7.5/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.github/examples/extract.svg` & `xklb-2.7.5/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.github/examples/tubeadd.svg` & `xklb-2.7.5/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.github/workflows/push.yaml` & `xklb-2.7.5/.github/workflows/push.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   test:
     strategy:
       fail-fast: false
       max-parallel: 8
       matrix:
-        nv: [ {os: windows-latest, py: "3.10"}, {os: macos-latest, py: "3.11"}, {os: ubuntu-latest, py: "3.12"} ]
+        nv: [ {os: windows-latest, py: "3.10"}, {os: macos-13, py: "3.11"}, {os: ubuntu-latest, py: "3.12"} ]
 
     runs-on: ${{ matrix.nv.os }}
     timeout-minutes: 20
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.nv.py }}
```

### Comparing `xklb-2.6.9/xklb/db_media.py` & `xklb-2.7.5/xklb/mediadb/db_media.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,14 +303,80 @@
         {'AND path not like "http%"' if args.local_media_only and 'time_downloaded' not in m_columns else ''}
         {'AND path like "http%"' if args.online_media_only and 'time_downloaded' not in m_columns else ''}
         {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only and 'time_downloaded' in m_columns else ''}
         {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only and 'time_downloaded' in m_columns else ''}
     """
 
 
+def natsort_media(args, media):
+    from natsort import natsorted, ns, os_sorted
+
+    reverse = False
+    if args.play_in_order.startswith("reverse_"):
+        args.play_in_order = args.play_in_order.replace("reverse_", "", 1)
+        reverse = True
+
+    compat = False
+    for opt in ("compat_", "nfkd_"):
+        if args.play_in_order.startswith(opt):
+            args.play_in_order = args.play_in_order.replace(opt, "", 1)
+            compat = True
+
+    if "_" in args.play_in_order:
+        alg, sort_key = args.play_in_order.split("_", 1)
+    else:
+        alg, sort_key = args.play_in_order, "ps"
+
+    def func_sort_key(sort_key):
+        def fn_key(d):
+            if sort_key in ("parent", "stem", "ps", "pts"):
+                path = Path(d["path"])
+
+                if sort_key == "parent":
+                    return path.parent
+                elif sort_key == "stem":
+                    return path.stem
+                elif sort_key == "ps":
+                    return (path.parent, path.stem)
+                else:  # sort_key == 'pts'
+                    return (path.parent, d["title"], path.stem)
+            else:
+                return d[sort_key]
+
+        return fn_key
+
+    media_sort_key = func_sort_key(sort_key)
+
+    NS_OPTS = ns.NUMAFTER | ns.NOEXP | ns.NANLAST
+    if compat:
+        NS_OPTS = NS_OPTS | ns.COMPATIBILITYNORMALIZE | ns.GROUPLETTERS
+
+    if alg == "natural":
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.DEFAULT, reverse=reverse)
+    elif alg in ("nspath", "path"):
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.PATH, reverse=reverse)
+    elif alg == "ignorecase":
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.IGNORECASE, reverse=reverse)
+    elif alg == "lowercase":
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.LOWERCASEFIRST, reverse=reverse)
+    elif alg in ("human", "locale"):
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.LOCALE, reverse=reverse)
+    elif alg == "signed":
+        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.REAL, reverse=reverse)
+    elif alg == "os":
+        media = os_sorted(media, key=media_sort_key, reverse=reverse)
+    elif alg == "python":
+        media = sorted(media, key=media_sort_key, reverse=reverse)
+    else:
+        media = natsorted(media, key=func_sort_key(alg), alg=NS_OPTS | ns.DEFAULT, reverse=reverse)
+
+    log.debug("natsort[0] %s", media[0:1])
+    return media
+
+
 def get_dir_media(args, dirs: Collection, include_subdirs=False, limit=2_000) -> list[dict]:
     if len(dirs) == 0:
         return processes.no_media_found()
 
     m_columns = db_utils.columns(args, "media")
 
     if include_subdirs:
@@ -342,16 +408,16 @@
                 {filter_paths}
             GROUP BY m.id, m.path
         )
         SELECT *
         FROM m
         ORDER BY play_count
             , m.path LIKE "http%"
-            {'' if 'sort' in args.defaults else ', ' + args.sort}
             , path
+            {'' if 'sort' in args.defaults else ', ' + args.sort}
         LIMIT {limit}
     """
 
     subpath_params = {f"subpath{i}": value + "%" for i, value in enumerate(dirs)}
 
     bindings = {**subpath_params}
     bindings = {**bindings, **{k: v for k, v in args.filter_bindings.items() if k.startswith("FTS")}}
@@ -362,107 +428,51 @@
         log.debug("dir_media dirs %s", dirs)
     else:
         log.debug("get_dir_media[0] %s", media[0:1])
 
     return media
 
 
+def get_next_dir_media(args, folder):
+    if args.play_in_order:
+        media = get_dir_media(args, [folder], limit=100)
+        media = natsort_media(args, media)
+        m = media[0:1]
+    else:
+        m = get_dir_media(args, [folder], limit=1)[0:1]
+    return m
+
+
 def get_sibling_media(args, media):
     if args.fetch_siblings in ("always", "all"):
         dirs = {str(Path(d["path"]).parent) + os.sep for d in media}
         media = get_dir_media(args, dirs)
     elif args.fetch_siblings == "each":
         parents = {str(Path(d["path"]).parent) + os.sep for d in media}
         media = []
         for parent in parents:
-            media.extend(get_dir_media(args, [parent], limit=1)[0:1])
+            media.extend(get_next_dir_media(args, parent))
     elif args.fetch_siblings == "if-audiobook":
         new_media = []
         seen = set()
         for d in media:
             if "audiobook" in d["path"].lower():
                 parent = str(Path(d["path"]).parent) + os.sep
                 if parent not in seen:
                     seen.add(parent)
-                    new_media.extend(get_dir_media(args, [parent], limit=1)[0:1])
+                    new_media.extend(get_next_dir_media(args, parent))
             else:
                 new_media.append(d)
         media = new_media
 
     # TODO: all-if>10, each-if=10 --lower --upper functionality could be replicated here
 
     return media
 
 
-def natsort_media(args, media):
-    from natsort import natsorted, ns, os_sorted
-
-    reverse = False
-    if args.play_in_order.startswith("reverse_"):
-        args.play_in_order = args.play_in_order.replace("reverse_", "", 1)
-        reverse = True
-
-    compat = False
-    for opt in ("compat_", "nfkd_"):
-        if args.play_in_order.startswith(opt):
-            args.play_in_order = args.play_in_order.replace(opt, "", 1)
-            compat = True
-
-    if "_" in args.play_in_order:
-        alg, sort_key = args.play_in_order.split("_", 1)
-    else:
-        alg, sort_key = args.play_in_order, "ps"
-
-    def func_sort_key(sort_key):
-        def fn_key(d):
-            if sort_key in ("parent", "stem", "ps", "pts"):
-                path = Path(d["path"])
-
-                if sort_key == "parent":
-                    return path.parent
-                elif sort_key == "stem":
-                    return path.stem
-                elif sort_key == "ps":
-                    return (path.parent, path.stem)
-                else:  # sort_key == 'pts'
-                    return (path.parent, d["title"], path.stem)
-            else:
-                return d[sort_key]
-
-        return fn_key
-
-    media_sort_key = func_sort_key(sort_key)
-
-    NS_OPTS = ns.NUMAFTER | ns.NOEXP | ns.NANLAST
-    if compat:
-        NS_OPTS = NS_OPTS | ns.COMPATIBILITYNORMALIZE | ns.GROUPLETTERS
-
-    if alg == "natural":
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.DEFAULT, reverse=reverse)
-    elif alg in ("nspath", "path"):
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.PATH, reverse=reverse)
-    elif alg == "ignorecase":
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.IGNORECASE, reverse=reverse)
-    elif alg == "lowercase":
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.LOWERCASEFIRST, reverse=reverse)
-    elif alg in ("human", "locale"):
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.LOCALE, reverse=reverse)
-    elif alg == "signed":
-        media = natsorted(media, key=media_sort_key, alg=NS_OPTS | ns.REAL, reverse=reverse)
-    elif alg == "os":
-        media = os_sorted(media, key=media_sort_key, reverse=reverse)
-    elif alg == "python":
-        media = sorted(media, key=media_sort_key, reverse=reverse)
-    else:
-        media = natsorted(media, key=func_sort_key(alg), alg=NS_OPTS | ns.DEFAULT, reverse=reverse)
-
-    log.debug("natsort[0] %s", media[0:1])
-    return media
-
-
 def get_related_media(args, m: dict) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     m_columns.update(rank=int)
 
     m = get(args, m["path"])
     words = set(
         iterables.conform(
```

### Comparing `xklb-2.6.9/xklb/db_playlists.py` & `xklb-2.7.5/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/lb.py` & `xklb-2.7.5/xklb/lb.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,22 @@
         "nouns": "Unstructured text -> compound nouns (stdin)",
     },
     "Folder subcommands": {
         "merge_folders": "Merge two or more file trees",
         "relmv": "Move files preserving parent folder hierarchy",
         "mv_list": "Find specific folders to move to different disks",
         "scatter": "Scatter files between folders or disks",
+        "mount_stats": "Show some relative mount stats",
+        "similar_folders": "Find similar folders based on folder name, size, and count",
     },
     "File subcommands": {
+        "christen": "Clean file paths",
         "sample_hash": "Calculate a hash based on small file segments",
         "sample_compare": "Compare files using sample-hash and other shortcuts",
+        "similar_files": "Find similar files based on filename",
     },
     "Tabular data subcommands": {
         "eda": "Exploratory Data Analysis on table-like files",
         "mcda": "Multi-criteria Ranking for Decision Support",
         "incremental_diff": "Diff large table-like files in chunks",
     },
     "Media File subcommands": {
@@ -50,27 +54,27 @@
         "process_image": "Shrink images by resizing and AV1 image format (.avif)",
     },
     "Multi-database subcommands": {
         "merge_dbs": "Merge SQLITE databases",
         "copy_play_counts": "Copy play history",
     },
     "Filesystem Database subcommands": {
-        "christen": "Clean filenames",
         "disk_usage": "Show disk usage",
-        "mount_stats": "Show some relative mount stats",
         "big_dirs": "Show large folders",
         "search_db": "Search a SQLITE database",
     },
     "Media Database subcommands": {
         "block": "Block a channel",
         "playlists": "List stored playlists",
         "download": "Download media",
         "download_status": "Show download status",
         "redownload": "Re-download deleted/lost media",
-        "history": "Show some playback statistics",
+        "history": "Show and manage playback history",
+        "history_add": "Add history from paths",
+        "stats": "Show some event statistics (created, deleted, watched, etc)",
         "search": "Search captions / subtitles",
         "optimize": "Re-optimize database",
     },
     "Playback subcommands": {
         "watch": "Watch / Listen",
         "now": "Show what is currently playing",
         "next": "Play next file and optionally delete current file",
@@ -192,29 +196,33 @@
     add_parser(subparsers, "xklb.createdb.web_add.web_update", ["web-dir-update"])
     add_parser(subparsers, "xklb.editdb.dedupe_db.dedupe_db", ["dedupe-dbs"])
     add_parser(subparsers, "xklb.editdb.dedupe_media.dedupe_media")
     add_parser(subparsers, "xklb.editdb.merge_online_local.merge_online_local")
     add_parser(subparsers, "xklb.editdb.mpv_watchlater.mpv_watchlater")
     add_parser(subparsers, "xklb.editdb.pushshift.pushshift_extract", ["pushshift"])
     add_parser(subparsers, "xklb.editdb.reddit_selftext.reddit_selftext")
+    add_parser(subparsers, "xklb.files.christen.christen")
     add_parser(subparsers, "xklb.files.sample_compare.sample_compare", ["cmp"])
     add_parser(subparsers, "xklb.files.sample_hash.sample_hash", ["hash", "hash-file"])
+    add_parser(subparsers, "xklb.files.similar_files.similar_files")
     add_parser(subparsers, "xklb.folders.merge_folders.merge_folders", ["merge-folder", "mv"])
     add_parser(subparsers, "xklb.folders.move_list.move_list", ["mv-list"])
     add_parser(subparsers, "xklb.folders.rel_mv.rel_mv", ["relmv", "mv-rel", "mvrel"])
     add_parser(subparsers, "xklb.folders.scatter.scatter")
+    add_parser(subparsers, "xklb.folders.similar_folders.similar_folders")
+    add_parser(subparsers, "xklb.folders.mount_stats.mount_stats", ["mu", "mount-usage"])
     add_parser(subparsers, "xklb.fsdb.big_dirs.big_dirs", ["large-folders"])
-    add_parser(subparsers, "xklb.fsdb.christen.christen")
     add_parser(subparsers, "xklb.fsdb.disk_usage.disk_usage", ["du", "usage"])
-    add_parser(subparsers, "xklb.fsdb.mount_stats.mount_stats", ["mu", "mount-usage"])
     add_parser(subparsers, "xklb.fsdb.search_db.search_db", ["s", "sdb", "search-dbs"])
     add_parser(subparsers, "xklb.mediadb.block.block")
     add_parser(subparsers, "xklb.mediadb.download.dl_download", ["dl", "download"])
     add_parser(subparsers, "xklb.mediadb.download_status.download_status", ["ds", "dl-status"])
     add_parser(subparsers, "xklb.mediadb.history.history", ["hi", "log"])
+    add_parser(subparsers, "xklb.mediadb.history_add.history_add", ["add-history"])
+    add_parser(subparsers, "xklb.mediadb.stats.stats")
     add_parser(subparsers, "xklb.mediadb.optimize_db.optimize_db", ["optimize"])
     add_parser(subparsers, "xklb.mediadb.playlists.playlists", ["pl", "folders"])
     add_parser(subparsers, "xklb.mediadb.redownload.redownload", ["re-dl", "re-download"])
     add_parser(subparsers, "xklb.mediadb.search.search", ["sc", "search-captions"])
     add_parser(subparsers, "xklb.mediafiles.media_check.media_check")
     add_parser(subparsers, "xklb.mediafiles.process_ffmpeg.process_ffmpeg", ["process-video", "process-audio"])
     add_parser(subparsers, "xklb.mediafiles.process_image.process_image")
```

### Comparing `xklb-2.6.9/xklb/media_printer.py` & `xklb-2.7.5/xklb/media_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 
 from tabulate import tabulate
 
-from xklb import db_media, history
+from xklb.mediadb import db_history, db_media
 from xklb.playback import post_actions
 from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def filter_deleted(media):
@@ -145,27 +145,29 @@
 
     else:
         # NOTE: when changing/moving this code be sure to preserve the behavior that -pa does not run the code
         if getattr(args, "delete_files", False):
             marked = post_actions.delete_media(args, [d["path"] for d in media])
             log.warning(f"Deleted {marked} files")
 
-        if getattr(args, "delete_rows", False) or "d" in print_args:
-            args.db["media"].delete_where("path = ?", [d["path"] for d in media])
+        if getattr(args, "delete_rows", False) or "D" in print_args:
+            with args.db.conn:
+                for d in media:
+                    args.db["media"].delete_where("path = ?", [d["path"]])
             log.warning(f"Deleted {len(media)} rows")
 
         if "r" in print_args:
             marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
             log.warning(f"Marked {marked} metadata records as deleted")
         elif getattr(args, "mark_deleted", False) or "d" in print_args:
             marked = db_media.mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
 
         if getattr(args, "mark_watched", False) or "w" in print_args:
-            marked = history.add(args, [d["path"] for d in media])
+            marked = db_history.add(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
     if (
         "a" not in print_args
         and "history" in tables
         and action == SC.download_status
         and "time_downloaded" in m_columns
@@ -208,26 +210,24 @@
             db_media.mark_media_deleted(args, deleted_paths)
             if len(media) == 0:
                 raise FileNotFoundError
 
         if not cols:
             cols = ["path"]
 
-        selected_cols = [{k: d.get(k, None) for k in cols} for d in media]
-        virtual_csv = StringIO()
-        wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
-        wr = csv.DictWriter(virtual_csv, fieldnames=cols)
-        wr.writerows(selected_cols)
-
-        virtual_csv.seek(0)
-        if getattr(args, "moved", False):
-            for line in virtual_csv.readlines():
-                printing.pipe_print(line.strip().replace(args.moved[0], "", 1))
-            moved_media(args, [d["path"] for d in media], *args.moved)
+        if len(cols) == 1:
+            printing.pipe_lines(d.get(cols[0], "") + "\n" for d in media)
         else:
+            selected_cols = [{k: d.get(k, None) for k in cols} for d in media]
+            virtual_csv = StringIO()
+            wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
+            wr = csv.DictWriter(virtual_csv, fieldnames=cols)
+            wr.writerows(selected_cols)
+
+            virtual_csv.seek(0)
             for line in virtual_csv.readlines():
                 printing.pipe_print(line.strip())
 
     elif "j" in print_args or consts.MOBILE_TERMINAL:
         print(json.dumps(media, indent=3))
     elif "c" in print_args:
         printing.write_csv_to_stdout(media)
@@ -243,15 +243,19 @@
 
         colalign = ["right" if should_align_right(k, v) else "left" for k, v in tbl[0].items()]
         print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False, colalign=colalign))
 
         if len(media) > 1:
             print(
                 f"{media_len or len(media)} {units}"
-                + (f" (limited by --limit {args.limit})" if args.limit and int(args.limit) <= len(media) else ""),
+                + (
+                    f" (limited by --limit {args.limit})"
+                    if args.limit and int(args.limit) <= len(media) and len(tbl) <= int(args.limit)
+                    else ""
+                ),
             )
 
         if duration > 0:
             duration = printing.human_duration(duration)
             if "a" not in print_args:
                 print("Total duration:", duration)
```

### Comparing `xklb-2.6.9/xklb/readme.py` & `xklb-2.7.5/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/usage.py` & `xklb-2.7.5/xklb/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,97 @@
+stats = """library stats DATABASE TIME_COLUMN
+
+    View watched stats
+
+        $ library stats video.db --completed
+        Finished watching:
+        ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
+        │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
+        ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
+        │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
+        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
+        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2023-01       │ 17 hours and 3.32 minutes       │ 15.27 minutes  │ 14.3 GB    │ 214.1 MB   │
+        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
+        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
+        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
+        ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
+
+    View download stats
+
+        $ library stats video.db time_downloaded --frequency daily
+        Downloaded media:
+        day         total_duration                          avg_duration                total_size    avg_size    count
+        ----------  --------------------------------------  ------------------------  ------------  ----------  -------
+        2023-08-11  1 month, 7 days and 8 hours             17 minutes                    192.2 GB     58.3 MB     3296
+        2023-08-12  18 days and 15 hours                    17 minutes                     89.7 GB     56.4 MB     1590
+        2023-08-14  13 days and 1 hours                     22 minutes                    111.2 GB    127.2 MB      874
+        2023-08-15  13 days and 6 hours                     17 minutes                    140.0 GB    126.7 MB     1105
+        2023-08-17  2 months, 8 days and 8 hours            19 minutes                    380.4 GB     72.6 MB     5243
+        2023-08-18  2 months, 30 days and 18 hours          17 minutes                    501.9 GB     63.3 MB     7926
+        2023-08-19  2 months, 6 days and 19 hours           19 minutes                    578.1 GB    110.6 MB     5229
+        2023-08-20  3 days and 9 hours                      6 minutes and 57 seconds       14.5 GB     20.7 MB      700
+        2023-08-21  4 days and 3 hours                      12 minutes                     18.0 GB     36.3 MB      495
+        2023-08-22  10 days and 8 hours                     17 minutes                     82.1 GB     91.7 MB      895
+        2023-08-23  19 days and 9 hours                     22 minutes                     93.7 GB     74.7 MB     1254
+
+        See also: library stats video.db time_downloaded -f daily --hide-deleted
+
+    View deleted stats
+
+        $ library stats video.db time_deleted
+        Deleted media:
+        ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+        │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+        ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+        │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
+        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+        │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
+        ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+        ╒════════════════════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤══════════════════╤════════════════╕
+        │ title_path                                                                                                 │ duration      │   subtitle_count │ time_deleted   │
+        ╞════════════════════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪══════════════════╪════════════════╡
+        │ Terminus (1987)                                                                                            │ 1 hour and    │                0 │ yesterday      │
+        │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
+        ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
+        │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
+        │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
+        ...
+
+
+    View time_modified stats
+
+        $ library stats example_dbs/web_add.image.db time_modified -f year
+        Time_Modified media:
+        year      total_size    avg_size    count
+        ------  ------------  ----------  -------
+        2010         4.4 MiB     1.5 MiB        3
+        2011       136.2 MiB    68.1 MiB        2
+        2013         1.6 GiB    10.7 MiB      154
+        2014         4.6 GiB    25.2 MiB      187
+        2015         4.3 GiB    26.5 MiB      167
+        2016         5.1 GiB    46.8 MiB      112
+        2017         4.8 GiB    51.7 MiB       95
+        2018         5.3 GiB    97.9 MiB       55
+        2019         1.3 GiB    46.5 MiB       29
+        2020        25.7 GiB   113.5 MiB      232
+        2021        25.6 GiB    96.5 MiB      272
+        2022        14.6 GiB    82.7 MiB      181
+        2023        24.3 GiB    72.5 MiB      343
+        2024        17.3 GiB   104.8 MiB      169
+        14 media
+"""
+
 download = r"""library download [--prefix /mnt/d/] [--safe] [--subs] [--auto-subs] [--small] DATABASE --video | --audio | --photos
 
-    Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
+    Files will be saved to <lb download prefix>/<extractor>/. The default prefix is the current working directory.
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
     But you can sort; eg. oldest first
 
@@ -40,14 +127,16 @@
         │ Soundcloud │                  │                 10 │        0 │
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │            │ and 20 minutes   │                    │          │
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘════════════╧══════════════════╧════════════════════╧══════════╛
+
+    Broadcatching absolution
 """
 
 block = r"""library block DATABASE URLS ...
 
     Blocklist specific URLs (eg. YouTube channels, etc)
 
         library block dl.db https://annoyingwebsite/etc/
@@ -609,139 +698,53 @@
                34:54 Glass boilers cost two
 
     Search and open file
 
         library search fts.db 'two words' --open
 """
 
+history_add = """library history-add DATABASE PATH ...
+
+    Add history
+
+        $ library history-add links.db $urls $paths
+        $ library history-add links.db (cb)
+
+    Items that don't already exist in the database will be counted under "skipped"
+
+"""
+
 history = """library history [--frequency daily weekly (monthly) yearly] [--limit LIMIT] DATABASE [(all) watching watched created modified deleted]
 
-    Explore history through different facets
+    View playback history
 
-        library history video.db watched
-        Finished watching:
-        ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
-        │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
-        ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
-        │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
-        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
-        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2023-01       │ 17 hours and 3.32 minutes       │ 15.27 minutes  │ 14.3 GB    │ 214.1 MB   │
-        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
-        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
-        ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
-        ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
+        $ library history web_add.image.db
+        In progress:
+        play_count  time_last_played    playhead    path                                     title
+        ------------  ------------------  ----------  ---------------------------------------  -----------
+                0  today, 20:48        2 seconds   https://siliconpr0n.org/map/COPYING.txt  COPYING.txt
 
-    library history video.db created --frequency yearly
-        Created media:
-        ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
-        │   time_period │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
-        ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
-        │          2005 │ 9.78 minutes                               │ 1.95 minutes   │ 16.9 MB    │ 3.4 MB     │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2006 │ 7 hours and 10.67 minutes                  │ 5 minutes      │ 891.1 MB   │ 10.4 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2007 │ 1 day, 17 hours and 33 minutes             │ 8.55 minutes   │ 5.9 GB     │ 20.3 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2008 │ 5 days, 16 hours and 10 minutes            │ 17.02 minutes  │ 20.7 GB    │ 43.1 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2009 │ 24 days, 2 hours and 56 minutes            │ 33.68 minutes  │ 108.4 GB   │ 105.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2010 │ 1 month, 1 days and 1 minutes              │ 35.52 minutes  │ 124.2 GB   │ 95.7 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2011 │ 2 months, 14 days, 1 hour and 22 minutes   │ 55.93 minutes  │ 222.0 GB   │ 114.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2012 │ 2 months, 22 days, 19 hours and 17 minutes │ 45.50 minutes  │ 343.6 GB   │ 129.6 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2013 │ 3 months, 11 days, 21 hours and 48 minutes │ 42.72 minutes  │ 461.1 GB   │ 131.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2014 │ 3 months, 7 days, 10 hours and 22 minutes  │ 46.80 minutes  │ 529.6 GB   │ 173.1 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2015 │ 2 months, 21 days, 23 hours and 36 minutes │ 36.73 minutes  │ 452.7 GB   │ 139.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2016 │ 3 months, 26 days, 7 hours and 59 minutes  │ 39.48 minutes  │ 603.4 GB   │ 139.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2017 │ 3 months, 10 days, 2 hours and 19 minutes  │ 31.78 minutes  │ 543.5 GB   │ 117.5 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2018 │ 3 months, 21 days, 20 hours and 56 minutes │ 30.98 minutes  │ 607.5 GB   │ 114.8 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2019 │ 5 months, 23 days, 2 hours and 30 minutes  │ 35.77 minutes  │ 919.7 GB   │ 129.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2020 │ 7 months, 16 days, 10 hours and 58 minutes │ 26.15 minutes  │ 1.2 TB     │ 93.9 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2021 │ 7 months, 21 days, 9 hours and 40 minutes  │ 39.93 minutes  │ 1.3 TB     │ 149.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2022 │ 17 years, 3 months, 0 days and 21 hours    │ 19.62 minutes  │ 35.8 TB    │ 77.5 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2023 │ 15 years, 3 months, 24 days and 1 hours    │ 17.57 minutes  │ 27.6 TB    │ 60.2 MB    │
-        ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
-        ╒════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤════════════════╕
-        │ title_path                                                                                 │ duration      │ time_created   │
-        ╞════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪════════════════╡
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 07/20 | Adam Cheng | 2009 #Chinesedrama │ 43.85 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zntYD1yLrG8                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 08/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zQnSfoWrh-4                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 06/20 | Adam Cheng | 2009 #Chinesedrama │ 43.60 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=Qiax1kFyGWU                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 04/20 | Adam Cheng | 2009 #Chinesedrama │ 43.45 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=NT9C3PRrlTA                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 02/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=MjpCiTawlTE                                                │               │                │
-        ╘════════════════════════════════════════════════════════════════════════════════════════════╧═══════════════╧════════════════╛
+    Show only completed history
 
-    View download stats
+        $ library history web_add.image.db --completed
 
-        library history video.db --freqency daily downloaded
-        Downloaded media:
-        day         total_duration                          avg_duration                total_size    avg_size    count
-        ----------  --------------------------------------  ------------------------  ------------  ----------  -------
-        2023-08-11  1 month, 7 days and 8 hours             17 minutes                    192.2 GB     58.3 MB     3296
-        2023-08-12  18 days and 15 hours                    17 minutes                     89.7 GB     56.4 MB     1590
-        2023-08-14  13 days and 1 hours                     22 minutes                    111.2 GB    127.2 MB      874
-        2023-08-15  13 days and 6 hours                     17 minutes                    140.0 GB    126.7 MB     1105
-        2023-08-17  2 months, 8 days and 8 hours            19 minutes                    380.4 GB     72.6 MB     5243
-        2023-08-18  2 months, 30 days and 18 hours          17 minutes                    501.9 GB     63.3 MB     7926
-        2023-08-19  2 months, 6 days and 19 hours           19 minutes                    578.1 GB    110.6 MB     5229
-        2023-08-20  3 days and 9 hours                      6 minutes and 57 seconds       14.5 GB     20.7 MB      700
-        2023-08-21  4 days and 3 hours                      12 minutes                     18.0 GB     36.3 MB      495
-        2023-08-22  10 days and 8 hours                     17 minutes                     82.1 GB     91.7 MB      895
-        2023-08-23  19 days and 9 hours                     22 minutes                     93.7 GB     74.7 MB     1254
+    Show only completed history
 
-        See also: library history video.db --freqency daily downloaded --hide-deleted
+        $ library history web_add.image.db --in-progress
 
-    View deleted stats
+    Delete history
 
-        library history video.db deleted
-        Deleted media:
-        ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
-        │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
-        ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
-        │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
-        ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
-        ╒════════════════════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤══════════════════╤════════════════╕
-        │ title_path                                                                                                 │ duration      │   subtitle_count │ time_deleted   │
-        ╞════════════════════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪══════════════════╪════════════════╡
-        │ Terminus (1987)                                                                                            │ 1 hour and    │                0 │ yesterday      │
-        │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
-        │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
-        │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
-        ...
+        Delete two hours of history
+        $ library history web_add.image.db --played-within '2 hours' -L inf --delete-rows
 
+        Delete all history
+        $ library history web_add.image.db -L inf --delete-rows
+
+    See also: library stats -h
+              library history-add -h
 """
 
 playlists = """library playlists DATABASE
 
     List of Playlists
 
         library playlists
@@ -1014,29 +1017,29 @@
         | path                                                                                                                                                                |     size |
         |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
 
 """
 
-christen = """library christen DATABASE [--run]
+christen = """library christen [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is simulate
 
-        library christen fs.db
+        library christen ~/messy/
 
     To actually do stuff use the run flag
 
-        library christen audio.db --run
+        library christen . --run
 
     You can optionally replace all the spaces in your filenames with dots
 
-        library christen --dot-space video.db
+        library christen --dot-space
 """
 
 cluster_sort = """library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 
         echo 'red apple
@@ -1299,24 +1302,24 @@
             Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
                 rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 """
 
 scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
-    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
-
     Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
 
         library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
 
     Reduce number of files per folder (creates more folders)
 
         library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
+    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
     Multi-device re-bin: balance by size
 
         library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
@@ -1367,14 +1370,17 @@
     Multi-device re-bin: only consider the most recent 100 files
 
         library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
 
     Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
 
         library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
+
+    This tool is intended for local use. If transferring many small files across the network something like
+    [fpart](https://github.com/martymac/fpart) or [fpsync](https://www.fpart.org/fpsync/) will be better.
 """
 
 links_open = """library links-open DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
     Open links from a links db
 
         wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
@@ -1680,14 +1686,19 @@
 
 site_add = """library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
+    Requires selenium-wire
+    Requires xmltodict when using --extract-xml
+
+        pip install selenium-wire xmltodict
+
     Run with `-vv` to see and interact with the browser
 """
 
 process_ffmpeg = """library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
 
     Resize videos to max 1440x960px AV1 and/or Opus to save space
 
@@ -1836,14 +1847,31 @@
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
     Download checked videos
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
+    View most recent files
+
+        library fs example_dbs/web_add.image.db -u time_modified desc --cols path,width,height,size,time_modified -p -l 10
+        path                                                                                                                      width    height       size  time_modified
+        ----------------------------------------------------------------------------------------------------------------------  -------  --------  ---------  -----------------
+        https://siliconpr0n.org/map/infineon/m7690-b1/single/infineon_m7690-b1_infosecdj_mz_nikon20x.jpg                           7066     10513   16.4 MiB  2 days ago, 20:54
+        https://siliconpr0n.org/map/starchip/scf384g/single/starchip_scf384g_infosecdj_mz_nikon20x.jpg                            10804     10730   19.2 MiB  2 days ago, 15:31
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms50x-1.25.jpg            28966     26816  192.2 MiB  4 days ago, 15:05
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms20x-1.25.jpg            11840     10978   49.2 MiB  4 days ago, 15:04
+        https://siliconpr0n.org/map/hp/2hpt20065-1/single/hp_2hpt20065-1_marmontel_mz_ms10x-1.25.jpg                              16457     14255  101.4 MiB  4 days ago, 15:03
+        https://siliconpr0n.org/map/pervasive/e2213ps01e1/single/pervasive_e2213ps01e1_azonenberg_back_roi1_mit10x_rotated.jpg    18880     61836  136.8 MiB  6 days ago, 16:00
+        https://siliconpr0n.org/map/pervasive/e2213ps01e/single/pervasive_e2213ps01e_azonenberg_back_mit5x_rotated.jpg            62208     30736  216.5 MiB  6 days ago, 15:57
+        https://siliconpr0n.org/map/amd/am2964bpc/single/amd_am2964bpc_infosecdj_mz_lmplan10x.jpg                                 12809     11727   39.8 MiB  6 days ago, 10:28
+        https://siliconpr0n.org/map/unknown/ks1804ir1/single/unknown_ks1804ir1_infosecdj_mz_lmplan10x.jpg                          6508      6707    8.4 MiB  6 days ago, 08:04
+        https://siliconpr0n.org/map/amd/am2960dc-b/single/amd_am2960dc-b_infosecdj_mz_lmplan10x.jpg                               16434     15035   64.9 MiB  7 days ago, 19:01
+        10 media (limited by --limit 10)
+
 """
 
 web_update = """library web-update DATABASE
 
     Update saved open directories
 
 """
@@ -1875,7 +1903,56 @@
 
 nouns = """library nouns (stdin)
 
     Extract compound nouns and phrases from unstructured mixed HTML plain text
 
         xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
 """
+
+similar_files = """library similar-files PATH ...
+
+    Find similar files using filenames and size
+
+        $ library similar-files ~/d/
+
+    Find similar files based on ONLY foldernames, using the full path
+
+        $ library similar-files --no-filter-sizes --full-path ~/d/
+
+    Find similar files based on ONLY size
+
+        $ library similar-files --no-filter-names ~/d/
+"""
+
+similar_folders = """library similar-folders PATH ...
+
+    Find similar folders based on foldernames, similar size, and similar number of files
+
+        $ library similar-folders ~/d/
+
+        group /home/xk/d/dump/datasets/*vector          total_size    median_size      files
+        ----------------------------------------------  ------------  -------------  -------
+        /home/xk/d/dump/datasets/vector/output/         1.8 GiB       89.5 KiB          1980
+        /home/xk/d/dump/datasets/vector/output2/        1.8 GiB       89.5 KiB          1979
+
+    Find similar folders based on ONLY foldernames, using the full path
+
+        $ library similar-folders --no-filter-sizes --no-filter-counts --full-path ~/d/
+
+    Find similar folders based on ONLY number of files
+
+        $ library similar-folders --no-filter-names --no-filter-sizes ~/d/
+
+    Find similar folders based on ONLY median size
+
+        $ library similar-folders --no-filter-names --no-filter-counts ~/d/
+
+    Find similar folders based on ONLY total size
+
+        $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
+
+    Print only paths
+
+        $ library similar-folders ~/d/ -pf
+        /home/xk/d/dump/datasets/vector/output/
+        /home/xk/d/dump/datasets/vector/output2/
+"""
```

### Comparing `xklb-2.6.9/xklb/createdb/av.py` & `xklb-2.7.5/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/createdb/fs_add.py` & `xklb-2.7.5/xklb/createdb/fs_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
 from xklb.createdb import av
 from xklb.files import sample_hash
-from xklb.mediadb import playlists
-from xklb.mediafiles.process_ffmpeg import process_ffmpeg
-from xklb.mediafiles.process_image import process_image
+from xklb.mediadb import db_media, db_playlists, playlists
+from xklb.mediafiles import process_ffmpeg, process_image
 from xklb.utils import (
     arg_utils,
     arggroups,
+    argparse_utils,
     consts,
     db_utils,
     file_utils,
     iterables,
     nums,
     objects,
     path_utils,
@@ -31,14 +31,15 @@
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
 
 
 def parse_args(action, usage):
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
     arggroups.db_profiles(parser)
     arggroups.capability_simulate(parser)
+    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
 
     parser.add_argument(
         "--io-multiplier",
         type=float,
         default=1.0,
         help="Especially useful for text, image, filesystem db types",
     )
@@ -148,15 +149,15 @@
 
     ext = path.rsplit(".", 1)[-1].lower()
     is_scan_all_files = getattr(mp_args, "scan_all_files", False)
 
     if media["type"] == "directory":
         return None
 
-    if not Path(path).exists():
+    if media["size"] == 0 or not Path(path).exists():
         return media
 
     if objects.is_profile(mp_args, DBType.audio) and (ext in consts.AUDIO_ONLY_EXTENSIONS or is_scan_all_files):
         media |= av.munge_av_tags(mp_args, path)
     elif objects.is_profile(mp_args, DBType.video) and (ext in consts.VIDEO_EXTENSIONS or is_scan_all_files):
         media |= av.munge_av_tags(mp_args, path)
 
@@ -225,15 +226,20 @@
     for k in list(e.keys()):
         if key_substring in k:
             values.append(e.pop(k))
     return values
 
 
 def munge_image_tags(m: dict, e: dict) -> dict:
-    chroma_subsample = int((e.pop("File:YCbCrSubSampling", None) or "0").replace(" ", ""))
+    chroma_subsample = nums.safe_int(
+        iterables.safe_unpack(
+            e.pop("File:YCbCrSubSampling", None),
+            *pop_substring_keys(e, "YCbCrSubSampling"),
+        )
+    )
     if chroma_subsample == 0:
         chroma_subsample = None
 
     unit_x = iterables.safe_unpack(
         *pop_substring_keys(e, "XResolution"),
     )
     unit_y = iterables.safe_unpack(
@@ -282,14 +288,18 @@
             e.pop("Composite:GPSLongitude", None),
             *pop_substring_keys(e, "GPSLongitude"),
         ),
         "latitude": iterables.safe_unpack(
             e.pop("Composite:GPSLatitude", None),
             *pop_substring_keys(e, "GPSLatitude"),
         ),
+        "focal_length": iterables.safe_unpack(
+            e.pop("Composite:Lens", None),
+            *pop_substring_keys(e, "Lens35efl"),
+        ),
         "unit": unit,
         "unit_x": unit_x,
         "unit_y": unit_y,
         "exiftool_warning": strings.combine(*pop_substring_keys(e, "ExifTool:Warning")),
         "tags": strings.combine(
             *pop_substring_keys(e, "Headline"),
             *pop_substring_keys(e, "Title"),
@@ -299,124 +309,20 @@
             *pop_substring_keys(e, "By-line"),
             *pop_substring_keys(e, "Credit"),
             *pop_substring_keys(e, "DocumentNotes"),
             *pop_substring_keys(e, "URL_List"),
             *pop_substring_keys(e, "Keywords"),
             *pop_substring_keys(e, "Make"),
             *pop_substring_keys(e, "Model"),
+            *pop_substring_keys(e, "LensID"),
             *pop_substring_keys(e, "Creator"),
             *pop_substring_keys(e, "Software"),
         ),
     }
 
-    for s in (
-        "PDF",
-        "ObjectName",
-        "YCbCrPositioning",
-        ":ISO",
-        "ExposureProgram",
-        "FNumber",
-        "SensingMethod",
-        "SubjectDistance",
-        "Scene",
-        "Sharpness",
-        "Saturation",
-        "Flash",
-        "Contrast",
-        "MeteringMode",
-        "InteropIndex",
-        "ExposureCompensation",
-        "BrightnessValue",
-        "CustomRendered",
-        "ComponentsConfiguration",
-        "ShutterSpeed",
-        "ExposureMode",
-        "Aperture",
-        "ScaleFactor",
-        "LightValue",
-        "GPSProcessingMethod",
-        "GPSPosition",
-        "focalDistance",
-        "GPSDOP",
-        "FocalLength",
-        "FOV",
-        "CircleOfConfusion",
-        "GPSLatitudeRef",
-        "GPSLongitudeRef",
-        "Thumbnail",
-        "PrintStyle",
-        "Angle",
-        "Altitude",
-        "Displayed",
-        "WriterName",
-        "ReaderName",
-        "Date",
-        "History",
-        "Version",
-        "Compression",
-        "Digest",
-        "PrintPosition",
-        "PrintScale",
-        "Copyright",
-        "WhiteBalance",
-        "WhitePoint",
-        "ColorSpace",
-        "ColorTransform",
-        "ColorComponents",
-        "LightSource",
-        "Swatch",
-        "Profile",
-        "XMP:",
-        "ByteOrder",
-        "Comment",
-        "BitsPerSample",
-        "BitsPerPixel",
-        "Interpretation",
-        "EncodingProcess",
-        "Megapixels",
-        "PixelAspectRatio",
-        "ImageSize",
-        "PhotoshopFormat",
-        "OriginalTransmissionReference",
-        "Time",
-        "NumSlices",
-        "ImageUniqueID",
-        "HasRealMergedData",
-        "CodedCharacterSet",
-        "Flags0",
-        "Flags1",
-        "Padding",
-        "ProgressiveScans",
-        "HasColorMap",
-        "Ducky:Quality",
-        "PhotoshopQuality",
-        "SlicesGroupName",
-        "SupplementalCategories",
-        "Duration",
-        "Animation",
-        "FrameCount",
-    ):
-        pop_substring_keys(e, s)
-
-    for k in (
-        "File:FileName",
-        "File:Directory",
-        "File:FileSize",
-        "File:MIMEType",
-        "File:FilePermissions",
-        "File:FileTypeExtension",
-        "File:FileType",
-        "IPTC:SpecialInstructions",
-        "File:Exif",
-    ):
-        e.pop(k, None)
-
-    if e != {}:
-        log.info("Extra data %s", e)
-
     return m
 
 
 def extract_image_metadata_chunk(metadata: list[dict]) -> list[dict]:
     try:
         import exiftool
     except ModuleNotFoundError:
```

### Comparing `xklb-2.6.9/xklb/createdb/gallery_add.py` & `xklb-2.7.5/xklb/createdb/gallery_add.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
 from xklb.createdb import gallery_backend
+from xklb.mediadb import db_media, db_playlists
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
```

### Comparing `xklb-2.6.9/xklb/createdb/gallery_backend.py` & `xklb-2.7.5/xklb/createdb/gallery_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import gallery_dl
 from gallery_dl.exception import StopExtraction
 from gallery_dl.extractor.message import Message
 from gallery_dl.job import Job
 from gallery_dl.util import build_duration_func
 
-from xklb import db_media, db_playlists
+from xklb.mediadb import db_media, db_playlists
 from xklb.utils import consts, printing, strings
 from xklb.utils.log_utils import log
 
 gallery_dl = None
 
 
 def load_module_level_gallery_dl(args) -> ModuleType:
```

### Comparing `xklb-2.6.9/xklb/createdb/hn_add.py` & `xklb-2.7.5/xklb/createdb/hn_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/createdb/links_add.py` & `xklb-2.7.5/xklb/createdb/links_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse, json, random, time
 from pathlib import Path
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
+from xklb.mediadb import db_media, db_playlists
 from xklb.text import extract_links
 from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args(**kwargs):
     parser = argparse.ArgumentParser(**kwargs)
```

### Comparing `xklb-2.6.9/xklb/createdb/places_import.py` & `xklb-2.7.5/xklb/createdb/places_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 from pathlib import Path
 
-from xklb import db_media, usage
+from xklb import usage
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, consts, db_utils, nums, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library places-import", usage=usage.places_import)
     arggroups.database(parser)
```

### Comparing `xklb-2.6.9/xklb/createdb/reddit_add.py` & `xklb-2.7.5/xklb/createdb/reddit_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import prawcore
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
+from xklb.mediadb import db_media, db_playlists
 from xklb.utils import arggroups, consts, db_utils, iterables, objects
 from xklb.utils.log_utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
```

### Comparing `xklb-2.6.9/xklb/createdb/row_add.py` & `xklb-2.7.5/xklb/createdb/row_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/createdb/rss_add.py` & `xklb-2.7.5/xklb/createdb/rss_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 def try_get_head_link(path):
     import requests
     from bs4 import BeautifulSoup
 
     try:
         response = requests.get(path)
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         link = soup.find("link", type="application/rss+xml")
         if link:
             return link.get("href")  # type: ignore
     except TypeError:
         return None
 
 
 def try_get_link_endswith(path):
     import requests
     from bs4 import BeautifulSoup
 
     try:
         response = requests.get(path)
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         link = soup.find("a", href=lambda href: href and (href.endswith((".rss", ".xml"))))  # type: ignore
         if link:
             return link.get("href")  # type: ignore
     except TypeError:
         return None
```

### Comparing `xklb-2.6.9/xklb/createdb/substack.py` & `xklb-2.7.5/xklb/createdb/substack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 
-from xklb import db_media, usage
+from xklb import usage
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, db_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library substack", usage=usage.substack)
     arggroups.requests(parser)
@@ -22,15 +23,15 @@
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def save_page(args, url):
     response = web.get(args, url)
     if response:
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         web.download_embeds(args, soup)
 
         try:
             subtitle = soup.select_one("h3.subtitle").getText()  # type: ignore
         except AttributeError:
             subtitle = None
```

### Comparing `xklb-2.6.9/xklb/createdb/subtitle.py` & `xklb-2.7.5/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/createdb/tabs_add.py` & `xklb-2.7.5/xklb/createdb/tabs_add.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse, sys
 from datetime import datetime, timedelta
 from pathlib import Path
 from random import randint
 
-from xklb import db_media, history, usage
+from xklb import usage
+from xklb.mediadb import db_history, db_media
 from xklb.utils import arggroups, consts, db_utils, iterables, objects, path_utils, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tabs-add", usage=usage.tabs_add)
     arggroups.extractor(parser)
@@ -97,15 +98,15 @@
         max_date = datetime.today()
 
         min_time = int(min_date.replace(hour=0, minute=0, second=0, microsecond=0).timestamp())
         max_time = int(max_date.replace(hour=0, minute=0, second=0, microsecond=0).timestamp())
 
         for d in tabs:
             time_played = randint(min_time, max_time)
-            history.add(args, [d["path"]], time_played=time_played, mark_done=True)
+            db_history.add(args, [d["path"]], time_played=time_played, mark_done=True)
 
 
 def tabs_shuffle() -> None:
     parser = argparse.ArgumentParser(prog="library tabs-shuffle", usage=usage.tabs_shuffle)
     parser.add_argument("--days", "-d", type=int, default=7)
     parser.add_argument(
         "--frequency",
@@ -162,8 +163,8 @@
         max_time = d["time_last_played"]
         time_played = randint(min_time, max_time)
 
         with args.db.conn:  # type: ignore
             args.db.conn.execute(  # type: ignore
                 "DELETE from history WHERE media_id = ? and time_played = ?", [d["id"], d["time_last_played"]]
             )
-        history.add(args, [d["path"]], time_played=time_played, mark_done=True)
+        db_history.add(args, [d["path"]], time_played=time_played, mark_done=True)
```

### Comparing `xklb-2.6.9/xklb/createdb/tildes.py` & `xklb-2.7.5/xklb/createdb/tildes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from datetime import datetime
 from pathlib import Path
 from time import sleep
 
 from bs4 import BeautifulSoup
 from dateutil import parser
 
-from xklb import db_media, usage
+from xklb import usage
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, db_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tildes", usage=usage.tildes)
     arggroups.requests(parser)
@@ -23,15 +24,15 @@
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def save_page(args, text):
-    soup = BeautifulSoup(text, "html.parser")
+    soup = BeautifulSoup(text, "lxml")
 
     comment_elements = soup.find_all("article", class_="comment")
     for comment_element in comment_elements:
         edited_time_element = comment_element.find("time", class_="comment-edited-time")
         score_element = comment_element.find("div", class_="comment-votes")
         parent_path_element = comment_element.find("a", class_="comment-nav-link", text="Parent")
         comment = {
```

### Comparing `xklb-2.6.9/xklb/createdb/tube_add.py` & `xklb-2.7.5/xklb/createdb/tube_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
 from xklb.createdb import tube_backend
+from xklb.mediadb import db_media, db_playlists
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
```

### Comparing `xklb-2.6.9/xklb/createdb/tube_backend.py` & `xklb-2.7.5/xklb/createdb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json, sys
 from copy import deepcopy
 from pathlib import Path
 from pprint import pprint
 from subprocess import CalledProcessError
 from types import ModuleType
 
-from xklb import db_media, db_playlists
 from xklb.createdb import subtitle
 from xklb.data.yt_dlp_errors import (
     prefix_unrecoverable_errors,
     yt_meaningless_errors,
     yt_recoverable_errors,
     yt_unrecoverable_errors,
 )
+from xklb.mediadb import db_media, db_playlists
 from xklb.mediafiles import media_check
 from xklb.utils import consts, db_utils, iterables, objects, path_utils, printing, sql_utils, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 yt_dlp = None
 yt_archive = set()
@@ -507,19 +507,17 @@
         else:
             log.info("[%s]: Downloaded to %s", webpath, local_path)
             db_media.download_add(args, webpath, info, local_path)
     elif any(yt_recoverable_errors.match(line) for line in ydl_errors):
         log.info("[%s]: Recoverable error matched (will try again later). %s", webpath, ydl_errors_txt)
         db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
     elif any(yt_unrecoverable_errors.match(line) for line in ydl_errors):
-        matched_error = [
-            m.string for m in iterables.conform([yt_unrecoverable_errors.match(line) for line in ydl_errors])
-        ]
+        matched_error = iterables.conform([line for line in ydl_errors if yt_unrecoverable_errors.match(line)])
         log.info("[%s]: Unrecoverable error matched. %s", webpath, ydl_errors_txt or strings.combine(matched_error))
         db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt, unrecoverable_error=True)
     elif any(prefix_unrecoverable_errors.match(line) for line in ydl_errors):
         log.warning("[%s]: Prefix error. %s", webpath, ydl_errors_txt)
         raise SystemExit(28)
     else:
         log.error("[%s]: Unknown error. %s", webpath, ydl_errors_txt)
-        pprint([yt_meaningless_errors.match(line) for line in ydl_full_log])
+        pprint(ydl_full_log)
         db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
```

### Comparing `xklb-2.6.9/xklb/createdb/web_add.py` & `xklb-2.7.5/xklb/createdb/web_add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse, json, random, sys, time
 from pathlib import Path
 from urllib.parse import urlparse
 
-from xklb import db_media, db_playlists, usage
+from xklb import usage
 from xklb.createdb import av, fs_add
 from xklb.files import sample_hash
+from xklb.mediadb import db_media, db_playlists
 from xklb.text import extract_links
 from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, iterables, objects, printing, strings, web
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args(**kwargs):
@@ -72,14 +73,15 @@
         media = [consolidate_media(args, s) for s in media]
 
     media = iterables.list_dict_filter_bool(media)
     args.db["media"].insert_all(media, pk="id", alter=True, replace=True)
 
 
 def spider(args, paths: set):
+    original_paths = paths.copy()
     get_urls = iterables.return_unique(extract_links.get_inner_urls)
 
     new_media_count = 0
     known_paths = set()
     traversed_paths = set()
     while len(paths) > 0:
         new_paths = {}
@@ -87,15 +89,15 @@
         traversed_paths.add(path)
         log.info("Loading %s", path)
 
         printing.print_overwrite(
             f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]"
         )
 
-        if web.is_index(path):
+        if path in original_paths or web.is_index(path) or web.is_html(path):
             for a_ref in get_urls(args, path):
                 if a_ref is None:
                     break
 
                 link, link_text = a_ref
 
                 link = web.remove_apache_sorting_params(link)
```

### Comparing `xklb-2.6.9/xklb/data/imagemagick_errors.py` & `xklb-2.7.5/xklb/data/imagemagick_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 
 unsupported_error = re.compile(
     "|".join(
         r""".*unsupported
 .* not supported
 .* password
+.* no images defined
 .* bad magic number
 .*can not handle
 .* count
 .* exceeded
 .* allocation failed
 .*no decode delegate for this image format""".splitlines(),
     ),
```

### Comparing `xklb-2.6.9/xklb/data/wordbank.py` & `xklb-2.7.5/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/data/yt_dlp_errors.py` & `xklb-2.7.5/xklb/data/yt_dlp_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 .*No such file or directory
 .*The downloaded file is empty
 .*Invalid data found
 .*fragment 1 not found
 .*Got error: 0 bytes read
 .*HTTP Error 429
 .*HTTP Error 400
-.*HTTP Error 503: Service Unavailable
+.*HTTP Error 503
 .*Origin Error
 .*API is not granting access
 .*Did not get any data blocks
 .*Too Many Requests
 .*Postprocessing
 .*Premieres in
 .*user.*not allowed
@@ -133,14 +133,15 @@
 .*Premieres in""".splitlines(),
     ),
 )
 
 yt_unrecoverable_errors = re.compile(
     "|".join(
         r""".*repetitive or misleading metadata
+.*got player responses for video.*instead of
 .*It is not available
 .*does not pass filter
 .*has already been recorded in the archive
 .*ideo.*is private
 .*already ended
 .*id.*was not found
 .*No video player ID
```

### Comparing `xklb-2.6.9/xklb/editdb/dedupe_db.py` & `xklb-2.7.5/xklb/editdb/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/editdb/dedupe_media.py` & `xklb-2.7.5/xklb/editdb/dedupe_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
 from pathlib import Path
 
 import humanize
 
-from xklb import db_media, media_printer, usage
+from xklb import media_printer, usage
 from xklb.files import sample_compare, sample_hash
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe-media", usage=usage.dedupe_media)
```

### Comparing `xklb-2.6.9/xklb/editdb/merge_online_local.py` & `xklb-2.7.5/xklb/editdb/merge_online_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, os
 from copy import deepcopy
 
-from xklb import db_media, media_printer, usage
+from xklb import media_printer, usage
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, consts, db_utils, devices, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
```

### Comparing `xklb-2.6.9/xklb/editdb/mpv_watchlater.py` & `xklb-2.7.5/xklb/editdb/mpv_watchlater.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 from pathlib import Path
 
-from xklb import history, usage
+from xklb import usage
+from xklb.mediadb import db_history
 from xklb.utils import arggroups, consts, db_utils, mpv_utils, nums, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library mpv-watchlater", usage=usage.mpv_watchlater)
     parser.add_argument("--watch-later-directory", default=consts.DEFAULT_MPV_WATCH_LATER, help=argparse.SUPPRESS)
@@ -32,17 +33,17 @@
         }
         for p in paths
         if md5s.get(p.stem)
     ]
 
     # create two records if first played and last played time are different
     for m in previously_watched:
-        history.add(args, media_ids=[m["id"]], time_played=m["time_first_played"], playhead=m["playhead"])
+        db_history.add(args, media_ids=[m["id"]], time_played=m["time_first_played"], playhead=m["playhead"])
         if m["time_first_played"] != m["time_last_played"]:
-            history.add(args, media_ids=[m["id"]], time_played=m["time_last_played"], playhead=m["playhead"])
+            db_history.add(args, media_ids=[m["id"]], time_played=m["time_last_played"], playhead=m["playhead"])
 
 
 def mpv_watchlater():
     args = parse_args()
     media = list(
         args.db.query(
             """
```

### Comparing `xklb-2.6.9/xklb/editdb/pushshift.py` & `xklb-2.7.5/xklb/editdb/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/editdb/reddit_selftext.py` & `xklb-2.7.5/xklb/editdb/reddit_selftext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, html
 from urllib.parse import urlparse
 
-from xklb import db_media, usage
+from xklb import usage
+from xklb.mediadb import db_media
 from xklb.utils import arggroups, db_utils, log_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
     arggroups.debug(parser)
```

### Comparing `xklb-2.6.9/xklb/files/sample_compare.py` & `xklb-2.7.5/xklb/files/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/files/sample_hash.py` & `xklb-2.7.5/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/folders/merge_folders.py` & `xklb-2.7.5/xklb/folders/merge_folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     destination_folders = (
         destination_folders_dict["file"] | destination_folders_dict["folder"] | destination_folders_dict["empty"]
     )
 
     all_source_folders = set()
     empty_folder_data: set[Path] = set()
     rename_data: list[tuple[bool, Path, Path]] = []
-    clobber = False
+    clobber = False  # default nothing to clobber; no confirmation prompt
     print("Sources:")
     for source in args.sources:
         source_folder, source_glob = arg_utils.split_folder_glob(source)
         source_files, source_folders_dict = existing_stats(source_folder, source_glob)
         source_folders = source_folders_dict["file"] | source_folders_dict["folder"] | source_folders_dict["empty"]
 
         source_new_empty_folders = gen_rename_data(
```

### Comparing `xklb-2.6.9/xklb/folders/move_list.py` & `xklb-2.7.5/xklb/folders/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/folders/rel_mv.py` & `xklb-2.7.5/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/folders/scatter.py` & `xklb-2.7.5/xklb/folders/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/fsdb/big_dirs.py` & `xklb-2.7.5/xklb/fsdb/big_dirs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse, os
+from collections import defaultdict
 from pathlib import Path
 
-from xklb import history, media_printer, usage
+from xklb import media_printer, usage
+from xklb.mediadb import db_history
 from xklb.tablefiles import mcda
 from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, nums, objects, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -39,18 +41,20 @@
         args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
 
     args.action = consts.SC.big_dirs
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def group_files_by_folder(args, media) -> list[dict]:
+def group_files_by_parents(args, media) -> list[dict]:
     p_media = {}
+    min_parts = 10
     for m in media:
         p = m["path"].split(os.sep)
+        min_parts = min(min_parts, len(p))
         while len(p) >= 2:
             p.pop()
             parent = os.sep.join(p) + os.sep
 
             if parent not in p_media:
                 p_media[parent] = []
             else:
@@ -64,14 +68,47 @@
             "total": len(media),
             "exists": sum(not bool(m.get("time_deleted")) for m in media),
             "deleted": sum(bool(m.get("time_deleted")) for m in media),
             "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
             "played": sum(bool(m.get("time_last_played")) for m in media),
         }
 
+    for parent, _ in list(d.items()):
+        if len(parent.split(os.sep)) < min_parts:
+            d.pop(parent)
+
+    for path, pdict in list(d.items()):
+        if pdict["exists"] == 0:
+            d.pop(path)
+        elif not args.depth:
+            if args.lower and pdict["exists"] < args.lower:
+                d.pop(path)
+            elif args.upper and pdict["exists"] > args.upper:
+                d.pop(path)
+
+    return [{**v, "path": k} for k, v in d.items()]
+
+
+def group_files_by_parent(args, media) -> list[dict]:
+    p_media = defaultdict(list)
+    for m in media:
+        p_media[str(Path(m["path"]).parent)].append(m)
+
+    d = {}
+    for parent, media in list(p_media.items()):
+        d[parent] = {
+            "size": sum(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "median_size": nums.safe_median(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "total": len(media),
+            "exists": sum(not bool(m.get("time_deleted")) for m in media),
+            "deleted": sum(bool(m.get("time_deleted")) for m in media),
+            "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
+            "played": sum(bool(m.get("time_last_played")) for m in media),
+        }
+
     for path, pdict in list(d.items()):
         if pdict["exists"] == 0:
             d.pop(path)
         elif not args.depth:
             if args.lower and pdict["exists"] < args.lower:
                 d.pop(path)
             elif args.upper and pdict["exists"] > args.upper:
@@ -120,27 +157,27 @@
         args,
         [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
     )
 
     media = list(
         args.db.query(
             f"""
-        SELECT
-            path
-            , size
-            {', time_deleted' if 'time_deleted' in m_columns else ''}
-            , MAX(h.time_played) time_played
-        FROM media m
-        LEFT JOIN history h on h.media_id = m.id
-        WHERE 1=1
-            {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
-            {" ".join(args.filter_sql)}
-        GROUP BY m.id
-        ORDER BY path
-        """,
+            SELECT
+                path
+                , size
+                {', time_deleted' if 'time_deleted' in m_columns else ''}
+                , MAX(h.time_played) time_played
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
+            WHERE 1=1
+                {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
+                {" ".join(args.filter_sql)}
+            GROUP BY m.id
+            ORDER BY path
+            """,
             args.filter_bindings,
         ),
     )
     return media
 
 
 def process_big_dirs(args, folders) -> list[dict]:
@@ -153,27 +190,27 @@
         folders = [d for d in folders if args.folder_size(d["size"])]
 
     return folders
 
 
 def big_dirs() -> None:
     args = parse_args()
-    history.create(args)
+    db_history.create(args)
 
     media = get_table(args)
     if args.cluster_sort and len(media) > 2:
         from xklb.text.cluster_sort import cluster_paths
 
         groups = cluster_paths([d["path"] for d in media], n_clusters=getattr(args, "clusters", None))
-        groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
+        groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
 
         media_keyed = {d["path"]: d for d in media}
         folders = [
             {
-                "path": group["common_prefix"],
+                "path": group["common_path"],
                 "total": len(group["grouped_paths"]),
                 "played": sum(bool(media_keyed[s].get("time_played")) for s in group["grouped_paths"]),
                 "exists": sum(not bool(media_keyed[s].get("time_deleted")) for s in group["grouped_paths"]),
                 "deleted": sum(bool(media_keyed[s].get("time_deleted")) for s in group["grouped_paths"]),
                 "deleted_size": sum(
                     media_keyed[s].get("size") or 0
                     for s in group["grouped_paths"]
@@ -188,16 +225,18 @@
                     media_keyed[s].get("size") or 0
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
             }
             for group in groups
         ]
+    elif args.parents:
+        folders = group_files_by_parents(args, media)
     else:
-        folders = group_files_by_folder(args, media)
+        folders = group_files_by_parent(args, media)
 
     folders = mcda.group_sort_by(args, folders)
     media = process_big_dirs(args, folders)
 
     if args.limit:
         media = media[-int(args.limit) :]
     media_printer.media_printer(args, media, units="folders")
```

### Comparing `xklb-2.6.9/xklb/fsdb/christen.py` & `xklb-2.7.5/xklb/files/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/fsdb/disk_usage.py` & `xklb-2.7.5/xklb/fsdb/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/fsdb/mount_stats.py` & `xklb-2.7.5/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/fsdb/search_db.py` & `xklb-2.7.5/xklb/fsdb/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/mediadb/block.py` & `xklb-2.7.5/xklb/mediadb/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 def add_to_blocklist(args, p):
     p = p.pop()
     args.db["blocklist"].insert({"key": args.match_column, "value": p}, alter=True, replace=True, pk=["key", "value"])
 
 
 def remove_from_blocklist(args, p):
     p = p.pop()
-    args.db["blocklist"].delete([args.match_column, p])
+    with args.db.conn:
+        args.db["blocklist"].delete([args.match_column, p])
 
 
 def block(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args = parse_args()
```

### Comparing `xklb-2.6.9/xklb/mediadb/download.py` & `xklb-2.7.5/xklb/mediadb/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, os, sys
 
-from xklb import db_media, media_printer, usage
+from xklb import media_printer, usage
 from xklb.createdb import gallery_backend, tube_backend
+from xklb.mediadb import db_media
 from xklb.utils import (
     arg_utils,
     arggroups,
     argparse_utils,
     consts,
     db_utils,
     iterables,
```

### Comparing `xklb-2.6.9/xklb/mediadb/download_status.py` & `xklb-2.7.5/xklb/mediadb/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/mediadb/history.py` & `xklb-2.7.5/xklb/playback/links_open.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,211 @@
-import argparse
+import argparse, shlex, webbrowser
+from pathlib import Path
+from time import sleep
 
 from xklb import media_printer, usage
-from xklb.history import create
-from xklb.utils import arggroups, consts, db_utils, objects, sql_utils, strings
+from xklb.mediadb import db_history, db_media
+from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes, web
 from xklb.utils.log_utils import log
+from xklb.utils.printing import pipe_print
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        "library history",
-        usage=usage.history,
+        prog="library open-links",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        usage=usage.links_open,
     )
-
     arggroups.sql_fs(parser)
-    arggroups.sql_media(parser)
 
-    arggroups.frequency(parser)
-    parser.add_argument(
-        "facet",
-        metavar="facet",
-        type=str.lower,
-        default="watched",
-        const="watched",
-        nargs="?",
-        help=f"One of: {', '.join(consts.time_facets)}",
-    )
-    parser.add_argument("--hide-deleted", action="store_true")
-    parser.add_argument("--played", "--opened", action="store_true")
+    parser.add_argument("--path", action="store_true")
+    parser.add_argument("--title", action="store_true")
+    parser.add_argument("--title-prefix", "--prefix", nargs="+", action="extend")
+
+    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
+
+    parser.add_argument("--category", "-c")
+
+    arggroups.operation_cluster(parser)
+    arggroups.operation_related(parser)
 
+    parser.add_argument("--browser")
     arggroups.debug(parser)
 
     arggroups.database(parser)
+    parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
+    args.action = consts.SC.links_open
+    args.defaults = []
 
-    args.facet = strings.partial_startswith(args.facet, consts.time_facets)
-    args.frequency = strings.partial_startswith(args.frequency, consts.frequency)
+    arg_utils.parse_args_limit(args)
 
-    args.db = db_utils.connect(args)
+    args.include += args.search
+    if args.include == ["."]:
+        args.include = [str(Path().cwd().resolve())]
 
-    args.action = consts.SC.history
-    log.info(objects.dict_filter_bool(args.__dict__))
+    if not args.title_prefix:
+        args.title_prefix = ["https://www.google.com/search?q=%"]
+    args.title_prefix = [s if "%" in s else s + "%" for s in args.title_prefix]
 
-    args.filter_bindings = {}
+    if args.browser:
+        args.browser = shlex.split(args.browser)
 
-    return args
+    if args.sort:
+        args.sort = [arg_utils.override_sort(s) for s in args.sort]
+        args.sort = " ".join(args.sort)
 
+    if args.cols:
+        args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
-def process_search(args, m_columns):
-    args.table = "media"
-    if args.db["media"].detect_fts():
-        if args.include:
-            args.table, search_bindings = db_utils.fts_search_sql(
-                "media",
-                fts_table=args.db["media"].detect_fts(),
-                include=args.include,
-                exclude=args.exclude,
-            )
-            args.filter_bindings = search_bindings
-        elif args.exclude:
-            db_utils.construct_search_bindings(
-                args,
-                [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-            )
-    else:
-        db_utils.construct_search_bindings(
-            args,
-            [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-        )
+    args.db = db_utils.connect(args)
+    log.info(objects.dict_filter_bool(args.__dict__))
 
+    return args
 
-def recent_media(args, time_column):
+
+def construct_links_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
-    process_search(args, m_columns)
-    query = f"""
-    SELECT
-        path
-        {', title' if 'title' in m_columns else ''}
-        {', duration' if 'duration' in m_columns else ''}
-        {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-        , {time_column}
-    FROM {args.table} m
-    {'JOIN history h on h.media_id = m.id' if args.played else ''}
+
+    args.filter_sql = []
+    args.filter_bindings = {}
+
+    args.filter_sql.extend([" and " + w for w in args.where])
+
+    for idx, inc in enumerate(args.include):
+        args.filter_sql.append(
+            f"""and (
+                path like :include{idx}
+                {f'OR title like :include{idx}' if 'title' in m_columns else ''}
+            )"""
+        )
+        if args.exact:
+            args.filter_bindings[f"include{idx}"] = inc
+        else:
+            args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
+    for idx, exc in enumerate(args.exclude):
+        args.filter_sql.append(
+            f"""and (
+                path not like :exclude{idx}
+                {f'AND title not like :exclude{idx}' if 'title' in m_columns else ''}
+            )"""
+        )
+        if args.exact:
+            args.filter_bindings[f"exclude{idx}"] = exc
+        else:
+            args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
+
+    if args.category:
+        args.filter_sql.append("AND category like :category")
+        if args.exact:
+            args.filter_bindings[f"category"] = args.category
+        else:
+            args.filter_bindings[f"category"] = "%" + args.category.replace(" ", "%").replace("%%", " ") + "%"
+
+    limit_sql = "LIMIT " + str(args.limit) if args.limit and not args.cluster_sort else ""
+    offset_sql = f"OFFSET {args.offset}" if args.offset and limit_sql else ""
+
+    args.select = ["path"]
+    if args.cols:
+        args.select.extend(args.cols)
+    for s in ["title", "hostname", "category"]:
+        if s in m_columns:
+            args.select.append(s)
+
+    query = f"""WITH m as (
+            SELECT
+                {', '.join(args.select) if args.select else ''}
+                , COALESCE(MAX(h.time_played), 0) time_last_played
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , time_deleted
+            FROM media
+            LEFT JOIN history h on h.media_id = media.id
+            WHERE COALESCE(time_deleted, 0)=0
+            GROUP BY media.id
+        )
+        SELECT
+        {', '.join(args.select) if args.select else ''}
+        {", time_last_played" if args.print else ''}
+    FROM m
     WHERE 1=1
-      AND coalesce({time_column}, 0)>0
-    {'AND COALESCE(time_deleted, 0)=0' if args.hide_deleted else ""}
-    ORDER BY {time_column} desc
-    LIMIT {args.limit or 5}
+        AND COALESCE(time_deleted, 0)=0
+        {'AND path like "http%"' if args.online_media_only else ''}
+        {'AND path not like "http%"' if args.local_media_only else ''}
+        {" ".join(args.filter_sql)}
+    ORDER BY 1=1
+        {', ' + args.sort if args.sort else ''}
+        , play_count
+        {', ROW_NUMBER() OVER ( PARTITION BY hostname )' if 'hostname' in m_columns else ''}
+        {', ROW_NUMBER() OVER ( PARTITION BY category )' if 'category' in m_columns else ''}
+        , random()
+    {limit_sql} {offset_sql}
     """
-    return list(args.db.query(query, args.filter_bindings))
 
+    return query, args.filter_bindings
+
+
+def play(args, path, url) -> None:
+    if args.browser:
+        if "".join(args.browser) in ["echo", "print"]:
+            pipe_print(url)
+        else:
+            processes.cmd(*args.browser, url)
+    else:
+        webbrowser.open(url, 2, autoraise=False)
+    db_history.add(args, [path], time_played=consts.APPLICATION_START, mark_done=True)
+
+
+def make_souffle(args, media):
+    pan = []
 
-def remove_duplicate_data(tbl):
-    if all(d["play_count"] == 1 for d in tbl):
-        for d in tbl:
-            del d["time_first_played"]
+    urls = set()
+    for m in media:
+        m_urls = set()
+        if args.title:
+            for engine in args.title_prefix:
+                suffix = m.get("title") or m["path"]
+                m_urls.add(suffix if suffix.startswith("http") else web.construct_search(engine, suffix))
 
+        if not args.title or args.path:
+            if not m["path"].startswith("http"):
+                for engine in args.title_prefix:
+                    m_urls.add(web.construct_search(engine, m["path"]))
+            else:
+                m_urls.add(m["path"])
 
-def history() -> None:
+        pan.extend([{**m, "url": url} for url in m_urls if url not in urls])
+        urls |= m_urls
+
+    return pan
+
+
+def links_open() -> None:
     args = parse_args()
-    m_columns = args.db["media"].columns_dict
-    create(args)
+    db_history.create(args)
 
-    WATCHED = ["watched", "listened", "seen", "heard"]
-    WATCHING = ["watching", "listening"]
-    if args.facet in WATCHED + WATCHING:
-        args.played = True
-
-    history_fn = sql_utils.historical_usage_items
-    if args.played:
-        history_fn = sql_utils.historical_usage
-
-    if args.facet in WATCHING:
-        print(args.facet.title() + ":")
-        tbl = history_fn(
-            args, args.frequency, "time_played", hide_deleted=args.hide_deleted, where="and coalesce(play_count, 0)=0"
-        )
-        media_printer.media_printer(args, tbl)
+    query, bindings = construct_links_query(args)
+    media = list(args.db.query(query, bindings))
 
-        process_search(args, m_columns)
-        query = f"""WITH m as (
-                SELECT
-                    SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-                    , MIN(h.time_played) time_first_played
-                    , MAX(h.time_played) time_last_played
-                    , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                    , path
-                    {', title' if 'title' in m_columns else ''}
-                    {', duration' if 'duration' in m_columns else ''}
-                    {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                FROM {args.table} m
-                JOIN history h on h.media_id = m.id
-                WHERE 1=1
-                {'AND COALESCE(time_deleted, 0)=0' if args.hide_deleted else ""}
-                GROUP BY m.id, m.path
-            )
-            SELECT *
-            FROM m
-            WHERE 1=1
-                and playhead > 60
-                and coalesce(play_count, 0) = 0
-            ORDER BY time_last_played desc, playhead desc
-            LIMIT {args.limit or 5}
-        """
-        tbl = list(args.db.query(query, args.filter_bindings))
-        remove_duplicate_data(tbl)
-        media_printer.media_printer(args, tbl)
-
-    elif args.facet in WATCHED:
-        print(args.facet.title() + ":")
-        tbl = history_fn(
-            args, args.frequency, "time_played", hide_deleted=args.hide_deleted, where="and coalesce(play_count, 0)>0"
-        )
-        media_printer.media_printer(args, tbl)
+    if args.related >= consts.RELATED:
+        media = db_media.get_related_media(args, media[0])
 
-        process_search(args, m_columns)
-        query = f"""WITH m as (
-                SELECT
-                    SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-                    , MIN(h.time_played) time_first_played
-                    , MAX(h.time_played) time_last_played
-                    , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                    , path
-                    {', title' if 'title' in m_columns else ''}
-                    {', duration' if 'duration' in m_columns else ''}
-                    {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                FROM {args.table} m
-                JOIN history h on h.media_id = m.id
-                WHERE 1=1
-                {'AND COALESCE(time_deleted, 0)=0' if args.hide_deleted else ""}
-                GROUP BY m.id, m.path
-            )
-            SELECT *
-            FROM m
-            WHERE play_count > 0
-            ORDER BY time_last_played desc, path
-            LIMIT {args.limit or 5}
-        """
-        tbl = list(args.db.query(query, args.filter_bindings))
-        remove_duplicate_data(tbl)
-        media_printer.media_printer(args, tbl)
+    if args.cluster_sort:
+        from xklb.text.cluster_sort import cluster_dicts
 
-    else:
-        print(f"{args.facet.title()} media:")
-        tbl = history_fn(args, args.frequency, f"time_{args.facet}", args.hide_deleted)
-        media_printer.media_printer(args, tbl)
-        tbl = recent_media(args, f"time_{args.facet}")
-        remove_duplicate_data(tbl)
-        media_printer.media_printer(args, tbl)
+        media = cluster_dicts(args, media)[: args.limit]
+
+    media = make_souffle(args, media)
+
+    if args.print:
+        media_printer.media_printer(args, media)
+        return
+
+    if not media:
+        processes.no_media_found()
 
+    for m in media:
+        play(args, m["path"], m["url"])
 
-if __name__ == "__main__":
-    history()
+        sleep(0.1)
+        if len(media) >= consts.MANY_LINKS:
+            sleep(0.7)
```

### Comparing `xklb-2.6.9/xklb/mediadb/optimize_db.py` & `xklb-2.7.5/xklb/mediadb/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/mediadb/playlists.py` & `xklb-2.7.5/xklb/mediadb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/mediadb/redownload.py` & `xklb-2.7.5/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/mediadb/search.py` & `xklb-2.7.5/xklb/mediadb/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse, textwrap
 from copy import deepcopy
 from itertools import groupby
 
-from xklb import db_media, media_printer, usage
+from xklb import media_printer, usage
+from xklb.mediadb import db_media
 from xklb.playback import media_player
 from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, printing, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library search", usage=usage.search)
```

### Comparing `xklb-2.6.9/xklb/mediafiles/media_check.py` & `xklb-2.7.5/xklb/mediafiles/media_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse, fractions, json, os, shlex, subprocess, tempfile
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
+from shutil import which
 
 from xklb import usage
 from xklb.utils import arggroups, consts, file_utils, nums, objects, printing, processes, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args():
@@ -22,14 +23,16 @@
         args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def decode_quick_scan(path, scans, scan_duration=3):
+    assert which("ffmpeg")
+
     def decode(scan):
         proc = processes.cmd(
             "ffmpeg",
             "-nostdin",
             "-nostats",
             "-xerror",
             "-v",
@@ -53,15 +56,15 @@
     with ThreadPoolExecutor(max_workers=4) as pool:
         futures = [pool.submit(decode, scan) for scan in scans]
 
     fail_count = 0
     for future in futures:
         try:
             future.result()
-        except RuntimeError:
+        except (RuntimeError, subprocess.CalledProcessError):
             fail_count += 1
 
     return fail_count / len(scans)
 
 
 def decode_full_scan(path, audio_scan=False, frames="frames", threads=5):
     ffprobe = processes.FFProbe(path)
```

### Comparing `xklb-2.6.9/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.7.5/xklb/mediafiles/process_ffmpeg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import argparse, json, os, shlex, subprocess
+import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
+from xklb.mediafiles import process_image
 from xklb.utils import arggroups, nums, objects, path_utils, processes, web
 from xklb.utils.arg_utils import kwargs_overwrite
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library process-ffmpeg", usage=usage.process_ffmpeg)
@@ -20,32 +21,66 @@
     args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
     args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
+def is_animation_from_probe(probe) -> bool:
+    if probe.audio_streams:
+        return True
+    for stream in probe.video_streams:
+        frames = nums.safe_int(stream["nb_frames"])
+        if frames is None:
+            r = processes.cmd(
+                "ffprobe",
+                "-nostdin",
+                "-v",
+                "error",
+                "-count_frames",
+                "-select_streams",
+                "v:0",
+                "-show_entries",
+                "stream=nb_read_frames",
+                "-of",
+                "default=nokey=1:noprint_wrappers=1",
+                probe.path,
+            )
+            frames = nums.safe_int(r.stdout)
+            if frames is None:
+                raise RuntimeError
+
+        if frames > 1:
+            return True
+
+    return False
+
+
 def process_path(args, path, **kwargs):
-    args = kwargs_overwrite(args, kwargs)
+    if kwargs:
+        args = kwargs_overwrite(args, kwargs)
 
-    output_path = Path(web.url_to_local_path(path) if path.startswith("http") else path)
+    output_path = Path(web.url_to_local_path(path) if str(path).startswith("http") else path)
     output_path = Path(path_utils.clean_path(bytes(output_path), max_name_len=251))
 
     path = Path(path)
     original_stats = path.stat()
+    probe = processes.FFProbe(path)
 
-    ffprobe_cmd = ["ffprobe", "-v", "error", "-print_format", "json", "-show_format", "-show_streams", path]
-    result = subprocess.run(ffprobe_cmd, capture_output=True)
-    info = json.loads(result.stdout)
-
-    if "streams" not in info:
+    if not probe.streams:
         log.error("No media streams found: %s", path)
         return path
-    video_stream = next((stream for stream in info["streams"] if stream["codec_type"] == "video"), None)
-    audio_stream = next((stream for stream in info["streams"] if stream["codec_type"] == "audio"), None)
+
+    if path.suffix.lower() in (".gif", ".png", ".apng", ".webp", ".avif", ".avifs", ".flif", ".mng"):
+        is_animation = is_animation_from_probe(probe)
+        if not is_animation:
+            return process_image.process_path(args, path)
+
+    video_stream = next((s for s in probe.video_streams), None)
+    audio_stream = next((s for s in probe.audio_streams), None)
     if not video_stream:
         log.warning("No video stream found: %s", path)
         if args.delete_no_video:
             path.unlink()
             return None
     if not audio_stream:
         log.warning("No audio stream found: %s", path)
@@ -64,60 +99,61 @@
     if path == output_path:
         log.error("Input and output files have the same names %s", path)
         return path
 
     ff_opts: list[str] = []
 
     if video_stream:
-        ff_opts.extend(["-c:v libsvtav1", "-preset 8 -crf 44"])
+        ff_opts.extend(["-c:v", "libsvtav1", "-preset", "8", "-crf", "44"])
 
         width = int(video_stream.get("width"))
         height = int(video_stream.get("height"))
 
         if width > (args.max_width * (1 + args.max_width_buffer)):
-            ff_opts.extend([f"-vf 'scale=-2:min(iw\\,{args.max_width})'"])
+            ff_opts.extend(["-vf", "scale=-2:min(iw\\,{args.max_width})"])
         elif height > (args.max_height * (1 + args.max_height_buffer)):
-            ff_opts.extend([f"-vf 'scale=-2:min(ih\\,{args.max_height})'"])
+            ff_opts.extend(["-vf", "scale=-2:min(ih\\,{args.max_height})"])
+        # TODO: Source Width,Height must be even for YUV_420 colorspace
 
     is_split = bool(audio_stream)
     if audio_stream:
         channels = audio_stream.get("channels") or 2
-        bitrate = int(audio_stream.get("bit_rate") or info["format"].get("bit_rate") or 256000)
+        bitrate = int(audio_stream.get("bit_rate") or probe.format.get("bit_rate") or 256000)
         source_rate = int(audio_stream.get("sample_rate") or 44100)
 
-        duration = float(audio_stream.get("duration") or info["format"].get("duration") or 0)
+        duration = float(audio_stream.get("duration") or probe.format.get("duration") or 0)
         is_split = args.always_split or (args.split_longer_than and duration > args.split_longer_than)
 
         try:
             assert bitrate > 0
             assert channels > 0
             assert source_rate > 0
         except AssertionError:
             log.exception("Broken file or audio format misdetected: %s", path)
             if args.delete_no_audio:
                 path.unlink()
                 return None
         else:
             if channels == 1:
-                ff_opts.extend(["-ac 1"])
+                ff_opts.extend(["-ac", "1"])
             else:
-                ff_opts.extend(["-ac 2"])
+                ff_opts.extend(["-ac", "2"])
 
             if bitrate >= 256000:
-                ff_opts.extend(["-b:a 128k"])
+                ff_opts.extend(["-b:a", "128k"])
             else:
-                ff_opts.extend(["-b:a 64k", "-frame_duration 40"])
+                ff_opts.extend(["-b:a", "64k", "-frame_duration", "40"])
 
             if source_rate >= 44100:
                 opus_rate = 48000
             elif source_rate >= 22050:
                 opus_rate = 24000
             else:
                 opus_rate = 16000
-            ff_opts.extend(["-c:a libopus", f"-ar {opus_rate}", "-filter:a loudnorm=i=-18:tp=-3:lra=17"])
+            ff_opts.extend(["-c:a", "libopus", "-ar", str(opus_rate), "-filter:a", "loudnorm=i=-18:tp=-3:lra=17"])
 
         if is_split:
             try:
                 result = subprocess.check_output(
                     [
                         "ffmpeg",
                         "-v",
@@ -152,44 +188,75 @@
                     final_splits.append(str(split))
                     prev = split
 
             if final_splits:
                 output_path = path.with_suffix(".%03d" + output_suffix)
                 final_splits = ",".join(final_splits)
                 print(f"Splitting {path} at points: {final_splits}")
-                ff_opts.extend(["-f segment", f"-segment_times {final_splits}"])
+                ff_opts.extend(["-f", "segment", "-segment_times", final_splits])
             else:
                 is_split = False
 
-    cmd = f'ffmpeg -nostdin -hide_banner -loglevel warning -y -i {shlex.quote(str(path))} {" ".join(ff_opts)} {shlex.quote(str(output_path))}'
+    if path.parent != output_path.parent:
+        log.warning("Output folder will be different due to path cleaning: %s", output_path.parent)
+        output_path.parent.mkdir(exist_ok=True, parents=True)
+
+    command = [
+        "ffmpeg",
+        "-nostdin",
+        "-hide_banner",
+        "-loglevel",
+        "warning",
+        "-y",
+        "-i",
+        str(path),
+        *ff_opts,
+        str(output_path),
+    ]
+
     if args.simulate:
-        print(cmd)
+        print(shlex.join(command))
         return path
     else:
         try:
-            processes.cmd(cmd, shell=True)
+            processes.cmd(*command)
         except subprocess.CalledProcessError:
             log.exception("Could not transcode: %s", path)
             if args.delete_unplayable:
                 path.unlink()
                 return None
             else:
                 raise
 
-        if video_stream and (not args.audio_only or (args.audio_only and args.no_preserve_video)):
-            path.unlink()  # Remove original
-        elif is_split:
-            path.unlink()  # Remove original
-            return path.with_suffix(".000" + output_suffix)  # TODO: return multiple paths...
-        elif output_path.stat().st_size > path.stat().st_size:
+        if is_split:
+            output_path = output_path.with_name(
+                output_path.name.replace(".%03d", ".000")
+            )  # TODO: support / return multiple paths...
+
+        if not Path(output_path).exists() or output_path.stat().st_size == 0:
             output_path.unlink()  # Remove transcode
             return path
-        else:
-            path.unlink()  # Remove original
-            os.utime(output_path, (original_stats.st_atime, original_stats.st_mtime))
+
+        delete_original = True
+        delete_transcode = False
+
+        if video_stream and args.audio_only and not args.no_preserve_video:
+            delete_original = False
+
+        if output_path.stat().st_size > path.stat().st_size:
+            delete_original = False
+            delete_transcode = True
+
+        if delete_transcode:
+            output_path.unlink()
+            return path
+        elif delete_original:
+            path.unlink()
+
+        os.utime(output_path, (original_stats.st_atime, original_stats.st_mtime))
 
     return output_path
 
 
 def process_ffmpeg():
     args = parse_args()
```

### Comparing `xklb-2.6.9/xklb/mediafiles/process_image.py` & `xklb-2.7.5/xklb/mediafiles/process_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,38 +7,52 @@
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library process-image", usage=usage.process_image)
     arggroups.capability_simulate(parser)
     parser.add_argument("--delete-unplayable", action="store_true")
+
+    parser.add_argument("--max-image-height", type=int, default=2400)
+    parser.add_argument("--max-image-width", type=int, default=2400)
     arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def process_path(args, path):
-    if path.startswith("http"):
+    if str(path).startswith("http"):
         output_path = Path(web.url_to_local_path(path))
     else:
         output_path = Path(path)
     output_path = Path(path_utils.clean_path(bytes(output_path.with_suffix(".avif"))))
 
     path = Path(path)
     if path == output_path:
         output_path = Path(path).with_suffix(".r.avif")
         if path == output_path:
             log.error("Input and output files must have different names %s", path)
             return path
 
-    command = ["magick", "convert", "-resize", "2400>", str(path), str(output_path)]
+    if path.parent != output_path.parent:
+        log.warning("Output folder will be different due to path cleaning: %s", output_path.parent)
+        output_path.parent.mkdir(exist_ok=True, parents=True)
+
+    command = [
+        "magick",
+        "convert",
+        "-resize",
+        f"{args.max_image_width}x{args.max_image_height}>",
+        str(path),
+        str(output_path),
+    ]
 
     if args.simulate:
         print(shlex.join(command))
         return path
 
     original_stats = path.stat()
 
@@ -62,14 +76,18 @@
             return path
         elif args.delete_unplayable and not is_env_error and is_image_error:
             path.unlink()
             return None
         else:
             raise
 
+    if not Path(output_path).exists() or output_path.stat().st_size == 0:
+        output_path.unlink()  # Remove transcode
+        return path
+
     if output_path.stat().st_size > path.stat().st_size:
         output_path.unlink()  # Remove transcode
         return path
     else:
         path.unlink()  # Remove original
         os.utime(output_path, (original_stats.st_atime, original_stats.st_mtime))
```

### Comparing `xklb-2.6.9/xklb/misc/dedupe_czkawka.py` & `xklb-2.7.5/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/misc/export_text.py` & `xklb-2.7.5/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/multidb/copy_play_counts.py` & `xklb-2.7.5/xklb/multidb/copy_play_counts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from pathlib import Path
 
-from xklb import history, usage
+from xklb import usage
 from xklb.editdb import dedupe_db
+from xklb.mediadb import db_history
 from xklb.utils import arggroups, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("--source-prefix", default="")
@@ -46,26 +47,26 @@
             """,
         ),
     )
 
     log.info(len(copy_counts))
     for d in copy_counts:
         renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
-        history.add(
+        db_history.add(
             args,
             [renamed_path],
             time_played=d.get("time_played"),
             playhead=d.get("playhead"),
             mark_done=d["done"],
         )
 
 
 def copy_play_counts() -> None:
     args = parse_args()
-    history.create(args)
+    db_history.create(args)
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
     dedupe_db.dedupe_rows(args, "history", ["id"], ["media_id", "time_played"])
 
 
 if __name__ == "__main__":
     copy_play_counts()
```

### Comparing `xklb-2.6.9/xklb/multidb/merge_dbs.py` & `xklb-2.7.5/xklb/multidb/merge_dbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse
+import argparse, sqlite3
 from pathlib import Path
 
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, db_utils, objects
 from xklb.utils.log_utils import log
 
 
@@ -30,29 +30,26 @@
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
-    if args.where:
-        args.where = " and ".join(args.where)
-
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
 
-    s_db = db_utils.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
+    s_db = db_utils.connect(args, conn=sqlite3.connect(args.database))
     for table in [s for s in s_db.table_names() if "_fts" not in s and not s.startswith("sqlite_")]:
         if args.only_tables and table not in args.only_tables:
             log.info("[%s]: Skipping %s", source_db, table)
             continue
         else:
             log.info("[%s]: %s", source_db, table)
 
@@ -73,15 +70,15 @@
         kwargs = {}
         if args.business_keys or args.primary_keys:
             source_table_pks = [s for s in (args.business_keys or args.primary_keys) if s in selected_columns]
             if source_table_pks:
                 log.info("[%s]: Using %s as primary key(s)", table, ", ".join(source_table_pks))
                 kwargs["pk"] = source_table_pks
 
-        data = s_db[table].rows_where(where=args.where)
+        data = s_db[table].rows_where(where=" and ".join(args.where) if args.where else None)
         data = ({k: v for k, v in d.items() if k in selected_columns} for d in data)
         with args.db.conn:
             args.db[table].insert_all(
                 data,
                 alter=True,
                 ignore=args.ignore,
                 replace=not args.ignore,
```

### Comparing `xklb-2.6.9/xklb/playback/links_open.py` & `xklb-2.7.5/xklb/playback/tabs_open.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,210 +1,178 @@
-import argparse, shlex, webbrowser
+import argparse, math, webbrowser
 from pathlib import Path
 from time import sleep
 
-from xklb import db_media, history, media_printer, usage
-from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes, web
+from xklb import media_printer, usage
+from xklb.mediadb import db_history
+from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes
 from xklb.utils.log_utils import log
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library open-links",
+        prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        usage=usage.links_open,
+        usage=usage.tabs_open,
     )
-    arggroups.sql_fs(parser)
-
-    parser.add_argument("--path", action="store_true")
-    parser.add_argument("--title", action="store_true")
-    parser.add_argument("--title-prefix", "--prefix", nargs="+", action="extend")
-
-    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument("--category", "-c")
-
-    arggroups.operation_cluster(parser)
-    arggroups.operation_related(parser)
 
-    parser.add_argument("--browser")
+    arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
-    args.action = consts.SC.links_open
-    args.defaults = []
-
-    arg_utils.parse_args_limit(args)
+    args.action = action
 
     args.include += args.search
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
 
-    if not args.title_prefix:
-        args.title_prefix = ["https://www.google.com/search?q=%"]
-    args.title_prefix = [s if "%" in s else s + "%" for s in args.title_prefix]
-
-    if args.browser:
-        args.browser = shlex.split(args.browser)
-
     if args.sort:
         args.sort = [arg_utils.override_sort(s) for s in args.sort]
         args.sort = " ".join(args.sort)
 
     if args.cols:
         args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def links_include_sql(x) -> str:
+def tabs_include_sql(x) -> str:
     return f"""and (
     path like :include{x}
-    OR title like :include{x}
+    OR category like :include{x}
+    OR frequency like :include{x}
 )"""
 
 
-def links_exclude_sql(x) -> str:
+def tabs_exclude_sql(x) -> str:
     return f"""and (
     path not like :exclude{x}
-    AND title not like :exclude{x}
+    AND category not like :exclude{x}
+    AND frequency not like :exclude{x}
 )"""
 
 
-def construct_links_query(args) -> tuple[str, dict]:
-    m_columns = db_utils.columns(args, "media")
-
+def construct_tabs_query(args) -> tuple[str, dict]:
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     for idx, inc in enumerate(args.include):
-        args.filter_sql.append(links_include_sql(idx))
+        args.filter_sql.append(tabs_include_sql(idx))
         if args.exact:
             args.filter_bindings[f"include{idx}"] = inc
         else:
             args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
-        args.filter_sql.append(links_exclude_sql(idx))
+        args.filter_sql.append(tabs_exclude_sql(idx))
         if args.exact:
             args.filter_bindings[f"exclude{idx}"] = exc
         else:
             args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
-    if args.category:
-        args.filter_sql.append("AND category like :category")
-        if args.exact:
-            args.filter_bindings[f"category"] = args.category
-        else:
-            args.filter_bindings[f"category"] = "%" + args.category.replace(" ", "%").replace("%%", " ") + "%"
-
-    limit_sql = "LIMIT " + str(args.limit) if args.limit and not args.cluster_sort else ""
-    offset_sql = f"OFFSET {args.offset}" if args.offset and limit_sql else ""
-
-    args.select = ["path"]
-    if args.cols:
-        args.select.extend(args.cols)
-    for s in ["title", "hostname", "category"]:
-        if s in m_columns:
-            args.select.append(s)
+    LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
+    OFFSET = f"OFFSET {args.offset}" if args.offset else ""
 
     query = f"""WITH m as (
             SELECT
-                {', '.join(args.select) if args.select else ''}
+                path
+                , frequency
                 , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , time_deleted
+                , hostname
+                , category
             FROM media
             LEFT JOIN history h on h.media_id = media.id
             WHERE COALESCE(time_deleted, 0)=0
             GROUP BY media.id
         )
-        SELECT
-        {', '.join(args.select) if args.select else ''}
+        SELECT path
+        , frequency
         {", time_last_played" if args.print else ''}
+        , CASE
+            WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Day', '-5 minutes' )) as int)
+            WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+7 Days', '-5 minutes' )) as int)
+            WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Month', '-5 minutes' )) as int)
+            WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+3 Months', '-5 minutes' )) as int)
+            WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Year', '-5 minutes' )) as int)
+        END time_valid
+        {', ' + ', '.join(args.cols) if args.cols else ''}
     FROM m
     WHERE 1=1
-        AND COALESCE(time_deleted, 0)=0
-        {'AND path like "http%"' if args.online_media_only else ''}
-        {'AND path not like "http%"' if args.local_media_only else ''}
         {" ".join(args.filter_sql)}
+        {f"and time_valid < {consts.today_stamp()}" if not args.print else ''}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
+        {', time_last_played, time_valid, path' if args.print else ''}
         , play_count
-        {', ROW_NUMBER() OVER ( PARTITION BY hostname )' if 'hostname' in m_columns else ''}
-        {', ROW_NUMBER() OVER ( PARTITION BY category )' if 'category' in m_columns else ''}
+        , frequency = 'daily' desc
+        , frequency = 'weekly' desc
+        , frequency = 'monthly' desc
+        , frequency = 'quarterly' desc
+        , frequency = 'yearly' desc
+        , ROW_NUMBER() OVER ( PARTITION BY
+            play_count
+            , frequency
+            , hostname
+            , category
+        ) -- prefer to spread hostname, category over time
         , random()
-    {limit_sql} {offset_sql}
+    {LIMIT} {OFFSET}
     """
 
     return query, args.filter_bindings
 
 
-def play(args, path, url) -> None:
-    if args.browser:
-        processes.cmd(*args.browser, url)
-    else:
-        webbrowser.open(url, 2, autoraise=False)
-    history.add(args, [path], time_played=consts.today_stamp(), mark_done=True)
+def play(args, m: dict) -> None:
+    media_file = m["path"]
 
+    webbrowser.open(media_file, 2, autoraise=False)
+    db_history.add(args, [media_file], time_played=consts.today_stamp(), mark_done=True)
 
-def make_souffle(args, media):
-    pan = []
 
-    urls = set()
-    for m in media:
-        m_urls = set()
-        if args.title:
-            for engine in args.title_prefix:
-                suffix = m.get("title") or m["path"]
-                m_urls.add(suffix if suffix.startswith("http") else web.construct_search(engine, suffix))
-
-        if not args.title or args.path:
-            if not m["path"].startswith("http"):
-                for engine in args.title_prefix:
-                    m_urls.add(web.construct_search(engine, m["path"]))
-            else:
-                m_urls.add(m["path"])
-
-        pan.extend([{**m, "url": url} for url in m_urls if url not in urls])
-        urls |= m_urls
-
-    return pan
-
-
-def links_open() -> None:
-    args = parse_args()
-    history.create(args)
+def frequency_filter(counts, media: list[dict]) -> list[dict]:
+    mapper = {
+        "daily": 1,
+        "weekly": 7,
+        "monthly": 30,
+        "quarterly": 91,
+        "yearly": 365,
+    }
+    filtered_media = []
+    for freq, freq_count in counts:
+        num_days = mapper.get(freq, 365)
+        num_tabs = max(1, math.ceil(freq_count / num_days))
+        log.debug(f"freq_count {freq_count} / num_days {num_days} = num_tabs {num_tabs}")
 
-    query, bindings = construct_links_query(args)
-    media = list(args.db.query(query, bindings))
+        filtered_media.extend([m for m in media if m["frequency"] == freq][:num_tabs])
 
-    if args.related >= consts.RELATED:
-        media = db_media.get_related_media(args, media[0])
+    return filtered_media
 
-    if args.cluster_sort:
-        from xklb.text.cluster_sort import cluster_dicts
 
-        media = cluster_dicts(args, media)[: args.limit]
+def tabs_open() -> None:
+    args = parse_args(consts.SC.tabs_open)
+    db_history.create(args)
 
-    media = make_souffle(args, media)
+    query, bindings = construct_tabs_query(args)
 
-    if args.print:
-        media_printer.media_printer(args, media)
+    if args.print or args.delete_rows or args.mark_deleted or args.mark_watched:
+        media_printer.printer(args, query, bindings)
         return
 
+    media = list(args.db.query(query, bindings))
     if not media:
         processes.no_media_found()
 
-    for m in media:
-        play(args, m["path"], m["url"])
+    counts = args.db.execute("select frequency, count(*) from media group by 1").fetchall()
+    media = frequency_filter(counts, media)
 
-        sleep(0.1)
+    for m in media:
+        play(args, m)
         if len(media) >= consts.MANY_LINKS:
-            sleep(0.7)
+            sleep(0.3)
```

### Comparing `xklb-2.6.9/xklb/playback/media_player.py` & `xklb-2.7.5/xklb/playback/media_player.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import argparse, platform, shutil, subprocess, threading, time
+import os, platform, shutil, subprocess, threading, time
+from argparse import Namespace
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from platform import system
 from random import randrange
 from shutil import which
 from time import sleep
 
-from xklb import db_media, history
 from xklb.createdb import subtitle
+from xklb.mediadb import db_history, db_media
 from xklb.playback import playback_control, post_actions
 from xklb.utils import consts, db_utils, devices, iterables, log_utils, mpv_utils, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def watch_chromecast(args, m: dict, subtitles_file=None) -> subprocess.CompletedProcess | None:
@@ -365,15 +366,15 @@
     log.debug(players)
 
     return players
 
 
 class MediaPrefetcher:
     def __init__(self, args, media: list[dict]):
-        self.args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
+        self.args = Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
         self.media = media
         self.media.reverse()
         self.remaining = len(media)
         self.ignore_paths = set()
         self.futures = deque()
 
     def fetch(self):
@@ -397,14 +398,17 @@
         player = generic_player()
         player_need_sleep = True
 
         if getattr(args, "override_player", False):
             player = [*args.override_player]
             player_need_sleep = False
 
+        elif getattr(args, "folders", False):
+            player_need_sleep = True
+
         elif args.action in (SC.read):
             if system() == "Linux":
                 player_path = find_xdg_application(m["path"])
                 if player_path:
                     player_need_sleep = False
                     player = [player_path]
 
@@ -416,15 +420,16 @@
                 if args.action in (SC.listen):
                     player.extend(
                         [f"--input-ipc-server={args.mpv_socket}", "--video=no", "--keep-open=no", "--really-quiet=yes"]
                     )
                 elif args.action in (SC.watch):
                     player.extend(["--force-window=yes", "--really-quiet=yes"])
 
-                if getattr(args, "multiple_playback", 1) < 2:
+                multiple_playback = getattr(args, "multiple_playback", None)
+                if multiple_playback and multiple_playback < 2:
                     player.extend(["--fullscreen=yes"])
 
                 if getattr(args, "loop", False):
                     player.extend(["--loop-file=inf"])
 
                 if getattr(args, "pause", False):
                     player.extend(["--pause=yes"])
@@ -482,16 +487,20 @@
                 db_media.mark_media_deleted(self.args, m["original_path"])
                 return {}
 
             if self.args.transcode or self.args.transcode_audio:
                 m["path"] = m["original_path"] = transcode(self.args, m["path"])
                 log.debug("transcode: %s", t.elapsed())
 
-        m["now_playing"] = playback_control.now_playing(m["path"])
+        if self.args.folders:
+            m["now_playing"] = m["path"]
+        else:
+            m["now_playing"] = playback_control.now_playing(m["path"])
         log.debug("playback_control: %s", t.elapsed())
+
         m["player"], m["player_need_sleep"] = self.infer_command(m)
         log.debug("player.parse: %s", t.elapsed())
 
         return m
 
     def get_m(self):
         m = None
@@ -516,22 +525,35 @@
 
         self.remaining = len(self.media) + len(self.futures)
         self.fetch()
         return m
 
 
 def single_player(args, m):
-    if system() == "Windows" or args.action in (SC.watch):
-        r = processes.cmd(*m["player"], m["path"], strict=False)
-    else:  # args.action in (SC.listen)
-        r = processes.cmd_interactive(*m["player"], m["path"], strict=False)
+    is_windows = system() == "Windows"
+
+    if args.folders:
+        if args.override_player:
+            r = processes.cmd(*m["player"], m["path"], strict=False)
+        elif is_windows:
+            os.startfile(m["path"])  # type: ignore
+        elif which("open"):
+            r = processes.cmd("open", m["path"], strict=False)
+        else:
+            r = processes.cmd("xdg-open", m["path"], strict=False)
+    else:
+        if is_windows or args.action in (SC.watch):
+            r = processes.cmd(*m["player"], m["path"], strict=False)
+        else:  # args.action in (SC.listen)
+            r = processes.cmd_interactive(*m["player"], m["path"], strict=False)
 
     if m["player_need_sleep"]:
         try:
-            devices.confirm("Continue?")
+            if not devices.confirm("Continue?"):
+                raise SystemExit(0)
         except Exception:
             log.exception("Could not open prompt")
             delay = 10  # TODO: idk
             sleep(delay)
     return r
 
 
@@ -661,15 +683,15 @@
             m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
         )
         log.debug("save_playhead %s", playhead)
         if playhead:
-            history.add(args, [m["original_path"]], playhead=playhead)
+            db_history.add(args, [m["original_path"]], playhead=playhead)
 
 
 def play_list(args, media):
     try:
         playlist = MediaPrefetcher(args, media)
         playlist.fetch()
```

### Comparing `xklb-2.6.9/xklb/playback/play_actions.py` & `xklb-2.7.5/xklb/playback/play_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse, os, shlex, sys
 from pathlib import Path
 
-from xklb import db_media, history, media_printer, usage
+from xklb import media_printer, usage
 from xklb.createdb import tube_backend
 from xklb.fsdb import big_dirs
+from xklb.mediadb import db_history, db_media
 from xklb.playback import media_player
 from xklb.tablefiles import mcda
 from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, nums, objects, processes, sql_utils
 from xklb.utils.arg_utils import parse_args_limit, parse_args_sort
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import Timer, log
 
@@ -37,16 +38,14 @@
         default=default_chromecast or "",
         help=argparse.SUPPRESS,
     )
     parser.add_argument("--chromecast", "--cast", "-c", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--cast-with-local", "-wl", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--interdimensional-cable", "-4dtv", type=int, help=argparse.SUPPRESS)
 
-    parser.add_argument("--moved", nargs=2, help=argparse.SUPPRESS)
-
     parser.add_argument(
         "--partial",
         "-P",
         "--previous",
         "--recent",
         default=False,
         const="n",
@@ -173,58 +172,53 @@
     if args.no_audio:
         args.filter_sql.append(" and audio_count=0 ")
     if args.subtitles:
         args.filter_sql.append(" and subtitle_count>0 ")
     if args.no_subtitles:
         args.filter_sql.append(" and subtitle_count=0 ")
 
-    def ii(string):
-        if string.isdigit():
-            return string + " minutes"
-        return string.replace("mins", "minutes").replace("secs", "seconds")
-
     if args.created_within:
         args.aggregate_filter_sql.append(
-            f"and time_created > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_within)}')) as int)",
+            f"and time_created >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.created_within)}')) as int)",
         )
     if args.created_before:
         args.aggregate_filter_sql.append(
-            f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_before)}')) as int)",
+            f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.created_before)}')) as int)",
         )
     if args.changed_within:
         args.aggregate_filter_sql.append(
-            f"and time_modified > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_within)}')) as int)",
+            f"and time_modified >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.changed_within)}')) as int)",
         )
     if args.changed_before:
         args.aggregate_filter_sql.append(
-            f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_before)}')) as int)",
+            f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.changed_before)}')) as int)",
         )
     if args.played_within:
         args.aggregate_filter_sql.append(
-            f"and time_last_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)",
+            f"and time_last_played >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.played_within)}')) as int)",
         )
     if args.played_before:
         args.aggregate_filter_sql.append(
-            f"and time_last_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)",
+            f"and time_last_played < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.played_before)}')) as int)",
         )
     if args.deleted_within:
         args.aggregate_filter_sql.append(
-            f"and time_deleted > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_within)}')) as int)",
+            f"and time_deleted >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.deleted_within)}')) as int)",
         )
     if args.deleted_before:
         args.aggregate_filter_sql.append(
-            f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)",
+            f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.deleted_before)}')) as int)",
         )
     if args.downloaded_within:
         args.aggregate_filter_sql.append(
-            f"and time_downloaded > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.downloaded_within)}')) as int)",
+            f"and time_downloaded >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.downloaded_within)}')) as int)",
         )
     if args.downloaded_before:
         args.aggregate_filter_sql.append(
-            f"and time_downloaded < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.downloaded_before)}')) as int)",
+            f"and time_downloaded < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.downloaded_before)}')) as int)",
         )
 
     args.table = "media"
     if args.db["media"].detect_fts() and not args.no_fts:
         if args.include:
             args.table, search_bindings = db_utils.fts_search_sql(
                 "media",
@@ -380,30 +374,30 @@
     if args.offset:
         media = media[int(args.offset) :]
 
     return media
 
 
 def process_playqueue(args) -> None:
-    history.create(args)
+    db_history.create(args)
 
     query, bindings = construct_query(args)
 
     if args.print and not any(
         [
             args.partial,
             args.lower,
             args.upper,
             args.safe,
             args.play_in_order,
             args.big_dirs,
             args.fetch_siblings,
             args.related,
             args.cluster_sort,
-            args.folder,
+            args.folders,
             args.folder_glob,
         ],
     ):
         media_printer.printer(args, query, bindings)
         return
 
     t = Timer()
@@ -450,15 +444,15 @@
 
     if args.related >= consts.RELATED:
         media = db_media.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
 
     if args.big_dirs:
         media_keyed = {d["path"]: d for d in media}
-        folders = big_dirs.group_files_by_folder(args, media)
+        folders = big_dirs.group_files_by_parents(args, media)
         dirs = big_dirs.process_big_dirs(args, folders)
         dirs = mcda.group_sort_by(args, dirs)
         log.debug("process_bigdirs: %s", t.elapsed())
         dirs = list(reversed([d["path"] for d in dirs]))
         if "limit" in args.defaults:
             media = db_media.get_dir_media(args, dirs)
             log.debug("get_dir_media: %s", t.elapsed())
@@ -489,16 +483,23 @@
 
     if getattr(args, "refresh", False):
         marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
         log.warning(f"Marked {marked} metadata records as deleted")
         args.refresh = False
         return process_playqueue(args)
 
-    if args.folder:
-        media = ({**m, "path": str(Path(m["path"]).parent)} for m in media)
+    if args.folders:
+        unique_folders = set()
+        media_unique_folders = []
+        for m in media:
+            folder_path = str(Path(m["path"]).parent)
+            if folder_path not in unique_folders:
+                unique_folders.add(folder_path)
+                media_unique_folders.append({**m, "path": folder_path})
+        media = media_unique_folders
     elif args.folder_glob:
         media = ({"path": s} for m in media for s in file_utils.fast_glob(Path(m["path"]).parent, args.folder_glob))
 
     if any(
         [
             args.print,
             args.delete_files,
```

### Comparing `xklb-2.6.9/xklb/playback/playback_control.py` & `xklb-2.7.5/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/playback/post_actions.py` & `xklb-2.7.5/xklb/playback/post_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re, shlex, shutil
 from pathlib import Path
 
 import humanize
 
-from xklb import db_media, history
+from xklb.mediadb import db_history, db_media
 from xklb.utils import devices, file_utils, iterables, processes
 from xklb.utils.log_utils import log
 
 try:
     import tkinter  # noqa
 
     from xklb.utils import gui
@@ -168,15 +168,15 @@
                 log.warning("%s: %s (%s remaining)", confirmed_action, media_file, media_len)
             else:
                 log.warning("%s: %s", confirmed_action, media_file)
 
     player_exit_code = getattr(player_process, "returncode", None) or 0
 
     if record_history and player_exit_code == 0:
-        history.add(args, [media_file], mark_done=True)
+        db_history.add(args, [media_file], mark_done=True)
 
     if 0 < player_exit_code < 5 and not args.ignore_errors:
         if args.delete_unplayable and player_exit_code == 2:  #  https://mpv.io/manual/master/#exit-codes
             delete_media(args, [media_file])
         else:
             processes.player_exit(player_process)
```

### Comparing `xklb-2.6.9/xklb/playback/surf.py` & `xklb-2.7.5/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/scratch/javguru.py` & `xklb-2.7.5/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/scratch/javtiful.py` & `xklb-2.7.5/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/scratch/mam_search.py` & `xklb-2.7.5/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/scratch/mam_slots.py` & `xklb-2.7.5/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/tablefiles/eda.py` & `xklb-2.7.5/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/tablefiles/incremental_diff.py` & `xklb-2.7.5/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/tablefiles/mcda.py` & `xklb-2.7.5/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/text/cluster_sort.py` & `xklb-2.7.5/xklb/text/cluster_sort.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse, difflib, json, os.path, sys
-from collections import Counter
 from pathlib import Path
 
 from xklb import usage
 from xklb.data import wordbank
 from xklb.tablefiles import eda, mcda
-from xklb.utils import arggroups, consts, db_utils, file_utils, iterables, nums, objects, printing, strings
+from xklb.utils import arggroups, consts, db_utils, file_utils, iterables, nums, objects, path_utils, printing, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
 
@@ -80,38 +79,21 @@
         if cluster_id not in grouped_strings:
             grouped_strings[cluster_id] = []
 
         grouped_strings[cluster_id].append(group_string)
     return grouped_strings
 
 
-def group_paths(paths, clusters):
+def map_and_name(paths, clusters):
     grouped_strings = map_cluster_to_paths(paths, clusters)
 
     result = []
     for _cluster_id, paths in grouped_strings.items():
         paths = sorted(paths)
-        common_prefix = os.path.commonprefix(paths)
-
-        suffix_words = []
-        for path in paths:
-            suffix = path[len(common_prefix) :]
-            words = list(iterables.ordered_set(strings.path_to_sentence(suffix).split()))
-            suffix_words.extend(words)
-
-        word_counts = Counter(suffix_words)
-        common_words = [w for w, c in word_counts.items() if c > int(len(paths) * 0.6) and len(w) > 1]
-
-        # join but preserve order
-        suffix = "*".join(s for s in iterables.ordered_set(suffix_words) if s in common_words)
-
-        metadata = {
-            "common_prefix": common_prefix.strip() + "*" + suffix,
-            "grouped_paths": paths,
-        }
+        metadata = {"common_path": path_utils.common_path(paths), "grouped_paths": paths}
         result.append(metadata)
     return result
 
 
 def find_clusters(n_clusters, sentence_strings, stop_words=None):
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
@@ -138,15 +120,15 @@
 
 def cluster_paths(paths, n_clusters=None, stop_words=None):
     if len(paths) < 2:
         return paths
 
     sentence_strings = (strings.path_to_sentence(s) for s in paths)
     clusters = find_clusters(n_clusters, sentence_strings, stop_words=stop_words)
-    result = group_paths(paths, clusters)
+    result = map_and_name(paths, clusters)
 
     return result
 
 
 def print_groups(groups):
     for group in groups:
         group["grouped_paths"] = [s.rstrip("\n") for s in group["grouped_paths"]]
@@ -176,16 +158,16 @@
     clusters = find_clusters(n_clusters, sentence_strings, stop_words=getattr(args, "stop_words", None))
 
     if args.verbose >= consts.LOG_INFO:
         from pandas import DataFrame
 
         eda.print_info(objects.NoneSpace(end_row="inf"), DataFrame(clusters))
 
-    groups = group_paths(paths, clusters)
-    groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
+    groups = map_and_name(paths, clusters)
+    groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
 
     if getattr(args, "sort_groups_by", None) is not None:
         if args.sort_groups_by in ("duration", "duration desc"):
             sorted_paths = iterables.flatten(
                 sorted(d["grouped_paths"], key=lambda p: media_keyed[p]["duration"], reverse=" desc" in args.sort)
                 for d in groups
             )
@@ -287,18 +269,15 @@
 
         grouped_strings[cluster_id].append(group_string + "\n")
     log.info("grouped_strings %s", t.elapsed())
 
     result = []
     for _cluster_id, paths in grouped_strings.items():
         common_prefix = os.path.commonprefix(paths)
-        metadata = {
-            "common_prefix": common_prefix,
-            "grouped_paths": sorted(paths),
-        }
+        metadata = {"common_path": common_prefix, "grouped_paths": sorted(paths)}
         result.append(metadata)
     log.info("common_prefix %s", t.elapsed())
 
     return result
 
 
 def filter_near_duplicates(groups: list[dict]) -> list[dict]:
@@ -318,16 +297,16 @@
                     is_duplicate = True
                     break
             if not is_duplicate:
                 temp_groups[curr] = []
 
         sorted_temp_groups = sorted(temp_groups.items(), key=lambda t: len(t[1]))
         for new_group_idx, (path, similar_paths) in enumerate(sorted_temp_groups):
-            new_group_name = group["common_prefix"] + f"#{new_group_idx}"
-            regrouped_data.append({"common_prefix": new_group_name, "grouped_paths": [path] + similar_paths})
+            new_group_name = group["common_path"] + f"#{new_group_idx}"
+            regrouped_data.append({"common_path": new_group_name, "grouped_paths": [path] + similar_paths})
 
     return regrouped_data
 
 
 def cluster_sort() -> None:
     args = parse_args()
 
@@ -336,15 +315,15 @@
 
     if args.profile == "lines":
         groups = cluster_paths(lines, args.clusters, args.stop_words)
     elif args.profile == "image":
         groups = cluster_images(lines, args.clusters)
     else:
         raise NotImplementedError
-    groups = sorted(groups, key=lambda d: (len(d["grouped_paths"]), -len(d["common_prefix"])))
+    groups = sorted(groups, key=lambda d: (len(d["grouped_paths"]), -len(d["common_path"])))
 
     if args.near_duplicates:
         groups = filter_near_duplicates(groups)
 
     if args.exclude_unique:
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
     elif args.unique_only:
```

### Comparing `xklb-2.6.9/xklb/text/extract_links.py` & `xklb-2.7.5/xklb/text/extract_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     return True
 
 
 def parse_inner_urls(args, url, markup):
     from bs4 import BeautifulSoup
 
-    soup = BeautifulSoup(markup, "html.parser")
+    soup = BeautifulSoup(markup, "lxml")
 
     for a_ref in soup.findAll(href=True):
         log.debug(a_ref)
 
         href = a_ref["href"].strip()
         if (len(href) > 1) and href[0] != "#":
             link = web.construct_absolute_url(url, href).strip()
```

### Comparing `xklb-2.6.9/xklb/text/extract_text.py` & `xklb-2.7.5/xklb/text/extract_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     s = re.sub(r"[“”‘’]", "'", s)
     s = re.sub(r"[‛‟„]", '"', s)
     s = re.sub(r"[…]", "...", s)
     return s
 
 
 def parse_text(args, html_content):
-    soup = BeautifulSoup(html_content, "html.parser")
+    soup = BeautifulSoup(html_content, "lxml")
     for item in soup.find_all():
         if item.name in ["meta"]:
             continue
 
         for descendant in item.descendants:
             if isinstance(descendant, NavigableString):
                 parent = descendant.find_parent()
```

### Comparing `xklb-2.6.9/xklb/text/markdown_links.py` & `xklb-2.7.5/xklb/text/markdown_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             try:
                 if args.selenium:
                     web.selenium_get_page(args, url)
                     html_text = args.driver.page_source
                 else:
                     html_text = web.requests_session(args).get(url).text
 
-                soup = BeautifulSoup(html_text, "html.parser")
+                soup = BeautifulSoup(html_text, "lxml")
                 title = soup.title.text.strip() if soup.title else url
             except requests.exceptions.RequestException as e:
                 title = fake_title(url)
 
             if title.startswith("Stream ") and "SoundCloud" in title:
                 title = title.replace("Stream ", "", 1)
```

### Comparing `xklb-2.6.9/xklb/text/nouns.py` & `xklb-2.7.5/xklb/text/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/arggroups.py` & `xklb-2.7.5/xklb/utils/arggroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,33 @@
         help="Delete files from filesystem",
     )
 
 
 def database(parser):
     capability_soft_delete(parser)
     capability_delete(parser)
-    parser.add_argument("--db", "-db", dest="database", help="Positional argument override")
+    parser.add_argument("--db", "-db", help="Positional argument override")
     parser.add_argument("database")
 
 
 def paths_or_stdin(parser):
-    parser.add_argument("--file", "-f", help="File with one URL per line")
+    parser.add_argument(
+        "--paths-from-text",
+        "--files",
+        "--file",
+        "-f",
+        action="store_true",
+        help="Read paths from line-delimited file(s)",
+    )
+    parser.add_argument("--paths-from-dbs", "--fsdbs", "--fsdb", action="store_true", help="Read paths from db(s)")
+    parser.add_argument("--titles-from-dbs", action="store_true", help="Read titles from db(s) instead of paths")
     parser.add_argument(
         "paths", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
     )
+    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
 
 
 def sql_fs(parser):
     parser.add_argument("--print", "-p", default="", const="p", nargs="?")
     parser.add_argument("--cols", "--col", nargs="*", help="Include specific column(s) when printing")
 
     parser.add_argument("--limit", "--queue", "--count", "-n", "-L", "-l")
@@ -117,15 +127,15 @@
         "--ignore-errors",
         "--ignoreerrors",
         "-i",
         action="store_true",
         help="After a playback error continue to the next track instead of exiting",
     )
 
-    parser.add_argument("--folder", action="store_true", help="Experimental escape hatch to open folder")
+    parser.add_argument("--folders", "--folder", action="store_true", help="Experimental escape hatch to open folder")
     parser.add_argument(
         "--folder-glob",
         "--folderglob",
         type=int,
         default=False,
         const=10,
         nargs="?",
@@ -171,14 +181,15 @@
 
 def operation_group_folders(parser):
     parser.add_argument("--lower", type=int, help="Minimum number of files per folder")
     parser.add_argument("--upper", type=int, help="Maximum number of files per folder")
 
     parser.add_argument("--sort-groups-by", "--sort-groups", "--sort-by", nargs="+")
     parser.add_argument("--depth", "-D", type=int, help="Depth of folders")
+    parser.add_argument("--parents", action="store_true")
 
     parser.add_argument(
         "--folder-size",
         "--foldersize",
         "-Z",
         action="append",
         help="Only include folders of specific sizes (uses the same syntax as fd-find)",
@@ -225,14 +236,17 @@
     parser.add_argument("--always-split", "--force-split", action="store_true")
     parser.add_argument("--split-longer-than")
     parser.add_argument("--min-split-segment", default=consts.DEFAULT_MIN_SPLIT)
 
     parser.add_argument("--audio-only", "-vn", action="store_true", help="Only extract audio")
     parser.add_argument("--no-preserve-video", action="store_true")
 
+    parser.add_argument("--max-image-height", type=int, default=2400)
+    parser.add_argument("--max-image-width", type=int, default=2400)
+
 
 def download(parser):
     parser.add_argument(
         "--extractor-config",
         "-extractor-config",
         nargs=1,
         action=argparse_utils.ArgparseDict,
@@ -444,21 +458,26 @@
         "-I",
         action="append_const",
         dest="profiles",
         const=DBType.image,
         help="Extract image metadata",
     )
     parser.add_argument("--scan-all-files", "-a", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
 
 
 def frequency(parser):
     parser.add_argument(
         "--frequency",
         "--freqency",
         "-f",
         default="monthly",
         const="monthly",
         type=str.lower,
         nargs="?",
         help=f"One of: {', '.join(consts.frequency)} (default: %(default)s)",
     )
+
+
+def history(parser):
+    history = parser.add_mutually_exclusive_group()
+    history.add_argument("--completed", "--played", "--watched", "--listened", action="store_true")
+    history.add_argument("--in-progress", "--playing", "--watching", "--listening", action="store_true")
```

### Comparing `xklb-2.6.9/xklb/utils/argparse_utils.py` & `xklb-2.7.5/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/consts.py` & `xklb-2.7.5/xklb/utils/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     gallery_update = "gallery-update"
     tabs_open = "tabs-open"
     links_open = "links-open"
     read = "read"
     view = "view"
     download = "download"
     block = "block"
+    stats = "stats"
     playlists = "playlists"
     download_status = "download-status"
     search = "search"
     history = "history"
     big_dirs = "big-dirs"
     disk_usage = "disk-usage"
     dedupe_media = "dedupe"
@@ -157,21 +158,21 @@
 )
 SUBTITLE_EXTENSIONS = set("srt|vtt|mks".split("|"))
 TEXTRACT_EXTENSIONS = set(
     "csv|tab|tsv|doc|docx|eml|epub|json|htm|html|msg|odt|pdf|pptx|ps|rtf|txt|log|xlsx|xls".split("|")
 )
 IMAGE_EXTENSIONS = set(
     (
-        "pdf|ai|ait|png|jng|mng|arq|arw|cr2|cs1|dcp|dng|eps|epsf|ps|erf|exv|fff"
+        "ai|ait|png|jng|mng|arq|arw|cr2|cs1|dcp|dng|eps|epsf|ps|erf|exv|fff"
         "|gpr|hdp|wdp|jxr|iiq|insp|jpeg|jpg|jpe|mef|mie|mos|mpo|mrw|nef|nrw|orf"
         "|ori|pef|psd|psb|psdt|raf|raw|rw2|rwl|sr2|srw|thm|tiff|tif|x3f|flif|gif"
         "|icc|icm|avif|heic|heif|hif|jp2|jpf|jpm|jpx|j2c|j2k|jpc|3fr|btf|dcr|k25"
         "|kdc|miff|mif|rwz|srf|xcf|bpg|doc|dot|fla|fpx|max|ppt|pps|pot|vsd|xls"
         "|xlt|pict|pct|360|aax|dvb|f4a|f4b|f4p|f4v|lrv|m4b"
-        "|m4p|m4v|mov|qt|mqv|qtif|qti|qif|cr3|crm|jxl|crw|ciff|ind|indd|indt"
+        "|m4p|qt|mqv|qtif|qti|qif|cr3|crm|jxl|crw|ciff|ind|indd|indt"
         "|nksc|vrd|xmp|la|ofr|pac|riff|rif|wav|webp|wv|asf|divx|djvu|djv|dvr-ms"
         "|flv|insv|inx|swf|wma|wmv|exif|eip|psp|pspimage"
     ).split("|")
 )
 
 
 time_facets = [
```

### Comparing `xklb-2.6.9/xklb/utils/db_utils.py` & `xklb-2.7.5/xklb/utils/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,18 @@
                 raise
             return d
 
     if kwargs.get("memory"):
         db = DB(tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
         return db
 
+    db_override = getattr(args, "db", None)
+    if db_override and isinstance(db_override, str):
+        args.database = db_override
+
     if not Path(args.database).exists() and ":memory:" not in args.database:
         log.error(f"Database file '{args.database}' does not exist. Create one with lb fsadd, tubeadd, or tabsadd.")
         raise SystemExit(1)
 
     db = DB(conn or args.database, tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
     with db.conn:  # type: ignore
         db.conn.execute("PRAGMA main.cache_size = 8000")  # type: ignore
```

### Comparing `xklb-2.6.9/xklb/utils/devices.py` & `xklb-2.7.5/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/file_utils.py` & `xklb-2.7.5/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/gui.py` & `xklb-2.7.5/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/iterables.py` & `xklb-2.7.5/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/log_utils.py` & `xklb-2.7.5/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/mpv_utils.py` & `xklb-2.7.5/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/nums.py` & `xklb-2.7.5/xklb/utils/nums.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     if s.endswith("%"):
         v = float(s.rstrip("%")) / 100
     else:
         v = float(s)
     return v
 
 
+def percentage_difference(value1, value2):
+    try:
+        return abs((value1 - value2) / ((value1 + value2) / 2)) * 100
+    except ZeroDivisionError:
+        return 100.0
+
+
 def to_timestamp(dt_object):
     return int(dt_object.replace(tzinfo=timezone.utc).timestamp())
 
 
 def safe_int(s) -> int | None:
     if not s:
         return None
@@ -67,14 +74,20 @@
     else:
         unit = "mb"
 
     unit_multiplier = byte_map.get(unit, 1024**2)  # default to MB
     return int(float(value) * unit_multiplier)
 
 
+def sql_human_time(s):
+    if s.isdigit():
+        return s + " minutes"
+    return s.replace("mins", "minutes").replace("secs", "seconds")
+
+
 def human_to_seconds(input_str):
     if input_str is None:
         return None
 
     time_units = {
         "s": 1,
         "sec": 1,
```

### Comparing `xklb-2.6.9/xklb/utils/objects.py` & `xklb-2.7.5/xklb/utils/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 def last_item(gen):
     last = None
     for _ in gen:
         last = _
     return last
 
 
+def take(gen, num=5):
+    for value, _ in zip(gen, range(num)):
+        yield value
+
+
 def flatten_dict(nested_dict, parent_key="", sep="_", passthrough_keys=None):
     if passthrough_keys is None:
         passthrough_keys = []
     flattened_dict = {}
     for key, value in nested_dict.items():
         new_key = f"{parent_key}{sep}{key}" if parent_key else key
         if isinstance(value, dict) and key not in passthrough_keys:
@@ -75,20 +80,25 @@
         return func(obj)
     elif isinstance(obj, list):
         return [recursive_flattener(func, i) for i in obj]
     else:
         return obj
 
 
-def lower_keys(input_dict):
-    output_dict = {}
-    for key, value in input_dict.items():
-        lowercase_key = key.lower().strip()
-        output_dict[lowercase_key] = value
-    return output_dict
+def rename_key(d, from_key, to_key):
+    d[to_key] = d.pop(from_key)
+    return d
+
+
+def lower_keys(d):
+    for key in list(d.keys()):
+        lower_key = key.lower().strip()
+        if key != lower_key:
+            rename_key(d, key, lower_key)
+    return d
 
 
 def dict_filter_bool(kwargs, keep_0=True) -> dict | None:
     if kwargs is None:
         return None
 
     if keep_0:
```

### Comparing `xklb-2.6.9/xklb/utils/pd_utils.py` & `xklb-2.7.5/xklb/utils/pd_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     col = re.sub(r"[\]\[\)\(\{\}]+", "", col)
     col = re.sub(r"[\:\-\.]+", "_", col)
     col = re.sub(r"__+", "_", col)
     return col
 
 
 def columns_snake_case(df):
-    df.columns = [kebab_camel_snake(x) for x in df.columns]
+    df.columns = [kebab_camel_snake(x) if isinstance(x, str) else x for x in df.columns]
     return df
 
 
 def convert_dtypes(df, clean=False):
     for col in df.columns:
         try:
             if clean:
```

### Comparing `xklb-2.6.9/xklb/utils/printing.py` & `xklb-2.7.5/xklb/utils/printing.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     except BrokenPipeError:
         sys.stdout = None
         sys.exit(141)
 
 
 def pipe_lines(x) -> None:
     try:
-        sys.stdout.writelines(x)
+        sys.stdout.writelines(x)  # must include line endings
     except BrokenPipeError:
         sys.stdout = None
         sys.exit(141)
 
 
 def write_csv_to_stdout(data):
     fieldnames = data[0].keys()
```

### Comparing `xklb-2.6.9/xklb/utils/processes.py` & `xklb-2.7.5/xklb/utils/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools, json, multiprocessing, os, platform, shlex, signal, subprocess, sys
 from typing import NoReturn
 
-from xklb.utils import iterables
+from xklb.utils import consts, iterables
 from xklb.utils.log_utils import log
 
 
 def exit_nicely(_signal, _frame) -> NoReturn:
     log.warning("\nExiting... (Ctrl+C)")
     raise SystemExit(130)
 
@@ -69,14 +69,16 @@
         if ignore_regexps is not None:
             s = "\n".join(l for l in s.splitlines() if not any(r.match(l) for r in ignore_regexps))
 
         s = s.strip()
         if s:
             if quiet and is_success:
                 log.debug(s)
+            elif consts.PYTEST_RUNNING:
+                log.warning(s)
             else:
                 log.info(s)
         return s
 
     try:
         r = subprocess.run(
             command,
@@ -172,14 +174,16 @@
                 raise RuntimeError
             elif p.returncode == -6:  # Too many open files
                 raise OSError
             else:
                 raise UnplayableFile(out, err)
         d = json.loads(out.decode("utf-8"))
 
+        self.path = path
+
         self.streams = d.get("streams")
         self.chapters = d.get("chapters")
         self.format = d.get("format")
 
         self.video_streams = []
         self.audio_streams = []
         self.subtitle_streams = []
```

### Comparing `xklb-2.6.9/xklb/utils/sql_utils.py` & `xklb-2.7.5/xklb/utils/sql_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from xklb.utils import db_utils
+from xklb.utils import db_utils, nums
 from xklb.utils.log_utils import log
 
 
 def compare_block_strings(value, media_value):
     if value is None and media_value is None:
         return True
     elif value is None or media_value is None:
@@ -201,38 +201,65 @@
             {"AND COALESCE(time_deleted, 0)=0" if hide_deleted else ""}
         GROUP BY {freq_label}
     """
 
     return list(args.db.query(query))
 
 
-def historical_usage(args, freq="monthly", time_column="time_played", hide_deleted=False, where=None):
+def filter_time_played(args):
+    sql = []
+    played_before = args.played_before or args.created_before
+    played_within = args.played_within or args.created_within
+    if played_before:
+        played_before = nums.sql_human_time(played_before)
+        sql.append(f"and h.time_played < cast(STRFTIME('%s', datetime( 'now', '-{played_before}')) as int)")
+    if played_within:
+        played_within = nums.sql_human_time(played_within)
+        sql.append(f"and h.time_played >= cast(STRFTIME('%s', datetime( 'now', '-{played_within}')) as int)")
+
+    return " ".join(sql)
+
+
+def filter_play_count(args):
+    sql = []
+
+    if getattr(args, "completed", False):
+        sql.append("and coalesce(play_count, 0)>0")
+    if getattr(args, "in_progress", False):
+        sql.append("and coalesce(play_count, 0)=0")
+
+    return " ".join(sql)
+
+
+def historical_usage(args, freq="monthly", time_column="time_played", hide_deleted=False):
     freq_label, freq_sql = frequency_time_to_sql(freq, time_column)
     m_columns = args.db["media"].columns_dict
     h_columns = args.db["history"].columns_dict
 
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 {', FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead' if 'playhead' in h_columns else ''}
                 , *
             FROM media m
             JOIN history h on h.media_id = m.id
             WHERE 1=1
+            {filter_time_played(args)}
             {"AND COALESCE(time_deleted, 0)=0" if hide_deleted else ""}
             GROUP BY m.id, m.path
         )
         SELECT
             {freq_sql} AS {freq_label}
             {', SUM(duration) AS total_duration' if 'duration' in m_columns else ''}
             {', AVG(duration) AS avg_duration' if 'duration' in m_columns else ''}
             {', SUM(size) AS total_size' if 'size' in m_columns else ''}
             {', AVG(size) AS avg_size' if 'size' in m_columns else ''}
             , count(*) as count
         FROM m
-        WHERE {time_column}>0 {where or ''}
+        WHERE {time_column}>0
+            {filter_play_count(args)}
         GROUP BY {freq_label}
     """
 
     return list(args.db.query(query))
```

### Comparing `xklb-2.6.9/xklb/utils/strings.py` & `xklb-2.7.5/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/xklb/utils/web.py` & `xklb-2.7.5/xklb/utils/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,7 +672,30 @@
             parsed_url.params,
             new_query_string,
             parsed_url.fragment,
         )
     )
 
     return new_url
+
+
+def is_html(url, max_size=15 * 1024 * 1024):
+    r = requests_session().get(url, stream=True)
+
+    content_length = r.headers.get("Content-Length")
+    if content_length and int(content_length) > max_size:
+        return False
+
+    content_type = r.headers.get("Content-Type")
+    if content_type and not any(
+        s in content_type for s in ("text/html", "text/xhtml", "text/xml", "application/xml", "application/xhtml+xml")
+    ):
+        return False
+
+    try:
+        chunk = next(r.iter_content(max_size + 1))  # one more byte than max_size
+        if len(chunk) > max_size:
+            return False
+    except (requests.RequestException, StopIteration):
+        return False
+
+    return True  # if ambiguous, return True
```

### Comparing `xklb-2.6.9/xklb/assets/kotobago.png` & `xklb-2.7.5/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/.gitignore` & `xklb-2.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.6.9/pyproject.toml` & `xklb-2.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 authors = [
   {name = "Jacob Chapman", email = "7908073+chapmanjacobd@users.noreply.github.com"},
 ]
 dependencies = [
     "beautifulsoup4>=4.10.0",  # https://git.launchpad.net/beautifulsoup/commit/?id=34e0ce8a9dd43ada1c55b50a156fbce63b1e2ebb
+    "lxml",
     "catt",
     "feedparser",
     "ffmpeg-python",
     "ftfy",
     "gallery-dl",
     "humanize",
     "ipython",
```

### Comparing `xklb-2.6.9/.github/README.md` & `xklb-2.7.5/.github/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.009)
+    xk media library subcommands (v2.7.005)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -138,29 +138,37 @@
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
     ├────────────────┼─────────────────────────────────────────────┤
     │ nouns          │ Unstructured text -> compound nouns (stdin) │
     ╰────────────────┴─────────────────────────────────────────────╯
 
     Folder subcommands:
-    ╭───────────────┬──────────────────────────────────────────────────╮
-    │ merge-folders │ Merge two or more file trees                     │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ relmv         │ Move files preserving parent folder hierarchy    │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ mv-list       │ Find specific folders to move to different disks │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ scatter       │ Scatter files between folders or disks           │
-    ╰───────────────┴──────────────────────────────────────────────────╯
+    ╭─────────────────┬────────────────────────────────────────────────────────────╮
+    │ merge-folders   │ Merge two or more file trees                               │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ relmv           │ Move files preserving parent folder hierarchy              │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ mv-list         │ Find specific folders to move to different disks           │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ scatter         │ Scatter files between folders or disks                     │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ mount-stats     │ Show some relative mount stats                             │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ similar-folders │ Find similar folders based on folder name, size, and count │
+    ╰─────────────────┴────────────────────────────────────────────────────────────╯
 
     File subcommands:
     ╭────────────────┬─────────────────────────────────────────────────────╮
+    │ christen       │ Clean file paths                                    │
+    ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-hash    │ Calculate a hash based on small file segments       │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-compare │ Compare files using sample-hash and other shortcuts │
+    ├────────────────┼─────────────────────────────────────────────────────┤
+    │ similar-files  │ Find similar files based on filename                │
     ╰────────────────┴─────────────────────────────────────────────────────╯
 
     Tabular data subcommands:
     ╭──────────────────┬───────────────────────────────────────────────╮
     │ eda              │ Exploratory Data Analysis on table-like files │
     ├──────────────────┼───────────────────────────────────────────────┤
     │ mcda             │ Multi-criteria Ranking for Decision Support   │
@@ -181,44 +189,44 @@
     ╭──────────────────┬────────────────────────╮
     │ merge-dbs        │ Merge SQLITE databases │
     ├──────────────────┼────────────────────────┤
     │ copy-play-counts │ Copy play history      │
     ╰──────────────────┴────────────────────────╯
 
     Filesystem Database subcommands:
-    ╭─────────────┬────────────────────────────────╮
-    │ christen    │ Clean filenames                │
-    ├─────────────┼────────────────────────────────┤
-    │ disk-usage  │ Show disk usage                │
-    ├─────────────┼────────────────────────────────┤
-    │ mount-stats │ Show some relative mount stats │
-    ├─────────────┼────────────────────────────────┤
-    │ big-dirs    │ Show large folders             │
-    ├─────────────┼────────────────────────────────┤
-    │ search-db   │ Search a SQLITE database       │
-    ╰─────────────┴────────────────────────────────╯
+    ╭────────────┬──────────────────────────╮
+    │ disk-usage │ Show disk usage          │
+    ├────────────┼──────────────────────────┤
+    │ big-dirs   │ Show large folders       │
+    ├────────────┼──────────────────────────┤
+    │ search-db  │ Search a SQLITE database │
+    ╰────────────┴──────────────────────────╯
 
     Media Database subcommands:
-    ╭─────────────────┬────────────────────────────────╮
-    │ block           │ Block a channel                │
-    ├─────────────────┼────────────────────────────────┤
-    │ playlists       │ List stored playlists          │
-    ├─────────────────┼────────────────────────────────┤
-    │ download        │ Download media                 │
-    ├─────────────────┼────────────────────────────────┤
-    │ download-status │ Show download status           │
-    ├─────────────────┼────────────────────────────────┤
-    │ redownload      │ Re-download deleted/lost media │
-    ├─────────────────┼────────────────────────────────┤
-    │ history         │ Show some playback statistics  │
-    ├─────────────────┼────────────────────────────────┤
-    │ search          │ Search captions / subtitles    │
-    ├─────────────────┼────────────────────────────────┤
-    │ optimize        │ Re-optimize database           │
-    ╰─────────────────┴────────────────────────────────╯
+    ╭─────────────────┬─────────────────────────────────────────────────────────────╮
+    │ block           │ Block a channel                                             │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ playlists       │ List stored playlists                                       │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ download        │ Download media                                              │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ download-status │ Show download status                                        │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ redownload      │ Re-download deleted/lost media                              │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ history         │ Show and manage playback history                            │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ history-add     │ Add history from paths                                      │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ stats           │ Show some event statistics (created, deleted, watched, etc) │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ search          │ Search captions / subtitles                                 │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ optimize        │ Re-optimize database                                        │
+    ╰─────────────────┴─────────────────────────────────────────────────────────────╯
 
     Playback subcommands:
     ╭────────────┬───────────────────────────────────────────────────╮
     │ watch      │ Watch / Listen                                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ now        │ Show what is currently playing                    │
     ├────────────┼───────────────────────────────────────────────────┤
@@ -649,14 +657,31 @@
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
     Download checked videos
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
+    View most recent files
+
+        library fs example_dbs/web_add.image.db -u time_modified desc --cols path,width,height,size,time_modified -p -l 10
+        path                                                                                                                      width    height       size  time_modified
+        ----------------------------------------------------------------------------------------------------------------------  -------  --------  ---------  -----------------
+        https://siliconpr0n.org/map/infineon/m7690-b1/single/infineon_m7690-b1_infosecdj_mz_nikon20x.jpg                           7066     10513   16.4 MiB  2 days ago, 20:54
+        https://siliconpr0n.org/map/starchip/scf384g/single/starchip_scf384g_infosecdj_mz_nikon20x.jpg                            10804     10730   19.2 MiB  2 days ago, 15:31
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms50x-1.25.jpg            28966     26816  192.2 MiB  4 days ago, 15:05
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms20x-1.25.jpg            11840     10978   49.2 MiB  4 days ago, 15:04
+        https://siliconpr0n.org/map/hp/2hpt20065-1/single/hp_2hpt20065-1_marmontel_mz_ms10x-1.25.jpg                              16457     14255  101.4 MiB  4 days ago, 15:03
+        https://siliconpr0n.org/map/pervasive/e2213ps01e1/single/pervasive_e2213ps01e1_azonenberg_back_roi1_mit10x_rotated.jpg    18880     61836  136.8 MiB  6 days ago, 16:00
+        https://siliconpr0n.org/map/pervasive/e2213ps01e/single/pervasive_e2213ps01e_azonenberg_back_mit5x_rotated.jpg            62208     30736  216.5 MiB  6 days ago, 15:57
+        https://siliconpr0n.org/map/amd/am2964bpc/single/amd_am2964bpc_infosecdj_mz_lmplan10x.jpg                                 12809     11727   39.8 MiB  6 days ago, 10:28
+        https://siliconpr0n.org/map/unknown/ks1804ir1/single/unknown_ks1804ir1_infosecdj_mz_lmplan10x.jpg                          6508      6707    8.4 MiB  6 days ago, 08:04
+        https://siliconpr0n.org/map/amd/am2960dc-b/single/amd_am2960dc-b_infosecdj_mz_lmplan10x.jpg                               16434     15035   64.9 MiB  7 days ago, 19:01
+        10 media (limited by --limit 10)
+
 
 
 </details>
 
 ###### gallery-add
 
 <details><summary>Add online gallery media (gallery-dl)</summary>
@@ -811,14 +836,19 @@
     $ library site-add -h
     usage: library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
+    Requires selenium-wire
+    Requires xmltodict when using --extract-xml
+
+        pip install selenium-wire xmltodict
+
     Run with `-vv` to see and interact with the browser
 
 
 </details>
 
 ###### reddit-add
 
@@ -1163,24 +1193,24 @@
 ###### scatter
 
 <details><summary>Scatter files between folders or disks</summary>
 
     $ library scatter -h
     usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
-    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
-
     Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
 
         library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
 
     Reduce number of files per folder (creates more folders)
 
         library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
+    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
     Multi-device re-bin: balance by size
 
         library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
@@ -1232,19 +1262,99 @@
 
         library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
 
     Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
 
         library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
 
+    This tool is intended for local use. If transferring many small files across the network something like
+    [fpart](https://github.com/martymac/fpart) or [fpsync](https://www.fpart.org/fpsync/) will be better.
+
+
+</details>
+
+###### mount-stats
+
+<details><summary>Show some relative mount stats</summary>
+
+    $ library mount-stats -h
+    usage: library mount-stats MOUNTPOINT ...
+
+    Print relative use and free for multiple mount points
+
+
+</details>
+
+###### similar-folders
+
+<details><summary>Find similar folders based on folder name, size, and count</summary>
+
+    $ library similar-folders -h
+    usage: library similar-folders PATH ...
+
+    Find similar folders based on foldernames, similar size, and similar number of files
+
+        $ library similar-folders ~/d/
+
+        group /home/xk/d/dump/datasets/*vector          total_size    median_size      files
+        ----------------------------------------------  ------------  -------------  -------
+        /home/xk/d/dump/datasets/vector/output/         1.8 GiB       89.5 KiB          1980
+        /home/xk/d/dump/datasets/vector/output2/        1.8 GiB       89.5 KiB          1979
+
+    Find similar folders based on ONLY foldernames, using the full path
+
+        $ library similar-folders --no-filter-sizes --no-filter-counts --full-path ~/d/
+
+    Find similar folders based on ONLY number of files
+
+        $ library similar-folders --no-filter-names --no-filter-sizes ~/d/
+
+    Find similar folders based on ONLY median size
+
+        $ library similar-folders --no-filter-names --no-filter-counts ~/d/
+
+    Find similar folders based on ONLY total size
+
+        $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
+
+    Print only paths
+
+        $ library similar-folders ~/d/ -pf
+        /home/xk/d/dump/datasets/vector/output/
+        /home/xk/d/dump/datasets/vector/output2/
+
 
 </details>
 
 ### File subcommands
 
+###### christen
+
+<details><summary>Clean file paths</summary>
+
+    $ library christen -h
+    usage: library christen [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is simulate
+
+        library christen ~/messy/
+
+    To actually do stuff use the run flag
+
+        library christen . --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space
+
+
+</details>
+
 ###### sample-hash
 
 <details><summary>Calculate a hash based on small file segments</summary>
 
     $ library sample-hash -h
     usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
@@ -1265,14 +1375,36 @@
     usage: library sample-compare [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
+###### similar-files
+
+<details><summary>Find similar files based on filename</summary>
+
+    $ library similar-files -h
+    usage: library similar-files PATH ...
+
+    Find similar files using filenames and size
+
+        $ library similar-files ~/d/
+
+    Find similar files based on ONLY foldernames, using the full path
+
+        $ library similar-files --no-filter-sizes --full-path ~/d/
+
+    Find similar files based on ONLY size
+
+        $ library similar-files --no-filter-names ~/d/
+
+
+</details>
+
 ### Tabular data subcommands
 
 ###### eda
 
 <details><summary>Exploratory Data Analysis on table-like files</summary>
 
     $ library eda -h
@@ -1554,38 +1686,14 @@
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
 
 </details>
 
 ### Filesystem Database subcommands
 
-###### christen
-
-<details><summary>Clean filenames</summary>
-
-    $ library christen -h
-    usage: library christen DATABASE [--run]
-
-    Rename files to be somewhat normalized
-
-    Default mode is simulate
-
-        library christen fs.db
-
-    To actually do stuff use the run flag
-
-        library christen audio.db --run
-
-    You can optionally replace all the spaces in your filenames with dots
-
-        library christen --dot-space video.db
-
-
-</details>
-
 ###### disk-usage
 
 <details><summary>Show disk usage</summary>
 
     $ library disk-usage -h
     usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
 
@@ -1616,26 +1724,14 @@
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
 
 
 
 </details>
 
-###### mount-stats
-
-<details><summary>Show some relative mount stats</summary>
-
-    $ library mount-stats -h
-    usage: library mount-stats MOUNTPOINT ...
-
-    Print relative use and free for multiple mount points
-
-
-</details>
-
 ###### big-dirs
 
 <details><summary>Show large folders</summary>
 
     $ library big-dirs -h
     usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
 
@@ -1771,15 +1867,15 @@
 ###### download
 
 <details><summary>Download media</summary>
 
     $ library download -h
     usage: library download [--prefix /mnt/d/] [--safe] [--subs] [--auto-subs] [--small] DATABASE --video | --audio | --photos
 
-    Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
+    Files will be saved to <lb download prefix>/<extractor>/. The default prefix is the current working directory.
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
     But you can sort; eg. oldest first
 
@@ -1816,14 +1912,16 @@
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │            │ and 20 minutes   │                    │          │
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘════════════╧══════════════════╧════════════════════╧══════════╛
 
+    Broadcatching absolution
+
 
 </details>
 
 ###### download-status
 
 <details><summary>Show download status</summary>
 
@@ -1909,22 +2007,77 @@
         library redownload city.db 2023-01-26T19:54:42 2023-01-26T20:45:24
 
 
 </details>
 
 ###### history
 
-<details><summary>Show some playback statistics</summary>
+<details><summary>Show and manage playback history</summary>
 
     $ library history -h
     usage: library history [--frequency daily weekly (monthly) yearly] [--limit LIMIT] DATABASE [(all) watching watched created modified deleted]
 
-    Explore history through different facets
+    View playback history
+
+        $ library history web_add.image.db
+        In progress:
+        play_count  time_last_played    playhead    path                                     title
+        ------------  ------------------  ----------  ---------------------------------------  -----------
+                0  today, 20:48        2 seconds   https://siliconpr0n.org/map/COPYING.txt  COPYING.txt
+
+    Show only completed history
+
+        $ library history web_add.image.db --completed
+
+    Show only completed history
+
+        $ library history web_add.image.db --in-progress
+
+    Delete history
+
+        Delete two hours of history
+        $ library history web_add.image.db --played-within '2 hours' -L inf --delete-rows
+
+        Delete all history
+        $ library history web_add.image.db -L inf --delete-rows
+
+    See also: library stats -h
+              library history-add -h
+
+
+</details>
 
-        library history video.db watched
+###### history-add
+
+<details><summary>Add history from paths</summary>
+
+    $ library history-add -h
+    usage: library history-add DATABASE PATH ...
+
+    Add history
+
+        $ library history-add links.db $urls $paths
+        $ library history-add links.db (cb)
+
+    Items that don't already exist in the database will be counted under "skipped"
+
+
+
+</details>
+
+###### stats
+
+<details><summary>Show some event statistics (created, deleted, watched, etc)</summary>
+
+    $ library stats -h
+    usage: library stats DATABASE TIME_COLUMN
+
+    View watched stats
+
+        $ library stats video.db --completed
         Finished watching:
         ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
         │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
         ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
         │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
@@ -1934,79 +2087,17 @@
         │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
         ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
 
-    library history video.db created --frequency yearly
-        Created media:
-        ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
-        │   time_period │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
-        ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
-        │          2005 │ 9.78 minutes                               │ 1.95 minutes   │ 16.9 MB    │ 3.4 MB     │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2006 │ 7 hours and 10.67 minutes                  │ 5 minutes      │ 891.1 MB   │ 10.4 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2007 │ 1 day, 17 hours and 33 minutes             │ 8.55 minutes   │ 5.9 GB     │ 20.3 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2008 │ 5 days, 16 hours and 10 minutes            │ 17.02 minutes  │ 20.7 GB    │ 43.1 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2009 │ 24 days, 2 hours and 56 minutes            │ 33.68 minutes  │ 108.4 GB   │ 105.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2010 │ 1 month, 1 days and 1 minutes              │ 35.52 minutes  │ 124.2 GB   │ 95.7 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2011 │ 2 months, 14 days, 1 hour and 22 minutes   │ 55.93 minutes  │ 222.0 GB   │ 114.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2012 │ 2 months, 22 days, 19 hours and 17 minutes │ 45.50 minutes  │ 343.6 GB   │ 129.6 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2013 │ 3 months, 11 days, 21 hours and 48 minutes │ 42.72 minutes  │ 461.1 GB   │ 131.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2014 │ 3 months, 7 days, 10 hours and 22 minutes  │ 46.80 minutes  │ 529.6 GB   │ 173.1 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2015 │ 2 months, 21 days, 23 hours and 36 minutes │ 36.73 minutes  │ 452.7 GB   │ 139.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2016 │ 3 months, 26 days, 7 hours and 59 minutes  │ 39.48 minutes  │ 603.4 GB   │ 139.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2017 │ 3 months, 10 days, 2 hours and 19 minutes  │ 31.78 minutes  │ 543.5 GB   │ 117.5 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2018 │ 3 months, 21 days, 20 hours and 56 minutes │ 30.98 minutes  │ 607.5 GB   │ 114.8 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2019 │ 5 months, 23 days, 2 hours and 30 minutes  │ 35.77 minutes  │ 919.7 GB   │ 129.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2020 │ 7 months, 16 days, 10 hours and 58 minutes │ 26.15 minutes  │ 1.2 TB     │ 93.9 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2021 │ 7 months, 21 days, 9 hours and 40 minutes  │ 39.93 minutes  │ 1.3 TB     │ 149.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2022 │ 17 years, 3 months, 0 days and 21 hours    │ 19.62 minutes  │ 35.8 TB    │ 77.5 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2023 │ 15 years, 3 months, 24 days and 1 hours    │ 17.57 minutes  │ 27.6 TB    │ 60.2 MB    │
-        ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
-        ╒════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤════════════════╕
-        │ title_path                                                                                 │ duration      │ time_created   │
-        ╞════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪════════════════╡
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 07/20 | Adam Cheng | 2009 #Chinesedrama │ 43.85 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zntYD1yLrG8                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 08/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zQnSfoWrh-4                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 06/20 | Adam Cheng | 2009 #Chinesedrama │ 43.60 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=Qiax1kFyGWU                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 04/20 | Adam Cheng | 2009 #Chinesedrama │ 43.45 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=NT9C3PRrlTA                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 02/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=MjpCiTawlTE                                                │               │                │
-        ╘════════════════════════════════════════════════════════════════════════════════════════════╧═══════════════╧════════════════╛
-
     View download stats
 
-        library history video.db --freqency daily downloaded
+        $ library stats video.db time_downloaded --frequency daily
         Downloaded media:
         day         total_duration                          avg_duration                total_size    avg_size    count
         ----------  --------------------------------------  ------------------------  ------------  ----------  -------
         2023-08-11  1 month, 7 days and 8 hours             17 minutes                    192.2 GB     58.3 MB     3296
         2023-08-12  18 days and 15 hours                    17 minutes                     89.7 GB     56.4 MB     1590
         2023-08-14  13 days and 1 hours                     22 minutes                    111.2 GB    127.2 MB      874
         2023-08-15  13 days and 6 hours                     17 minutes                    140.0 GB    126.7 MB     1105
@@ -2014,19 +2105,19 @@
         2023-08-18  2 months, 30 days and 18 hours          17 minutes                    501.9 GB     63.3 MB     7926
         2023-08-19  2 months, 6 days and 19 hours           19 minutes                    578.1 GB    110.6 MB     5229
         2023-08-20  3 days and 9 hours                      6 minutes and 57 seconds       14.5 GB     20.7 MB      700
         2023-08-21  4 days and 3 hours                      12 minutes                     18.0 GB     36.3 MB      495
         2023-08-22  10 days and 8 hours                     17 minutes                     82.1 GB     91.7 MB      895
         2023-08-23  19 days and 9 hours                     22 minutes                     93.7 GB     74.7 MB     1254
 
-        See also: library history video.db --freqency daily downloaded --hide-deleted
+        See also: library stats video.db time_downloaded -f daily --hide-deleted
 
     View deleted stats
 
-        library history video.db deleted
+        $ library stats video.db time_deleted
         Deleted media:
         ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
         │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
         ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
         │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
         ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
@@ -2038,14 +2129,36 @@
         │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
         ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
         │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
         │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
         ...
 
 
+    View time_modified stats
+
+        $ library stats example_dbs/web_add.image.db time_modified -f year
+        Time_Modified media:
+        year      total_size    avg_size    count
+        ------  ------------  ----------  -------
+        2010         4.4 MiB     1.5 MiB        3
+        2011       136.2 MiB    68.1 MiB        2
+        2013         1.6 GiB    10.7 MiB      154
+        2014         4.6 GiB    25.2 MiB      187
+        2015         4.3 GiB    26.5 MiB      167
+        2016         5.1 GiB    46.8 MiB      112
+        2017         4.8 GiB    51.7 MiB       95
+        2018         5.3 GiB    97.9 MiB       55
+        2019         1.3 GiB    46.5 MiB       29
+        2020        25.7 GiB   113.5 MiB      232
+        2021        25.6 GiB    96.5 MiB      272
+        2022        14.6 GiB    82.7 MiB      181
+        2023        24.3 GiB    72.5 MiB      343
+        2024        17.3 GiB   104.8 MiB      169
+        14 media
+
 
 </details>
 
 ###### search
 
 <details><summary>Search captions / subtitles</summary>
```

### Comparing `xklb-2.6.9/PKG-INFO` & `xklb-2.7.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.6.9
+Version: 2.7.5
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -43,14 +43,15 @@
 Requires-Dist: catt
 Requires-Dist: feedparser
 Requires-Dist: ffmpeg-python
 Requires-Dist: ftfy
 Requires-Dist: gallery-dl
 Requires-Dist: humanize
 Requires-Dist: ipython
+Requires-Dist: lxml
 Requires-Dist: markdown
 Requires-Dist: mutagen
 Requires-Dist: natsort
 Requires-Dist: praw
 Requires-Dist: puremagic
 Requires-Dist: pysubs2
 Requires-Dist: python-dateutil
@@ -181,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.009)
+    xk media library subcommands (v2.7.005)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -226,29 +227,37 @@
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
     ├────────────────┼─────────────────────────────────────────────┤
     │ nouns          │ Unstructured text -> compound nouns (stdin) │
     ╰────────────────┴─────────────────────────────────────────────╯
 
     Folder subcommands:
-    ╭───────────────┬──────────────────────────────────────────────────╮
-    │ merge-folders │ Merge two or more file trees                     │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ relmv         │ Move files preserving parent folder hierarchy    │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ mv-list       │ Find specific folders to move to different disks │
-    ├───────────────┼──────────────────────────────────────────────────┤
-    │ scatter       │ Scatter files between folders or disks           │
-    ╰───────────────┴──────────────────────────────────────────────────╯
+    ╭─────────────────┬────────────────────────────────────────────────────────────╮
+    │ merge-folders   │ Merge two or more file trees                               │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ relmv           │ Move files preserving parent folder hierarchy              │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ mv-list         │ Find specific folders to move to different disks           │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ scatter         │ Scatter files between folders or disks                     │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ mount-stats     │ Show some relative mount stats                             │
+    ├─────────────────┼────────────────────────────────────────────────────────────┤
+    │ similar-folders │ Find similar folders based on folder name, size, and count │
+    ╰─────────────────┴────────────────────────────────────────────────────────────╯
 
     File subcommands:
     ╭────────────────┬─────────────────────────────────────────────────────╮
+    │ christen       │ Clean file paths                                    │
+    ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-hash    │ Calculate a hash based on small file segments       │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-compare │ Compare files using sample-hash and other shortcuts │
+    ├────────────────┼─────────────────────────────────────────────────────┤
+    │ similar-files  │ Find similar files based on filename                │
     ╰────────────────┴─────────────────────────────────────────────────────╯
 
     Tabular data subcommands:
     ╭──────────────────┬───────────────────────────────────────────────╮
     │ eda              │ Exploratory Data Analysis on table-like files │
     ├──────────────────┼───────────────────────────────────────────────┤
     │ mcda             │ Multi-criteria Ranking for Decision Support   │
@@ -269,44 +278,44 @@
     ╭──────────────────┬────────────────────────╮
     │ merge-dbs        │ Merge SQLITE databases │
     ├──────────────────┼────────────────────────┤
     │ copy-play-counts │ Copy play history      │
     ╰──────────────────┴────────────────────────╯
 
     Filesystem Database subcommands:
-    ╭─────────────┬────────────────────────────────╮
-    │ christen    │ Clean filenames                │
-    ├─────────────┼────────────────────────────────┤
-    │ disk-usage  │ Show disk usage                │
-    ├─────────────┼────────────────────────────────┤
-    │ mount-stats │ Show some relative mount stats │
-    ├─────────────┼────────────────────────────────┤
-    │ big-dirs    │ Show large folders             │
-    ├─────────────┼────────────────────────────────┤
-    │ search-db   │ Search a SQLITE database       │
-    ╰─────────────┴────────────────────────────────╯
+    ╭────────────┬──────────────────────────╮
+    │ disk-usage │ Show disk usage          │
+    ├────────────┼──────────────────────────┤
+    │ big-dirs   │ Show large folders       │
+    ├────────────┼──────────────────────────┤
+    │ search-db  │ Search a SQLITE database │
+    ╰────────────┴──────────────────────────╯
 
     Media Database subcommands:
-    ╭─────────────────┬────────────────────────────────╮
-    │ block           │ Block a channel                │
-    ├─────────────────┼────────────────────────────────┤
-    │ playlists       │ List stored playlists          │
-    ├─────────────────┼────────────────────────────────┤
-    │ download        │ Download media                 │
-    ├─────────────────┼────────────────────────────────┤
-    │ download-status │ Show download status           │
-    ├─────────────────┼────────────────────────────────┤
-    │ redownload      │ Re-download deleted/lost media │
-    ├─────────────────┼────────────────────────────────┤
-    │ history         │ Show some playback statistics  │
-    ├─────────────────┼────────────────────────────────┤
-    │ search          │ Search captions / subtitles    │
-    ├─────────────────┼────────────────────────────────┤
-    │ optimize        │ Re-optimize database           │
-    ╰─────────────────┴────────────────────────────────╯
+    ╭─────────────────┬─────────────────────────────────────────────────────────────╮
+    │ block           │ Block a channel                                             │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ playlists       │ List stored playlists                                       │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ download        │ Download media                                              │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ download-status │ Show download status                                        │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ redownload      │ Re-download deleted/lost media                              │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ history         │ Show and manage playback history                            │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ history-add     │ Add history from paths                                      │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ stats           │ Show some event statistics (created, deleted, watched, etc) │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ search          │ Search captions / subtitles                                 │
+    ├─────────────────┼─────────────────────────────────────────────────────────────┤
+    │ optimize        │ Re-optimize database                                        │
+    ╰─────────────────┴─────────────────────────────────────────────────────────────╯
 
     Playback subcommands:
     ╭────────────┬───────────────────────────────────────────────────╮
     │ watch      │ Watch / Listen                                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ now        │ Show what is currently playing                    │
     ├────────────┼───────────────────────────────────────────────────┤
@@ -737,14 +746,31 @@
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
     Download checked videos
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
+    View most recent files
+
+        library fs example_dbs/web_add.image.db -u time_modified desc --cols path,width,height,size,time_modified -p -l 10
+        path                                                                                                                      width    height       size  time_modified
+        ----------------------------------------------------------------------------------------------------------------------  -------  --------  ---------  -----------------
+        https://siliconpr0n.org/map/infineon/m7690-b1/single/infineon_m7690-b1_infosecdj_mz_nikon20x.jpg                           7066     10513   16.4 MiB  2 days ago, 20:54
+        https://siliconpr0n.org/map/starchip/scf384g/single/starchip_scf384g_infosecdj_mz_nikon20x.jpg                            10804     10730   19.2 MiB  2 days ago, 15:31
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms50x-1.25.jpg            28966     26816  192.2 MiB  4 days ago, 15:05
+        https://siliconpr0n.org/map/hp/2hpt20065-1-68k-core/single/hp_2hpt20065-1-68k-core_marmontel_mz_ms20x-1.25.jpg            11840     10978   49.2 MiB  4 days ago, 15:04
+        https://siliconpr0n.org/map/hp/2hpt20065-1/single/hp_2hpt20065-1_marmontel_mz_ms10x-1.25.jpg                              16457     14255  101.4 MiB  4 days ago, 15:03
+        https://siliconpr0n.org/map/pervasive/e2213ps01e1/single/pervasive_e2213ps01e1_azonenberg_back_roi1_mit10x_rotated.jpg    18880     61836  136.8 MiB  6 days ago, 16:00
+        https://siliconpr0n.org/map/pervasive/e2213ps01e/single/pervasive_e2213ps01e_azonenberg_back_mit5x_rotated.jpg            62208     30736  216.5 MiB  6 days ago, 15:57
+        https://siliconpr0n.org/map/amd/am2964bpc/single/amd_am2964bpc_infosecdj_mz_lmplan10x.jpg                                 12809     11727   39.8 MiB  6 days ago, 10:28
+        https://siliconpr0n.org/map/unknown/ks1804ir1/single/unknown_ks1804ir1_infosecdj_mz_lmplan10x.jpg                          6508      6707    8.4 MiB  6 days ago, 08:04
+        https://siliconpr0n.org/map/amd/am2960dc-b/single/amd_am2960dc-b_infosecdj_mz_lmplan10x.jpg                               16434     15035   64.9 MiB  7 days ago, 19:01
+        10 media (limited by --limit 10)
+
 
 
 </details>
 
 ###### gallery-add
 
 <details><summary>Add online gallery media (gallery-dl)</summary>
@@ -899,14 +925,19 @@
     $ library site-add -h
     usage: library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
+    Requires selenium-wire
+    Requires xmltodict when using --extract-xml
+
+        pip install selenium-wire xmltodict
+
     Run with `-vv` to see and interact with the browser
 
 
 </details>
 
 ###### reddit-add
 
@@ -1251,24 +1282,24 @@
 ###### scatter
 
 <details><summary>Scatter files between folders or disks</summary>
 
     $ library scatter -h
     usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
-    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
-
     Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
 
         library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
 
     Reduce number of files per folder (creates more folders)
 
         library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
+    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
     Multi-device re-bin: balance by size
 
         library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
@@ -1320,19 +1351,99 @@
 
         library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
 
     Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
 
         library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
 
+    This tool is intended for local use. If transferring many small files across the network something like
+    [fpart](https://github.com/martymac/fpart) or [fpsync](https://www.fpart.org/fpsync/) will be better.
+
+
+</details>
+
+###### mount-stats
+
+<details><summary>Show some relative mount stats</summary>
+
+    $ library mount-stats -h
+    usage: library mount-stats MOUNTPOINT ...
+
+    Print relative use and free for multiple mount points
+
+
+</details>
+
+###### similar-folders
+
+<details><summary>Find similar folders based on folder name, size, and count</summary>
+
+    $ library similar-folders -h
+    usage: library similar-folders PATH ...
+
+    Find similar folders based on foldernames, similar size, and similar number of files
+
+        $ library similar-folders ~/d/
+
+        group /home/xk/d/dump/datasets/*vector          total_size    median_size      files
+        ----------------------------------------------  ------------  -------------  -------
+        /home/xk/d/dump/datasets/vector/output/         1.8 GiB       89.5 KiB          1980
+        /home/xk/d/dump/datasets/vector/output2/        1.8 GiB       89.5 KiB          1979
+
+    Find similar folders based on ONLY foldernames, using the full path
+
+        $ library similar-folders --no-filter-sizes --no-filter-counts --full-path ~/d/
+
+    Find similar folders based on ONLY number of files
+
+        $ library similar-folders --no-filter-names --no-filter-sizes ~/d/
+
+    Find similar folders based on ONLY median size
+
+        $ library similar-folders --no-filter-names --no-filter-counts ~/d/
+
+    Find similar folders based on ONLY total size
+
+        $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
+
+    Print only paths
+
+        $ library similar-folders ~/d/ -pf
+        /home/xk/d/dump/datasets/vector/output/
+        /home/xk/d/dump/datasets/vector/output2/
+
 
 </details>
 
 ### File subcommands
 
+###### christen
+
+<details><summary>Clean file paths</summary>
+
+    $ library christen -h
+    usage: library christen [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is simulate
+
+        library christen ~/messy/
+
+    To actually do stuff use the run flag
+
+        library christen . --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space
+
+
+</details>
+
 ###### sample-hash
 
 <details><summary>Calculate a hash based on small file segments</summary>
 
     $ library sample-hash -h
     usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
@@ -1353,14 +1464,36 @@
     usage: library sample-compare [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
+###### similar-files
+
+<details><summary>Find similar files based on filename</summary>
+
+    $ library similar-files -h
+    usage: library similar-files PATH ...
+
+    Find similar files using filenames and size
+
+        $ library similar-files ~/d/
+
+    Find similar files based on ONLY foldernames, using the full path
+
+        $ library similar-files --no-filter-sizes --full-path ~/d/
+
+    Find similar files based on ONLY size
+
+        $ library similar-files --no-filter-names ~/d/
+
+
+</details>
+
 ### Tabular data subcommands
 
 ###### eda
 
 <details><summary>Exploratory Data Analysis on table-like files</summary>
 
     $ library eda -h
@@ -1642,38 +1775,14 @@
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
 
 </details>
 
 ### Filesystem Database subcommands
 
-###### christen
-
-<details><summary>Clean filenames</summary>
-
-    $ library christen -h
-    usage: library christen DATABASE [--run]
-
-    Rename files to be somewhat normalized
-
-    Default mode is simulate
-
-        library christen fs.db
-
-    To actually do stuff use the run flag
-
-        library christen audio.db --run
-
-    You can optionally replace all the spaces in your filenames with dots
-
-        library christen --dot-space video.db
-
-
-</details>
-
 ###### disk-usage
 
 <details><summary>Show disk usage</summary>
 
     $ library disk-usage -h
     usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
 
@@ -1704,26 +1813,14 @@
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
 
 
 
 </details>
 
-###### mount-stats
-
-<details><summary>Show some relative mount stats</summary>
-
-    $ library mount-stats -h
-    usage: library mount-stats MOUNTPOINT ...
-
-    Print relative use and free for multiple mount points
-
-
-</details>
-
 ###### big-dirs
 
 <details><summary>Show large folders</summary>
 
     $ library big-dirs -h
     usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
 
@@ -1859,15 +1956,15 @@
 ###### download
 
 <details><summary>Download media</summary>
 
     $ library download -h
     usage: library download [--prefix /mnt/d/] [--safe] [--subs] [--auto-subs] [--small] DATABASE --video | --audio | --photos
 
-    Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
+    Files will be saved to <lb download prefix>/<extractor>/. The default prefix is the current working directory.
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
     But you can sort; eg. oldest first
 
@@ -1904,14 +2001,16 @@
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │            │ and 20 minutes   │                    │          │
         ├────────────┼──────────────────┼────────────────────┼──────────┤
         │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘════════════╧══════════════════╧════════════════════╧══════════╛
 
+    Broadcatching absolution
+
 
 </details>
 
 ###### download-status
 
 <details><summary>Show download status</summary>
 
@@ -1997,22 +2096,77 @@
         library redownload city.db 2023-01-26T19:54:42 2023-01-26T20:45:24
 
 
 </details>
 
 ###### history
 
-<details><summary>Show some playback statistics</summary>
+<details><summary>Show and manage playback history</summary>
 
     $ library history -h
     usage: library history [--frequency daily weekly (monthly) yearly] [--limit LIMIT] DATABASE [(all) watching watched created modified deleted]
 
-    Explore history through different facets
+    View playback history
+
+        $ library history web_add.image.db
+        In progress:
+        play_count  time_last_played    playhead    path                                     title
+        ------------  ------------------  ----------  ---------------------------------------  -----------
+                0  today, 20:48        2 seconds   https://siliconpr0n.org/map/COPYING.txt  COPYING.txt
+
+    Show only completed history
+
+        $ library history web_add.image.db --completed
+
+    Show only completed history
+
+        $ library history web_add.image.db --in-progress
+
+    Delete history
+
+        Delete two hours of history
+        $ library history web_add.image.db --played-within '2 hours' -L inf --delete-rows
+
+        Delete all history
+        $ library history web_add.image.db -L inf --delete-rows
+
+    See also: library stats -h
+              library history-add -h
+
+
+</details>
 
-        library history video.db watched
+###### history-add
+
+<details><summary>Add history from paths</summary>
+
+    $ library history-add -h
+    usage: library history-add DATABASE PATH ...
+
+    Add history
+
+        $ library history-add links.db $urls $paths
+        $ library history-add links.db (cb)
+
+    Items that don't already exist in the database will be counted under "skipped"
+
+
+
+</details>
+
+###### stats
+
+<details><summary>Show some event statistics (created, deleted, watched, etc)</summary>
+
+    $ library stats -h
+    usage: library stats DATABASE TIME_COLUMN
+
+    View watched stats
+
+        $ library stats video.db --completed
         Finished watching:
         ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
         │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
         ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
         │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
@@ -2022,79 +2176,17 @@
         │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
         ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
         ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
 
-    library history video.db created --frequency yearly
-        Created media:
-        ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
-        │   time_period │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
-        ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
-        │          2005 │ 9.78 minutes                               │ 1.95 minutes   │ 16.9 MB    │ 3.4 MB     │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2006 │ 7 hours and 10.67 minutes                  │ 5 minutes      │ 891.1 MB   │ 10.4 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2007 │ 1 day, 17 hours and 33 minutes             │ 8.55 minutes   │ 5.9 GB     │ 20.3 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2008 │ 5 days, 16 hours and 10 minutes            │ 17.02 minutes  │ 20.7 GB    │ 43.1 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2009 │ 24 days, 2 hours and 56 minutes            │ 33.68 minutes  │ 108.4 GB   │ 105.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2010 │ 1 month, 1 days and 1 minutes              │ 35.52 minutes  │ 124.2 GB   │ 95.7 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2011 │ 2 months, 14 days, 1 hour and 22 minutes   │ 55.93 minutes  │ 222.0 GB   │ 114.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2012 │ 2 months, 22 days, 19 hours and 17 minutes │ 45.50 minutes  │ 343.6 GB   │ 129.6 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2013 │ 3 months, 11 days, 21 hours and 48 minutes │ 42.72 minutes  │ 461.1 GB   │ 131.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2014 │ 3 months, 7 days, 10 hours and 22 minutes  │ 46.80 minutes  │ 529.6 GB   │ 173.1 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2015 │ 2 months, 21 days, 23 hours and 36 minutes │ 36.73 minutes  │ 452.7 GB   │ 139.2 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2016 │ 3 months, 26 days, 7 hours and 59 minutes  │ 39.48 minutes  │ 603.4 GB   │ 139.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2017 │ 3 months, 10 days, 2 hours and 19 minutes  │ 31.78 minutes  │ 543.5 GB   │ 117.5 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2018 │ 3 months, 21 days, 20 hours and 56 minutes │ 30.98 minutes  │ 607.5 GB   │ 114.8 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2019 │ 5 months, 23 days, 2 hours and 30 minutes  │ 35.77 minutes  │ 919.7 GB   │ 129.7 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2020 │ 7 months, 16 days, 10 hours and 58 minutes │ 26.15 minutes  │ 1.2 TB     │ 93.9 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2021 │ 7 months, 21 days, 9 hours and 40 minutes  │ 39.93 minutes  │ 1.3 TB     │ 149.9 MB   │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2022 │ 17 years, 3 months, 0 days and 21 hours    │ 19.62 minutes  │ 35.8 TB    │ 77.5 MB    │
-        ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
-        │          2023 │ 15 years, 3 months, 24 days and 1 hours    │ 17.57 minutes  │ 27.6 TB    │ 60.2 MB    │
-        ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
-        ╒════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤════════════════╕
-        │ title_path                                                                                 │ duration      │ time_created   │
-        ╞════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪════════════════╡
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 07/20 | Adam Cheng | 2009 #Chinesedrama │ 43.85 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zntYD1yLrG8                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 08/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=zQnSfoWrh-4                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 06/20 | Adam Cheng | 2009 #Chinesedrama │ 43.60 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=Qiax1kFyGWU                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 04/20 | Adam Cheng | 2009 #Chinesedrama │ 43.45 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=NT9C3PRrlTA                                                │               │                │
-        ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
-        │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 02/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
-        │ https://www.youtube.com/watch?v=MjpCiTawlTE                                                │               │                │
-        ╘════════════════════════════════════════════════════════════════════════════════════════════╧═══════════════╧════════════════╛
-
     View download stats
 
-        library history video.db --freqency daily downloaded
+        $ library stats video.db time_downloaded --frequency daily
         Downloaded media:
         day         total_duration                          avg_duration                total_size    avg_size    count
         ----------  --------------------------------------  ------------------------  ------------  ----------  -------
         2023-08-11  1 month, 7 days and 8 hours             17 minutes                    192.2 GB     58.3 MB     3296
         2023-08-12  18 days and 15 hours                    17 minutes                     89.7 GB     56.4 MB     1590
         2023-08-14  13 days and 1 hours                     22 minutes                    111.2 GB    127.2 MB      874
         2023-08-15  13 days and 6 hours                     17 minutes                    140.0 GB    126.7 MB     1105
@@ -2102,19 +2194,19 @@
         2023-08-18  2 months, 30 days and 18 hours          17 minutes                    501.9 GB     63.3 MB     7926
         2023-08-19  2 months, 6 days and 19 hours           19 minutes                    578.1 GB    110.6 MB     5229
         2023-08-20  3 days and 9 hours                      6 minutes and 57 seconds       14.5 GB     20.7 MB      700
         2023-08-21  4 days and 3 hours                      12 minutes                     18.0 GB     36.3 MB      495
         2023-08-22  10 days and 8 hours                     17 minutes                     82.1 GB     91.7 MB      895
         2023-08-23  19 days and 9 hours                     22 minutes                     93.7 GB     74.7 MB     1254
 
-        See also: library history video.db --freqency daily downloaded --hide-deleted
+        See also: library stats video.db time_downloaded -f daily --hide-deleted
 
     View deleted stats
 
-        library history video.db deleted
+        $ library stats video.db time_deleted
         Deleted media:
         ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
         │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
         ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
         │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
         ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
         │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
@@ -2126,14 +2218,36 @@
         │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
         ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
         │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
         │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
         ...
 
 
+    View time_modified stats
+
+        $ library stats example_dbs/web_add.image.db time_modified -f year
+        Time_Modified media:
+        year      total_size    avg_size    count
+        ------  ------------  ----------  -------
+        2010         4.4 MiB     1.5 MiB        3
+        2011       136.2 MiB    68.1 MiB        2
+        2013         1.6 GiB    10.7 MiB      154
+        2014         4.6 GiB    25.2 MiB      187
+        2015         4.3 GiB    26.5 MiB      167
+        2016         5.1 GiB    46.8 MiB      112
+        2017         4.8 GiB    51.7 MiB       95
+        2018         5.3 GiB    97.9 MiB       55
+        2019         1.3 GiB    46.5 MiB       29
+        2020        25.7 GiB   113.5 MiB      232
+        2021        25.6 GiB    96.5 MiB      272
+        2022        14.6 GiB    82.7 MiB      181
+        2023        24.3 GiB    72.5 MiB      343
+        2024        17.3 GiB   104.8 MiB      169
+        14 media
+
 
 </details>
 
 ###### search
 
 <details><summary>Search captions / subtitles</summary>
```

