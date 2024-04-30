# Comparing `tmp/xklb-2.7.5.tar.gz` & `tmp/xklb-2.7.8.tar.gz`

## Comparing `xklb-2.7.5.tar` & `xklb-2.7.8.tar`

### file list

```diff
@@ -1,136 +1,135 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.5/.gitattributes
--rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.5/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/__init__.py
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/lb.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/media_printer.py
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/readme.py
--rw-r--r--   0        0        0   112110 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/av.py
--rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/row_add.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/rss_add.py
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/__init__.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/christen.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/move_list.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/scatter.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/big_dirs.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/search.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediadb/stats.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/__init__.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/media_player.py
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/surf.py
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/extract_text.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/__init__.py
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17730 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/consts.py
--rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/devices.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/nums.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/processes.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/strings.py
--rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.5/.gitignore
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.5/pyproject.toml
--rw-r--r--   0        0        0   155846 2020-02-02 00:00:00.000000 xklb-2.7.5/.github/README.md
--rw-r--r--   0        0        0   159627 2020-02-02 00:00:00.000000 xklb-2.7.5/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.8/.gitattributes
+-rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.8/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/__init__.py
+-rw-r--r--   0        0        0    14290 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/lb.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/media_printer.py
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/readme.py
+-rw-r--r--   0        0        0   112269 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/av.py
+-rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/christen.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/big_dirs.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/surf.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17658 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/processes.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.8/.gitignore
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.8/pyproject.toml
+-rw-r--r--   0        0        0   156014 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/README.md
+-rw-r--r--   0        0        0   159795 2020-02-02 00:00:00.000000 xklb-2.7.8/PKG-INFO
```

### Comparing `xklb-2.7.5/pdm.lock` & `xklb-2.7.8/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/LICENSE` & `xklb-2.7.8/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/Windows.md` & `xklb-2.7.8/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/examples/art.avif` & `xklb-2.7.8/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/examples/extract.svg` & `xklb-2.7.8/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/examples/tubeadd.svg` & `xklb-2.7.8/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/workflows/push.yaml` & `xklb-2.7.8/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/lb.py` & `xklb-2.7.8/xklb/lb.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "mount_stats": "Show some relative mount stats",
         "similar_folders": "Find similar folders based on folder name, size, and count",
     },
     "File subcommands": {
         "christen": "Clean file paths",
         "sample_hash": "Calculate a hash based on small file segments",
         "sample_compare": "Compare files using sample-hash and other shortcuts",
-        "similar_files": "Find similar files based on filename",
+        "similar_files": "Find similar files based on filename and size",
     },
     "Tabular data subcommands": {
         "eda": "Exploratory Data Analysis on table-like files",
         "mcda": "Multi-criteria Ranking for Decision Support",
         "incremental_diff": "Diff large table-like files in chunks",
     },
     "Media File subcommands": {
```

### Comparing `xklb-2.7.5/xklb/media_printer.py` & `xklb-2.7.8/xklb/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/readme.py` & `xklb-2.7.8/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/usage.py` & `xklb-2.7.8/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1917,14 +1917,19 @@
     Find similar files based on ONLY foldernames, using the full path
 
         $ library similar-files --no-filter-sizes --full-path ~/d/
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
+
+    Read paths from dbs
+
+        $ library similar-files --dbs db1.db db2.db
+
 """
 
 similar_folders = """library similar-folders PATH ...
 
     Find similar folders based on foldernames, similar size, and similar number of files
 
         $ library similar-folders ~/d/
@@ -1946,13 +1951,17 @@
 
         $ library similar-folders --no-filter-names --no-filter-counts ~/d/
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
+    Read paths from dbs
+
+        $ library similar-folders --dbs db1.db db2.db
+
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 """
```

### Comparing `xklb-2.7.5/xklb/createdb/av.py` & `xklb-2.7.8/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/fs_add.py` & `xklb-2.7.8/xklb/createdb/fs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/gallery_add.py` & `xklb-2.7.8/xklb/createdb/gallery_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/gallery_backend.py` & `xklb-2.7.8/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/hn_add.py` & `xklb-2.7.8/xklb/createdb/hn_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/links_add.py` & `xklb-2.7.8/xklb/createdb/links_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/places_import.py` & `xklb-2.7.8/xklb/createdb/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/reddit_add.py` & `xklb-2.7.8/xklb/createdb/reddit_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/row_add.py` & `xklb-2.7.8/xklb/createdb/row_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/site_add.py` & `xklb-2.7.8/xklb/createdb/site_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/substack.py` & `xklb-2.7.8/xklb/createdb/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/subtitle.py` & `xklb-2.7.8/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/tabs_add.py` & `xklb-2.7.8/xklb/createdb/tabs_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 from random import randint
 
 from xklb import usage
 from xklb.mediadb import db_history, db_media
 from xklb.utils import arggroups, consts, db_utils, iterables, objects, path_utils, strings
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tabs-add", usage=usage.tabs_add)
     arggroups.extractor(parser)
     arggroups.frequency(parser)
 
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--allow-immediate", action="store_true")
     arggroups.debug(parser)
     arggroups.database(parser)
-    parser.add_argument("paths", nargs="+")
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
     args.frequency = strings.partial_startswith(args.frequency, consts.frequency)
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
@@ -84,14 +85,15 @@
     }
 
 
 def tabs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
     args = parse_args()
+    args.paths = list(gen_paths(args))
 
     tabs = iterables.list_dict_filter_bool([consolidate_url(args, path) for path in get_new_paths(args)])
     for tab in tabs:
         db_media.add(args, tab)
     if not args.allow_immediate and args.frequency != "daily":
         # prevent immediately opening -- pick a random day within the week
         min_date = datetime.today() - timedelta(days=get_days(args.frequency) - 2)  # at least two days away
```

### Comparing `xklb-2.7.5/xklb/createdb/tildes.py` & `xklb-2.7.8/xklb/createdb/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/tube_add.py` & `xklb-2.7.8/xklb/createdb/tube_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/tube_backend.py` & `xklb-2.7.8/xklb/createdb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/createdb/web_add.py` & `xklb-2.7.8/xklb/createdb/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/data/imagemagick_errors.py` & `xklb-2.7.8/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/data/wordbank.py` & `xklb-2.7.8/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/data/yt_dlp_errors.py` & `xklb-2.7.8/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/editdb/dedupe_db.py` & `xklb-2.7.8/xklb/editdb/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/editdb/dedupe_media.py` & `xklb-2.7.8/xklb/editdb/dedupe_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/editdb/merge_online_local.py` & `xklb-2.7.8/xklb/editdb/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/editdb/mpv_watchlater.py` & `xklb-2.7.8/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/editdb/pushshift.py` & `xklb-2.7.8/xklb/editdb/pushshift.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     args = parse_args("pushshift", usage=usage.pushshift)
 
     args.db.enable_wal()
 
     count = 0
     reddit_posts = []
     media = []
+    print("Reading from stdin...", file=sys.stderr)
     for line in sys.stdin:
         line = line.rstrip("\n")
         if line in ["", '""', "\n"]:
             continue
 
         try:
             post_dict = orjson.loads(line)
```

### Comparing `xklb-2.7.5/xklb/editdb/reddit_selftext.py` & `xklb-2.7.8/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/files/christen.py` & `xklb-2.7.8/xklb/files/christen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse, shutil
-from os import fsdecode
+from os import fsdecode, fsencode
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, objects, path_utils
+from xklb.utils import arggroups, file_utils, objects, path_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library christen", usage=usage.christen)
     parser.add_argument("--dot-space", action="store_true")
     parser.add_argument("--case-insensitive", action="store_true")
     parser.add_argument("--lowercase-folders", action="store_true")
-    parser.add_argument("--overwrite", "-f", action="store_true")
+    parser.add_argument("--overwrite", "--force", action="store_true")
     parser.add_argument("--run", "-r", action="store_true")
     arggroups.debug(parser)
 
-    parser.add_argument("paths", nargs="*")
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def rename_path(args, base, b) -> None:
@@ -65,15 +65,17 @@
 
 def christen() -> None:
     args = parse_args()
 
     for path in args.paths:
         base = Path(path).resolve()
         log.info("[%s]: Processing subfolders...", base)
-        subpaths = sorted((bytes(p.relative_to(base)) for p in base.rglob("*")), key=len, reverse=True)
+        subpaths = sorted(
+            (fsencode(p) for p in file_utils.rglob(str(base), args.ext or None)[0]), key=len, reverse=True
+        )
         for p in subpaths:
             rename_path(args, base, p)
 
     print(
         r"""
     You may want to run bfs to remove nested empty folders:
```

### Comparing `xklb-2.7.5/xklb/files/sample_compare.py` & `xklb-2.7.8/xklb/files/sample_compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 import argparse, hashlib
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from xklb import usage
 from xklb.files import sample_hash
 from xklb.utils import arggroups, nums, objects
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
+def parse_args():
+    parser = argparse.ArgumentParser(prog="library sample-compare", usage=usage.sample_compare)
+    arggroups.sample_hash_bytes(parser)
+    parser.add_argument("--ignore-holes", "--ignore-sparse", action="store_true")
+    parser.add_argument("--skip-full-hash", action="store_true")
+    arggroups.debug(parser)
+
+    arggroups.paths_or_stdin(parser)
+    args = parser.parse_args()
+
+    args.gap = nums.float_from_percent(args.gap)
+
+    log.info(objects.dict_filter_bool(args.__dict__))
+    return args
+
+
 def full_hash_file(path):
     sha256_hash = hashlib.sha256()
 
     try:
         with open(path, "rb") as file:
             for byte_block in iter(lambda: file.read(1048576), b""):
                 sha256_hash.update(byte_block)
@@ -73,27 +90,17 @@
     else:
         log.error("Files are not equal:\n%s", paths_str)
 
     return is_equal
 
 
 def sample_compare() -> None:
-    parser = argparse.ArgumentParser(prog="library sample-compare", usage=usage.sample_compare)
-    arggroups.sample_hash_bytes(parser)
-    parser.add_argument("--ignore-holes", "--ignore-sparse", action="store_true")
-    parser.add_argument("--skip-full-hash", action="store_true")
-    arggroups.debug(parser)
-
-    parser.add_argument("paths", nargs="+")
-    args = parser.parse_args()
-
-    args.gap = nums.float_from_percent(args.gap)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    args = parse_args()
 
+    args.paths = list(gen_paths(args))
     is_equal = sample_cmp(
         *args.paths,
         threads=args.threads,
         gap=args.gap,
         chunk_size=args.chunk_size,
         ignore_holes=args.ignore_holes,
         skip_full_hash=args.skip_full_hash,
```

### Comparing `xklb-2.7.5/xklb/files/sample_hash.py` & `xklb-2.7.8/xklb/files/sample_hash.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 import argparse, hashlib, shlex
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 
 from xklb import usage
 from xklb.utils import arggroups, nums, objects
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
+def parse_args():
+    parser = argparse.ArgumentParser(prog="library sample-hash", usage=usage.sample_hash)
+    arggroups.sample_hash_bytes(parser)
+    arggroups.debug(parser)
+
+    arggroups.paths_or_stdin(parser)
+    args = parser.parse_args()
+
+    args.gap = nums.float_from_percent(args.gap)
+
+    log.info(objects.dict_filter_bool(args.__dict__))
+    return args
+
+
 def single_thread_read(path, segments, chunk_size):
     with open(path, "rb") as f:
         for start in segments:
             f.seek(start)
             yield f.read(chunk_size)
 
 
@@ -54,29 +69,20 @@
     for d in data:
         file_hash.update(d)
     file_hash_hex = file_hash.hexdigest()
     return file_hash_hex
 
 
 def sample_hash() -> None:
-    parser = argparse.ArgumentParser(prog="library sample-hash", usage=usage.sample_hash)
-    arggroups.sample_hash_bytes(parser)
-    arggroups.debug(parser)
-
-    parser.add_argument("paths", nargs="+")
-    args = parser.parse_args()
-
-    args.gap = nums.float_from_percent(args.gap)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    args = parse_args()
 
     with ThreadPoolExecutor(max_workers=4) as pool:
         future_to_path = {
             pool.submit(sample_hash_file, path, threads=args.threads, gap=args.gap, chunk_size=args.chunk_size): path
-            for path in args.paths
+            for path in gen_paths(args)
         }
         for future in as_completed(future_to_path):
             path = future_to_path[future]
             try:
                 file_hash_hex = future.result()
                 print(file_hash_hex, shlex.quote(path), sep="\t")
             except Exception as e:
```

### Comparing `xklb-2.7.5/xklb/files/similar_files.py` & `xklb-2.7.8/xklb/files/similar_files.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/merge_folders.py` & `xklb-2.7.8/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/mount_stats.py` & `xklb-2.7.8/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/move_list.py` & `xklb-2.7.8/xklb/folders/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/rel_mv.py` & `xklb-2.7.8/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/scatter.py` & `xklb-2.7.8/xklb/folders/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/folders/similar_folders.py` & `xklb-2.7.8/xklb/folders/similar_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/fsdb/big_dirs.py` & `xklb-2.7.8/xklb/fsdb/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/fsdb/disk_usage.py` & `xklb-2.7.8/xklb/fsdb/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/fsdb/search_db.py` & `xklb-2.7.8/xklb/fsdb/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/block.py` & `xklb-2.7.8/xklb/mediadb/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/db_history.py` & `xklb-2.7.8/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/db_media.py` & `xklb-2.7.8/xklb/mediadb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/db_playlists.py` & `xklb-2.7.8/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/download.py` & `xklb-2.7.8/xklb/mediadb/download.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/download_status.py` & `xklb-2.7.8/xklb/mediadb/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/history.py` & `xklb-2.7.8/xklb/mediadb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/history_add.py` & `xklb-2.7.8/xklb/mediadb/history_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/optimize_db.py` & `xklb-2.7.8/xklb/mediadb/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/playlists.py` & `xklb-2.7.8/xklb/mediadb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/redownload.py` & `xklb-2.7.8/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/search.py` & `xklb-2.7.8/xklb/mediadb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediadb/stats.py` & `xklb-2.7.8/xklb/mediadb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/mediafiles/media_check.py` & `xklb-2.7.8/xklb/mediafiles/media_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import argparse, fractions, json, os, shlex, subprocess, tempfile
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from shutil import which
 
 from xklb import usage
 from xklb.utils import arggroups, consts, file_utils, nums, objects, printing, processes, strings
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(prog="library media-check", usage=usage.media_check)
     arggroups.capability_delete(parser)
     arggroups.media_check(parser)
     arggroups.debug(parser)
-    parser.add_argument("paths", nargs="+")
+
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     args.gap = nums.float_from_percent(args.gap)
     if args.delete_corrupt:
         args.delete_corrupt = nums.float_from_percent(args.delete_corrupt)
     if args.full_scan_if_corrupt:
         args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
@@ -157,14 +159,15 @@
         if corruption_threshold_exceeded(full_scan_if_corrupt, corruption, duration):
             corruption = decode_full_scan(path, audio_scan=audio_scan, threads=threads)
     return corruption
 
 
 def media_check() -> None:
     args = parse_args()
+    args.paths = list(gen_paths(args))
 
     with ThreadPoolExecutor(max_workers=1 if args.verbose >= consts.LOG_DEBUG else 4) as pool:
         future_to_path = {
             pool.submit(
                 calculate_corruption,
                 path,
                 chunk_size=args.chunk_size,
```

### Comparing `xklb-2.7.5/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.7.8/xklb/mediafiles/process_ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.mediafiles import process_image
 from xklb.utils import arggroups, nums, objects, path_utils, processes, web
-from xklb.utils.arg_utils import kwargs_overwrite
+from xklb.utils.arg_utils import gen_paths, kwargs_overwrite
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library process-ffmpeg", usage=usage.process_ffmpeg)
     arggroups.capability_simulate(parser)
     arggroups.process_ffmpeg(parser)
     parser.add_argument("--delete-unplayable", action="store_true")
     arggroups.debug(parser)
 
-    parser.add_argument("paths", nargs="+")
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
     args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
@@ -256,15 +256,15 @@
 
     return output_path
 
 
 def process_ffmpeg():
     args = parse_args()
 
-    for path in args.paths:
+    for path in gen_paths(args):
         if not path.startswith("http"):
             path = str(Path(path).resolve())
 
         try:
             process_path(args, path)
         except Exception:
             print(path)
```

### Comparing `xklb-2.7.5/xklb/mediafiles/process_image.py` & `xklb-2.7.8/xklb/mediafiles/process_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.data import imagemagick_errors
 from xklb.utils import arggroups, objects, path_utils, processes, web
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library process-image", usage=usage.process_image)
     arggroups.capability_simulate(parser)
     parser.add_argument("--delete-unplayable", action="store_true")
 
     parser.add_argument("--max-image-height", type=int, default=2400)
     parser.add_argument("--max-image-width", type=int, default=2400)
     arggroups.debug(parser)
 
-    parser.add_argument("paths", nargs="+")
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def process_path(args, path):
@@ -93,15 +94,15 @@
 
     return output_path
 
 
 def process_image():
     args = parse_args()
 
-    for path in args.paths:
+    for path in gen_paths(args):
         if not path.startswith("http"):
             path = str(Path(path).resolve())
 
         try:
             process_path(args, path)
         except Exception:
             print(path)
```

### Comparing `xklb-2.7.5/xklb/misc/dedupe_czkawka.py` & `xklb-2.7.8/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/misc/export_text.py` & `xklb-2.7.8/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/multidb/copy_play_counts.py` & `xklb-2.7.8/xklb/multidb/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/multidb/merge_dbs.py` & `xklb-2.7.8/xklb/multidb/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/links_open.py` & `xklb-2.7.8/xklb/playback/links_open.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/media_player.py` & `xklb-2.7.8/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/play_actions.py` & `xklb-2.7.8/xklb/playback/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/playback_control.py` & `xklb-2.7.8/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/post_actions.py` & `xklb-2.7.8/xklb/playback/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/surf.py` & `xklb-2.7.8/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/playback/tabs_open.py` & `xklb-2.7.8/xklb/playback/tabs_open.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         usage=usage.tabs_open,
     )
-
     arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     args.action = action
```

### Comparing `xklb-2.7.5/xklb/scratch/javguru.py` & `xklb-2.7.8/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/scratch/javtiful.py` & `xklb-2.7.8/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/scratch/mam_search.py` & `xklb-2.7.8/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/scratch/mam_slots.py` & `xklb-2.7.8/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/tablefiles/eda.py` & `xklb-2.7.8/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/tablefiles/incremental_diff.py` & `xklb-2.7.8/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/tablefiles/mcda.py` & `xklb-2.7.8/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/text/cluster_sort.py` & `xklb-2.7.8/xklb/text/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/text/extract_links.py` & `xklb-2.7.8/xklb/text/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/text/extract_text.py` & `xklb-2.7.8/xklb/text/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/text/markdown_links.py` & `xklb-2.7.8/xklb/text/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/text/nouns.py` & `xklb-2.7.8/xklb/text/nouns.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,9 +60,10 @@
 
 
 def nouns() -> None:
     parser = argparse.ArgumentParser(usage.nouns)
     arggroups.debug(parser)
     args = parser.parse_args()
 
+    print("Reading from stdin...", file=sys.stderr)
     for line in sys.stdin:
         line_processor(line)
```

### Comparing `xklb-2.7.5/xklb/utils/arg_utils.py` & `xklb-2.7.8/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/arggroups.py` & `xklb-2.7.8/xklb/utils/arggroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,27 +32,22 @@
     capability_delete(parser)
     parser.add_argument("--db", "-db", help="Positional argument override")
     parser.add_argument("database")
 
 
 def paths_or_stdin(parser):
     parser.add_argument(
-        "--paths-from-text",
-        "--files",
-        "--file",
-        "-f",
-        action="store_true",
-        help="Read paths from line-delimited file(s)",
+        "--paths-from-text", "--files", action="store_true", help="Read paths from line-delimited file(s)"
     )
-    parser.add_argument("--paths-from-dbs", "--fsdbs", "--fsdb", action="store_true", help="Read paths from db(s)")
+    parser.add_argument("--paths-from-dbs", "--fsdbs", "--dbs", action="store_true", help="Read paths from db(s)")
     parser.add_argument("--titles-from-dbs", action="store_true", help="Read titles from db(s) instead of paths")
+    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
     parser.add_argument(
         "paths", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
     )
-    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
 
 
 def sql_fs(parser):
     parser.add_argument("--print", "-p", default="", const="p", nargs="?")
     parser.add_argument("--cols", "--col", nargs="*", help="Include specific column(s) when printing")
 
     parser.add_argument("--limit", "--queue", "--count", "-n", "-L", "-l")
@@ -263,15 +258,14 @@
     parser.add_argument(
         "--retry-delay",
         default="14 days",
         help="Must be specified in SQLITE Modifiers format: N seconds, minutes, hours, days, months, or years",
     )
     parser.add_argument(
         "--force",
-        "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
 
 
 def download_subtitle(parser):
     parser.add_argument("--subs", action="store_true")
```

### Comparing `xklb-2.7.5/xklb/utils/argparse_utils.py` & `xklb-2.7.8/xklb/utils/argparse_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
 class ArgparseArgsOrStdin(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if values == STDIN_DASH:
+            print("Reading from stdin...", file=sys.stderr)
             lines = sys.stdin.readlines()
             if not lines or (len(lines) == 1 and lines[0].strip() == ""):
                 lines = None
             else:
                 lines = [s.strip() for s in lines]
         else:
             lines = values
```

### Comparing `xklb-2.7.5/xklb/utils/consts.py` & `xklb-2.7.8/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/db_utils.py` & `xklb-2.7.8/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/devices.py` & `xklb-2.7.8/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/file_utils.py` & `xklb-2.7.8/xklb/utils/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     filtered_files = set()
     folders = set()
     stack = [base_dir]
     while stack:
         current_dir = stack.pop()
         try:
             scanned_dir = os.scandir(current_dir)
-        except FileNotFoundError:
+        except (FileNotFoundError, PermissionError):
             pass
         else:
             for entry in scanned_dir:
                 if entry.is_dir(follow_symlinks=False):
                     folders.add(entry.path)
                     stack.append(entry.path)
                 else:
```

### Comparing `xklb-2.7.5/xklb/utils/gui.py` & `xklb-2.7.8/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/iterables.py` & `xklb-2.7.8/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/log_utils.py` & `xklb-2.7.8/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/mpv_utils.py` & `xklb-2.7.8/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/nums.py` & `xklb-2.7.8/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/objects.py` & `xklb-2.7.8/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/path_utils.py` & `xklb-2.7.8/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/pd_utils.py` & `xklb-2.7.8/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/printing.py` & `xklb-2.7.8/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/processes.py` & `xklb-2.7.8/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/sql_utils.py` & `xklb-2.7.8/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/strings.py` & `xklb-2.7.8/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/utils/web.py` & `xklb-2.7.8/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/xklb/assets/kotobago.png` & `xklb-2.7.8/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.gitignore` & `xklb-2.7.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/pyproject.toml` & `xklb-2.7.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.7.5/.github/README.md` & `xklb-2.7.8/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.7.005)
+    xk media library subcommands (v2.7.008)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -160,15 +160,15 @@
     ╭────────────────┬─────────────────────────────────────────────────────╮
     │ christen       │ Clean file paths                                    │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-hash    │ Calculate a hash based on small file segments       │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-compare │ Compare files using sample-hash and other shortcuts │
     ├────────────────┼─────────────────────────────────────────────────────┤
-    │ similar-files  │ Find similar files based on filename                │
+    │ similar-files  │ Find similar files based on filename and size       │
     ╰────────────────┴─────────────────────────────────────────────────────╯
 
     Tabular data subcommands:
     ╭──────────────────┬───────────────────────────────────────────────╮
     │ eda              │ Exploratory Data Analysis on table-like files │
     ├──────────────────┼───────────────────────────────────────────────┤
     │ mcda             │ Multi-criteria Ranking for Decision Support   │
@@ -1312,14 +1312,18 @@
 
         $ library similar-folders --no-filter-names --no-filter-counts ~/d/
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
+    Read paths from dbs
+
+        $ library similar-folders --dbs db1.db db2.db
+
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 
 
@@ -1377,15 +1381,15 @@
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
 ###### similar-files
 
-<details><summary>Find similar files based on filename</summary>
+<details><summary>Find similar files based on filename and size</summary>
 
     $ library similar-files -h
     usage: library similar-files PATH ...
 
     Find similar files using filenames and size
 
         $ library similar-files ~/d/
@@ -1394,14 +1398,19 @@
 
         $ library similar-files --no-filter-sizes --full-path ~/d/
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
 
+    Read paths from dbs
+
+        $ library similar-files --dbs db1.db db2.db
+
+
 
 </details>
 
 ### Tabular data subcommands
 
 ###### eda
```

### Comparing `xklb-2.7.5/PKG-INFO` & `xklb-2.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.7.5
+Version: 2.7.8
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -182,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.7.005)
+    xk media library subcommands (v2.7.008)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -249,15 +249,15 @@
     ╭────────────────┬─────────────────────────────────────────────────────╮
     │ christen       │ Clean file paths                                    │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-hash    │ Calculate a hash based on small file segments       │
     ├────────────────┼─────────────────────────────────────────────────────┤
     │ sample-compare │ Compare files using sample-hash and other shortcuts │
     ├────────────────┼─────────────────────────────────────────────────────┤
-    │ similar-files  │ Find similar files based on filename                │
+    │ similar-files  │ Find similar files based on filename and size       │
     ╰────────────────┴─────────────────────────────────────────────────────╯
 
     Tabular data subcommands:
     ╭──────────────────┬───────────────────────────────────────────────╮
     │ eda              │ Exploratory Data Analysis on table-like files │
     ├──────────────────┼───────────────────────────────────────────────┤
     │ mcda             │ Multi-criteria Ranking for Decision Support   │
@@ -1401,14 +1401,18 @@
 
         $ library similar-folders --no-filter-names --no-filter-counts ~/d/
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
+    Read paths from dbs
+
+        $ library similar-folders --dbs db1.db db2.db
+
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 
 
@@ -1466,15 +1470,15 @@
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
 ###### similar-files
 
-<details><summary>Find similar files based on filename</summary>
+<details><summary>Find similar files based on filename and size</summary>
 
     $ library similar-files -h
     usage: library similar-files PATH ...
 
     Find similar files using filenames and size
 
         $ library similar-files ~/d/
@@ -1483,14 +1487,19 @@
 
         $ library similar-files --no-filter-sizes --full-path ~/d/
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
 
+    Read paths from dbs
+
+        $ library similar-files --dbs db1.db db2.db
+
+
 
 </details>
 
 ### Tabular data subcommands
 
 ###### eda
```

