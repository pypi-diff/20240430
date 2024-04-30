# Comparing `tmp/pygpt_net-2.2.3.tar.gz` & `tmp/pygpt_net-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.3.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.4.tar", max compression
```

## Comparing `pygpt_net-2.2.3.tar` & `pygpt_net-2.2.4.tar`

### file list

```diff
@@ -1,844 +1,844 @@
--rwxr-xr-x   0        0        0    57909 2024-04-29 10:51:04.357787 pygpt_net-2.2.3/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.3/LICENSE
--rwxr-xr-x   0        0        0   132129 2024-04-29 10:51:04.357787 pygpt_net-2.2.3/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.3/icon.png
--rw-r--r--   0        0        0     2979 2024-04-29 10:51:04.361787 pygpt_net-2.2.3/pyproject.toml
--rwxr-xr-x   0        0        0    56887 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.3/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    15484 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.3/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.3/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     9877 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    16076 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    13996 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    14251 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15540 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.3/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.3/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2144 2024-03-15 15:31:21.786121 pygpt_net-2.2.3/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.3/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.3/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.3/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.3/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.3/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.3/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.3/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.3/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.3/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.3/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.3/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.3/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.3/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.3/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    13084 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15668 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.3/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.3/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.3/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.3/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    20106 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.3/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.3/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.3/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.3/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.3/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.3/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.3/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.3/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.3/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.3/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.3/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.3/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.3/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.3/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.3/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9236 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7998 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.3/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.3/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.3/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.3/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.3/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.3/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.3/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.3/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.3/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.3/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.3/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.3/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.3/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.3/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.3/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.3/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.3/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.3/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.3/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.3/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.3/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.3/src/pygpt_net/core/dispatcher.py
--rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.3/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.3/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.3/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.3/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.3/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.3/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.3/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.3/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.3/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.3/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.3/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.3/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.3/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.3/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.3/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.3/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.3/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.3/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.3/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.3/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.3/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.3/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.3/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.3/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    42853 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.3/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.3/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.3/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.3/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0    10603 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    18526 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1440 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.completion.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.3/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.3/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.3/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.3/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.3/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.3/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.3/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.3/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.3/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.3/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.3/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.3/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.3/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    45308 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    53672 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    45481 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    47105 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    44558 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    44462 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    62742 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    48231 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.3/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.3/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.3/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.3/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.3/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.3/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.3/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.3/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.3/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.3/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.3/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.3/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.3/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.3/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.3/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.3/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.3/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.3/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.3/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.3/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.3/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.3/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5125 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10392 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.3/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.3/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.3/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     6961 2024-03-08 00:36:17.343108 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    26515 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    19981 2024-04-29 05:51:11.644212 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    12886 2024-04-29 10:51:04.365787 pygpt_net-2.2.3/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.3/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.3/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.3/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.3/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.3/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.3/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.3/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.3/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.3/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.3/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    18684 2024-04-29 10:51:04.369787 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5356 2024-04-27 07:58:32.754704 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.3/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4427 2024-04-27 07:58:32.754704 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.3/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.3/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.3/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.3/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.3/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.3/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.3/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.3/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.3/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.3/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.3/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.3/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.3/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.3/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.3/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     2854 2024-04-14 20:50:29.556142 pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.3/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     1956 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.3/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.3/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.3/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.3/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.3/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   135845 1970-01-01 00:00:00.000000 pygpt_net-2.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0    58137 2024-04-29 15:13:32.567516 pygpt_net-2.2.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.4/LICENSE
+-rwxr-xr-x   0        0        0   132359 2024-04-29 15:13:32.567516 pygpt_net-2.2.4/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.4/icon.png
+-rw-r--r--   0        0        0     2979 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/pyproject.toml
+-rwxr-xr-x   0        0        0    57113 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.4/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15484 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/__init__.py
+-rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.4/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.4/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    19949 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    13989 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    15446 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15540 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.4/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2144 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.4/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.4/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.4/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.4/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.4/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    13539 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15668 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.4/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.4/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.4/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.4/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    20106 2024-04-29 10:51:04.365787 pygpt_net-2.2.4/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.4/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.4/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.4/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.4/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.4/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.4/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.4/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.4/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9839 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7998 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.4/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.4/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.4/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.4/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.4/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.4/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.4/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/dispatcher.py
+-rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.4/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.4/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.4/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.4/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.4/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.4/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.4/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.4/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.4/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.4/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    42853 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.4/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.4/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.4/src/pygpt_net/core/worker.py
+-rwxr-xr-x   0        0        0    10603 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    18526 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1440 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.completion.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.4/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.4/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.4/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    46483 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    54728 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    46620 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    48330 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    45664 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    45600 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    64199 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    49212 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.4/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.4/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.4/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.4/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.4/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.4/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.4/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.4/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.4/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.4/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.4/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     6961 2024-03-08 00:36:17.343108 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    29315 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    19981 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    14743 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.4/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.4/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.4/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.4/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    22284 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.4/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4420 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.4/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.4/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.4/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   136075 1970-01-01 00:00:00.000000 pygpt_net-2.2.4/PKG-INFO
```

### Comparing `pygpt_net-2.2.3/CHANGELOG.md` & `pygpt_net-2.2.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+# 2.2.4 (2024-04-29)
+
+- Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
+- Added sync current/all context menu options to Sync button.
+- Improved remote stores handling.
+
 # 2.2.3 (2024-04-29)
 
 - Fixed Assistants files sync btn.
 - Added batch upload files or directory in Assistants vector stores dialog.
 
 # 2.2.2 (2024-04-29)
```

### Comparing `pygpt_net-2.2.3/LICENSE` & `pygpt_net-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/README.md` & `pygpt_net-2.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.3** | build: **2024.04.29** | Python: **>=3.10, <3.12**
+Release: **2.2.4** | build: **2024.04.29** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -3054,14 +3054,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.4 (2024-04-29)**
+
+- Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
+- Added sync current/all context menu options to Sync button.
+- Improved remote stores handling.
+
 **2.2.3 (2024-04-29)**
 
 - Fixed Assistants files sync btn.
 - Added batch upload files or directory in Assistants vector stores dialog.
 
 **2.2.2 (2024-04-29)**
```

### Comparing `pygpt_net-2.2.3/icon.png` & `pygpt_net-2.2.4/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/pyproject.toml` & `pygpt_net-2.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.3"
+version = "2.2.4"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.4/src/pygpt_net/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.2.4 (2024-04-29)
+
+- Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
+- Added sync current/all context menu options to Sync button.
+- Improved remote stores handling.
+
 2.2.3 (2024-04-29)
 
 - Fixed Assistants files sync btn.
 - Added batch upload files or directory in Assistants vector stores dialog.
 
 2.2.2 (2024-04-29)
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/LICENSE` & `pygpt_net-2.2.4/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __build__ = "2024.04.29"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/app.py` & `pygpt_net-2.2.4/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/config.py` & `pygpt_net-2.2.4/src/pygpt_net/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/container.py` & `pygpt_net-2.2.4/src/pygpt_net/container.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import webbrowser
 
 from pygpt_net.item.assistant import AssistantItem
 
 from .batch import Batch
@@ -232,15 +232,15 @@
         if idx is not None:
             id = self.window.core.assistants.get_by_idx(idx)
             if id is not None and id != "":
                 if self.window.core.assistants.has(id):
                     # if exists then show confirmation dialog
                     if not force:
                         self.window.ui.dialogs.confirm(
-                            type='assistant_delete',
+                            type='assistant.delete',
                             id=idx,
                             msg=trans('confirm.assistant.delete'),
                         )
                         return
 
                     # clear if this is current assistant
                     if id == self.window.core.config.get('assistant'):
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 
 from PySide6.QtWidgets import QApplication, QFileDialog
 
 from pygpt_net.utils import trans
 
@@ -29,15 +29,15 @@
         """
         Import all remote assistants from API
 
         :param force: if true, imports without confirmation
         """
         if not force:
             self.window.ui.dialogs.confirm(
-                type='assistant_import',
+                type='assistant.import',
                 id='',
                 msg=trans('confirm.assistant.import'),
             )
             return
 
         # run asynchronous
         self.window.ui.status("Importing assistants...please wait...")
@@ -59,36 +59,66 @@
         # run asynchronous
         self.window.ui.status("Importing vector stores...please wait...")
         self.window.core.assistants.store.truncate()  # clear all stores
         self.window.core.gpt.assistants.importer.import_vector_stores()
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
 
+    def import_files_current(self):
+        """Import files from API"""
+        id = self.window.core.config.get('assistant')
+        if id is None or id == "":
+            return
+        if self.window.core.assistants.has(id):
+            assistant = self.window.core.assistants.get_by_id(id)
+            store_id = assistant.vector_store
+            if store_id is None or store_id == "":
+                self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.assign"))
+                return
+            self.import_store_files(store_id)
+
     def import_files(self, force: bool = False):
         """
-        Sync files with API
+        Sync files with API (all)
 
         :param force: force sync files
         """
         if not force:
             self.window.ui.dialogs.confirm(
-                type='assistant_import_files',
+                type='assistant.files.import.all',
                 id='',
                 msg=trans('confirm.assistant.import_files'),
             )
             return
+        try:
+            self.window.controller.assistant.files.import_files()  # all
+        except Exception as e:
+            self.window.core.debug.log(e)
+            self.window.ui.dialogs.alert(e)
 
-        id = self.window.core.config.get('assistant')
-        if id is None or id == "":
+    def import_store_files(self, store_id: str, force: bool = False):
+        """
+        Sync files with API (store)
+
+        :param store_id: vector store ID
+        :param force: force sync files
+        """
+        if store_id is None:
+            self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.select"))
             return
-        assistant = self.window.core.assistants.get_by_id(id)
-        if assistant is None:
+
+        if not force:
+            self.window.ui.dialogs.confirm(
+                type='assistant.files.import.store',
+                id=store_id,
+                msg=trans('confirm.assistant.import_files.store'),
+            )
             return
         try:
-            self.window.controller.assistant.files.import_files(assistant)
+            self.window.controller.assistant.files.import_files(store_id)  # by store
         except Exception as e:
             self.window.core.debug.log(e)
             self.window.ui.dialogs.alert(e)
 
     def truncate_files(self, force: bool = False):
         """
         Truncate all files in API
@@ -103,23 +133,90 @@
             )
             return
         # run asynchronous
         self.window.ui.status("Removing files...please wait...")
         QApplication.processEvents()
         self.window.core.gpt.assistants.importer.truncate_files()  # remove all files from API
 
+    def truncate_store_files_by_idx(self, idx: int, force: bool = False):
+        """
+        Truncate all files in API (store)
+
+        :param idx: store index
+        :param force: if true, imports without confirmation
+        """
+        store_id = self.window.controller.assistant.store.get_by_tab_idx(idx)
+        self.truncate_store_files(store_id, force)
+
+    def truncate_store_files(self, store_id: str, force: bool = False):
+        """
+        Truncate all files in API (store)
+
+        :param store_id: store ID
+        :param force: if true, imports without confirmation
+        """
+        if store_id is None:
+            self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.select"))
+            return
+
+        if not force:
+            self.window.ui.dialogs.confirm(
+                type='assistant.files.truncate.store',
+                id=store_id,
+                msg=trans('confirm.assistant.files.truncate.store'),
+            )
+            return
+        # run asynchronous
+        self.window.ui.status("Removing files...please wait...")
+        QApplication.processEvents()
+        self.window.core.gpt.assistants.importer.truncate_files(store_id)  # remove all files from API
+
+    def clear_store_files_by_idx(self, idx: int, force: bool = False):
+        """
+        Clear files (store, local only)
+
+        :param idx: store index
+        :param force: if true, clears without confirmation
+        """
+        store_id = self.window.controller.assistant.store.get_by_tab_idx(idx)
+        self.clear_store_files(store_id, force)
+
+    def clear_store_files(self, store_id: str = None, force: bool = False):
+        """
+        Clear files (store, local only)
+
+        :param store_id: store ID
+        :param force: if true, clears without confirmation
+        """
+        if store_id is None:
+            self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.select"))
+            return
+
+        if not force:
+            self.window.ui.dialogs.confirm(
+                type='assistant.files.clear.store',
+                id=store_id,
+                msg=trans('confirm.assistant.files.clear'),
+            )
+            return
+        self.window.ui.status("Clearing store files...please wait...")
+        self.window.core.assistants.files.truncate_local(store_id)  # clear files local
+        self.window.controller.assistant.files.update()
+        self.window.ui.status("OK. All store files cleared.")
+        self.window.ui.dialogs.alert(trans("status.finished"))
+
     def clear_files(self, force: bool = False):
         """
-        Clear files (local only)
+        Clear files (all, local only)
 
         :param force: if true, clears without confirmation
         """
         if not force:
             self.window.ui.dialogs.confirm(
-                type='assistant.files.clear',
+                type='assistant.files.clear.all',
                 id='',
                 msg=trans('confirm.assistant.files.clear'),
             )
             return
         self.window.ui.status("Clearing files...please wait...")
         self.window.core.assistants.files.truncate_local()  # clear files local
         self.window.controller.assistant.files.update()
@@ -303,21 +400,24 @@
         """
         self.window.core.debug.log(error)
         print("Error importing files")
         self.window.ui.status("Error importing files.")
         self.window.ui.dialogs.alert(error)
         self.window.controller.assistant.files.update()
 
-    def handle_truncated_files(self, num: int):
+    def handle_truncated_files(self, store_id: str = None, num: int = 0):
         """
         Handle truncated (in API) files
 
+        :param store_id: vector store ID
         :param num: number of truncated files
         """
         self.window.ui.status("OK. Truncated files: " + str(num) + ".")
+        if store_id is not None:
+            self.window.controller.assistant.store.refresh_by_store_id(store_id)
         self.window.controller.assistant.files.update()
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def handle_truncated_files_failed(self, error: any):
         """
         Handle error on truncated files
 
@@ -406,15 +506,15 @@
     def upload(self, force: bool = False):
         """
         Upload files to vector store
 
         :param force: if true, uploads without confirmation
         """
         if self.window.controller.assistant.store.current is None:
-            self.window.ui.dialogs.alert("Please select vector store first.")
+            self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.select"))
             return
 
         store_id = self.window.controller.assistant.store.current
         self.window.core.gpt.assistants.importer.upload_files(store_id, self.files_to_upload)
         self.files_to_upload = []  # clear files
 
     def handle_uploaded_files(self, num: int):
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.item.assistant import AssistantItem
@@ -60,23 +60,23 @@
         num = 0
         for id in list(attachments):
             attachment = attachments[id]
             if not attachment.send:
                 num += 1  # increment uploaded files counter if file is not uploaded yet
         return num
 
-    def import_files(self, assistant: AssistantItem):
+    def import_files(self, store_id: str = None):
         """
         Import assistant files from API
 
-        :param assistant: assistant
+        :param store_id: store ID
         """
         # run asynchronous
         self.window.ui.status("Importing files...please wait...")
-        self.window.core.gpt.assistants.importer.import_files(assistant)
+        self.window.core.gpt.assistants.importer.import_files(store_id)
 
     def download(self, idx: int):
         """
         Download file
 
         :param idx: selected attachment index
         """
@@ -144,15 +144,15 @@
         """
         Delete all files
 
         :param force: force clear files
         """
         if not force:
             self.window.ui.dialogs.confirm(
-                type='attachments_uploaded.clear',
+                type='attachments.uploaded.clear',
                 id=-1,
                 msg=trans('attachments_uploaded.clear.confirm'),
             )
             return
 
         id = self.window.core.config.get('assistant')
         if id is None or id == "":
@@ -182,15 +182,15 @@
         Delete file
 
         :param idx: file idx
         :param force: force delete without confirmation
         """
         if not force:
             self.window.ui.dialogs.confirm(
-                type='attachments_uploaded.delete',
+                type='attachments.uploaded.delete',
                 id=idx,
                 msg=trans('attachments_uploaded.delete.confirm'),
             )
             return
 
         # get current assistant
         id = self.window.core.config.get('assistant')
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 14:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import copy
 import json
 
 from PySide6.QtWidgets import QApplication
 
@@ -167,14 +167,39 @@
         # update from API
         self.window.core.assistants.store.update_status(store.id)
         self.window.core.assistants.store.update(store)
 
         if update and store.id == self.current:
             self.update_current()
 
+    def refresh_by_idx(self, idx: int):
+        """
+        Refresh store by idx
+
+        :param idx: store idx
+        """
+        store_id = self.get_by_tab_idx(idx)
+        if store_id is not None:
+            self.refresh_by_store_id(store_id)
+
+    def refresh_by_store_id(self, store_id: str):
+        """
+        Refresh store by ID
+
+        :param store_id: store id
+        """
+        if store_id is not None:
+            store = self.window.core.assistants.store.items[store_id]
+            if store is not None:
+                self.window.ui.status(trans('status.sending'))
+                QApplication.processEvents()
+                self.refresh_store(store)
+                self.window.ui.status(trans('status.assistant.saved'))
+                self.update()
+
     def update_current(self):
         """Update current store"""
         if self.current is not None and self.window.core.assistants.store.has(self.current):
             store = self.window.core.assistants.store.items[self.current]
             # update textarea
             option = copy.deepcopy(self.get_option("status"))
             option["value"] = json.dumps(store.status, indent=4)
@@ -279,27 +304,41 @@
         """
         Delete store by idx
 
         :param idx: store idx
         :param force: force delete
         """
         store_id = self.get_by_tab_idx(idx)
+        self.delete(store_id, force=force)
+
+    def delete(self, store_id: str = None, force: bool = False):
+        """
+        Delete store by idx
+
+        :param store_id: store id
+        :param force: force delete
+        """
         if not force:
             self.window.ui.dialogs.confirm(
                 type="assistant.store.delete",
-                id=idx,
+                id=store_id,
                 msg=trans("dialog.assistant.store.delete.confirm"),
             )
             return
+
+        if store_id is None:
+            self.window.ui.dialogs.alert("Please select vector store first.")
+            return
+
         self.window.ui.status(trans('status.sending'))
         QApplication.processEvents()
         if self.current == store_id:
             self.current = None
-
         try:
+            print("Deleting store: {}".format(store_id))
             if self.window.core.assistants.store.delete(store_id):
                 self.window.controller.assistant.batch.remove_store_from_assistants(store_id)
                 self.window.ui.status(trans('status.deleted'))
                 self.window.core.assistants.store.save()
                 self.window.controller.assistant.files.update()
                 self.update()  # update stores list in assistant dialog
                 self.init()
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/text.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/config/placeholder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/extra.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 10:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 class Confirm:
     def __init__(self, window=None):
         """
         Confirmation dialogs controller
 
@@ -115,17 +115,17 @@
             except Exception as e:
                 self.window.core.debug.error(e)
                 self.window.ui.dialogs.alert(e)
 
         # attachments
         elif type == 'attachments.delete':
             self.window.controller.attachment.delete(id, force=True, remove_local=True)
-        elif type == 'attachments_uploaded.clear':
+        elif type == 'attachments.uploaded.clear':
             self.window.controller.assistant.files.clear(True)
-        elif type == 'attachments_uploaded.delete':
+        elif type == 'attachments.uploaded.delete':
             self.window.controller.assistant.files.delete(id, True)
         elif type == 'attachments.clear':
             self.window.controller.attachment.clear(force=True, remove_local=True)
 
         # files
         elif type == 'files.delete':
             self.window.controller.files.delete(id, True)
@@ -145,30 +145,36 @@
             self.window.tools.get("editor").open_file(id=id, force=True, save=True)
         elif type == 'editor.changed.close':
             self.window.tools.get("editor").close(id, save=True)
         elif type == 'editor.changed.restore':
             self.window.tools.get("editor").restore(id=id, force=True, save=True)
 
         # assistants
-        elif type == 'assistant_delete':
+        elif type == 'assistant.delete':
             self.window.controller.assistant.delete(id, True)
-        elif type == 'assistant_import':
-            self.window.controller.assistant.batch.import_assistants(True)
-        elif type == 'assistant_import_files':
+        elif type == 'assistant.import':
+            self.window.controller.assistant.batch.import_all(True)
+        elif type == 'assistant.files.import.all':
             self.window.controller.assistant.batch.import_files(True)
+        elif type == 'assistant.files.import.store':
+            self.window.controller.assistant.batch.import_store_files(id, True)  # by store_id
         elif type == 'assistant.files.truncate':
             self.window.controller.assistant.batch.truncate_files(True)
-        elif type == 'assistant.files.clear':
+        elif type == 'assistant.files.truncate.store':
+            self.window.controller.assistant.batch.truncate_store_files(id, True)  # by store_id
+        elif type == 'assistant.files.clear.all':
             self.window.controller.assistant.batch.clear_files(True)
+        elif type == 'assistant.files.clear.store':
+            self.window.controller.assistant.batch.clear_store_files(id, True)  # by store_id
         elif type == 'assistant.files.upload':
             self.window.controller.assistant.batch.upload(True)
 
         # assistants vector stores
         elif type == 'assistant.store.delete':
-            self.window.controller.assistant.store.delete_by_idx(id, True)
+            self.window.controller.assistant.store.delete(id, True)  # by store_id
         elif type == 'assistant.store.import':
             self.window.controller.assistant.batch.import_stores(True)
         elif type == 'assistant.store.truncate':
             self.window.controller.assistant.batch.truncate_stores(True)
         elif type == 'assistant.store.clear':
             self.window.controller.assistant.batch.clear_stores(True)
         elif type == 'assistant.store.refresh':
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/lang/mapping.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/settings/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.4/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.4/src/pygpt_net/core/assistants/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 from packaging.version import Version
 
 from pygpt_net.item.assistant import AssistantFileItem, AssistantItem
 from pygpt_net.provider.core.assistant_file.db_sqlite import DbSqliteProvider
 
@@ -213,24 +213,27 @@
         Delete file and remove from vector stores if exists
 
         :param file: file item
         :return: True if file was deleted
         """
         file_id = file.file_id
         items = self.get_all_by_file_id(file_id)  # get store_ids
-        store_ids = []
         for id in items:
             store_id = items[id].store_id
             if store_id is None or store_id == "":
                 continue  # skip if no store_id
-            if store_id in store_ids:
-                continue
-            self.window.core.gpt.assistants.vs_delete_file(store_id, file_id)  # remove from vector store
+            try:
+                self.window.core.gpt.assistants.vs_delete_file(store_id, file_id)  # remove from vector store
+            except Exception as e:
+                self.window.core.debug.log("Failed to delete file from vector store: " + str(e))
         self.provider.delete_by_id(file.record_id)  # delete file in DB
-        self.window.core.gpt.assistants.file_delete(file.file_id)  # delete file in API
+        try:
+            self.window.core.gpt.assistants.file_delete(file.file_id)  # delete file in API
+        except Exception as e:
+            self.window.core.debug.log("Failed to delete remote file: " + str(e))
         if file.record_id in self.items:
             del self.items[file.record_id]
         return True
 
     def on_store_deleted(self, store_id: str):
         """
         Clear deleted store from files
@@ -248,36 +251,43 @@
         Rename file
 
         :param record_id: record ID
         :param name: new name
         :return: True if renamed
         """
         self.provider.rename_file(record_id, name)
-        # TODO: rename in API here
         if record_id in self.items:
             self.items[record_id].name = name
         return True
 
-    def truncate(self) -> bool:
+    def truncate(self, store_id: str = None) -> bool:
         """
         Truncate all files
 
+        :param store_id: store ID
         :return: True if truncated
         """
-        self.window.core.gpt.assistants.vs_remove_files_from_stores()  # remove files from all vector stores
-        return self.truncate_local()  # truncate files in DB
+        if store_id is not None:
+            self.window.core.gpt.assistants.vs_remove_files_from_store(store_id)  # remove files from vector store
+        else:
+            self.window.core.gpt.assistants.vs_remove_files_from_stores()  # remove files from all vector stores
+        return self.truncate_local(store_id)  # truncate files in DB
 
-    def truncate_local(self) -> bool:
+    def truncate_local(self, store_id: str = None) -> bool:
         """
         Truncate all files (local only)
 
+        :param store_id: store ID
         :return: True if truncated
         """
-        self.provider.truncate()  # truncate files in DB
-        self.items = {}  # clear items
+        if store_id is not None:
+            self.provider.truncate_by_store(store_id)  # truncate files in DB (by store_id)
+        else:
+            self.provider.truncate_all()  # truncate all files in DB
+            self.items = {}  # clear items
         return True
 
     def import_from_store(self, store_id: str) -> bool:
         """
         Import files from store
 
         :param store_id: store ID
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.4/src/pygpt_net/core/assistants/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.4/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.4/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.4/src/pygpt_net/core/bridge.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.4/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.4/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.4/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/command.py` & `pygpt_net-2.2.4/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.4/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.4/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.4/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.4/src/pygpt_net/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/history.py` & `pygpt_net-2.2.4/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/image.py` & `pygpt_net-2.2.4/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/info.py` & `pygpt_net-2.2.4/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.4/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.4/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/models.py` & `pygpt_net-2.2.4/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.4/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.4/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.4/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.4/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.4/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.4/src/pygpt_net/core/prompt/template.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.4/src/pygpt_net/core/render/web/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.4/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.4/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.4/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/web.py` & `pygpt_net-2.2.4/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/config.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989384288747345%*

 * *Differences: {"'__meta__'": "{'version': '2.2.4', 'app.version': '2.2.4'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.3",
+        "app.version": "2.2.4",
         "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.3"
+        "version": "2.2.4"
     },
     "agent.auto_stop": true,
     "agent.goal.notify": true,
     "agent.idx": "base",
     "agent.iterations": 3,
     "agent.mode": "chat",
     "ai_name": "",
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/models.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'__meta__'": "{'version': '2.2.4', 'app.version': '2.2.4'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.3",
+        "app.version": "2.2.4",
         "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.3"
+        "version": "2.2.4"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/modes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'__meta__'": "{'version': '2.2.4', 'app.version': '2.2.4'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.3",
+        "app.version": "2.2.4",
         "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.3"
+        "version": "2.2.4"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/presets/current.agent.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.agent.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/settings.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.4/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.4/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.4/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.4/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.de.ini`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Name
 attachments.header.path = Pfad
 attachments.header.size = Größe
 attachments.send_clear = Liste nach dem Senden löschen
 attachments.tab = Anhänge
 attachments_uploaded.btn.clear = Dateien löschen
 attachments_uploaded.btn.sync = Synchronisieren
+attachments_uploaded.btn.sync.current = Nur aktuell
+attachments_uploaded.btn.sync.all = Alle Speicher
 attachments_uploaded.clear.confirm = WARNUNG: Sind Sie sicher, dass Sie alle diese Dateien vom Remote-Server löschen möchten?
 attachments_uploaded.delete.confirm = WARNUNG: Sind Sie sicher, dass Sie die Datei vom Remote-Server löschen möchten?
 attachments_uploaded.sync.tip = Tipp: Klicken Sie auf 'Synchronisieren', um die Dateiliste von OpenAI abzurufen
 attachments_uploaded.tab = Hochgeladene Dateien
 audio.magic_word.detected = Zauberwort erkannt!
 audio.magic_word.invalid = Kein Zauberwort :(
 audio.magic_word.please = Bitte das Zauberwort...
@@ -139,22 +141,24 @@
 chat.name.bot = KI
 clipboard.copied = In die Zwischenablage kopiert.
 clipboard.copied_to = In die Zwischenablage kopiert:
 cmd.enabled = Befehle ausführen
 cmd.tip = Tipp: Um die Ausführung von Befehlen aus Plugins zu ermöglichen, die mit "Command:" gekennzeichnet sind, müssen Sie die Option "Befehle ausführen" aktivieren.
 coming_soon = Demnächst...
 confirm.assistant.delete = Assistent löschen?
+confirm.assistant.files.clear = Dateien löschen (nur lokal)?
+confirm.assistant.files.truncate = Sind Sie sicher, dass Sie alle Dateien von allen Speichern entfernen möchten?
+confirm.assistant.files.truncate.store = Sind Sie sicher, dass Sie alle Dateien aus dem ausgewählten Speicher entfernen möchten?
 confirm.assistant.import = Alle Assistenten von API importieren?
-confirm.assistant.files.truncate = Sind Sie sicher, dass Sie alle Dateien von allen Assistenten entfernen?
 confirm.assistant.import_files = Alle Dateien von API importieren?
-confirm.assistant.store.import = Alle Vektor Speicher von API importieren?
-confirm.assistant.store.truncate = Alle Vektor Speicher im API löschen?
-confirm.assistant.store.clear = Vektor Speicher löschen (nur lokal)?
-confirm.assistant.files.clear = Dateien löschen (nur lokal)?
-confirm.assistant.store.refresh = Alle Vektor Speicher aktualisieren?
+confirm.assistant.import_files.store = Aktuelle Speicherdateien von API importieren?
+confirm.assistant.store.clear = Vektor-Speicher leeren (nur lokal)?
+confirm.assistant.store.import = Alle Vektor-Speicher von API importieren?
+confirm.assistant.store.refresh = Alle Speicher aktualisieren?
+confirm.assistant.store.truncate = Alle Vektor-Speicher in der API löschen?
 confirm.img.delete = Datei von der Festplatte löschen?
 confirm.preset.clear = Sind Sie sicher, dass Sie das Voreinstellung löschen möchten?
 confirm.preset.delete = Sind Sie sicher, dass Sie diese Voreinstellung löschen möchten?
 confirm.preset.overwrite = Voreinstellung existiert. Überschreiben?
 confirm.preset.restore = Standard-Preset für diesen Modus wiederherstellen?
 confirm.profile.delete = Sind Sie sicher, dass Sie das Profil löschen möchten? Es wird nur aus der Liste entfernt.
 confirm.profile.delete_all = Sind Sie sicher, dass Sie das Profil samt aller Konfigurationsdateien und Benutzerdateien im Profil-Arbeitsverzeichnis löschen möchten?
@@ -205,27 +209,37 @@
 dialog.about.website = Offizielle Webseite
 dialog.assistant = Assistent erstellen / bearbeiten
 dialog.assistant.btn.current = Aktuelle verwenden
 dialog.assistant.btn.close = Abbrechen
 dialog.assistant.btn.save = Speichern
 dialog.assistant.btn.store = Vektor Speicher
 dialog.assistant.store = Vektor Speicher der Assistenten
+dialog.assistant.store.alert.select = Bitte zuerst Vektor-Speicher auswählen.
+dialog.assistant.store.alert.assign = Bitte zuerst einen Vektor-Speicher dem Assistenten zuweisen.
 dialog.assistant.store.btn.close = Abbrechen
 dialog.assistant.store.btn.new = Erstellen
 dialog.assistant.store.btn.save = Speichern
 dialog.assistant.store.btn.refresh_status = Status aktualisieren
 dialog.assistant.store.btn.upload.files = + Dateien
 dialog.assistant.store.btn.upload.dir = + Verzeichnis
 dialog.assistant.store.delete.confirm = Sind Sie sicher, dass Sie den Vektor Speicher des Assistenten löschen wollen?
-dialog.assistant.store.menu.import = Alles importieren
-dialog.assistant.store.menu.refresh_store = Alles aktualisieren
-dialog.assistant.store.menu.clear_store = Vektor Speicher leeren (nur lokal)
-dialog.assistant.store.menu.clear_files = Dateien leeren (nur lokal)
-dialog.assistant.store.menu.truncate_store = Speicher leeren (lokal + remote)
-dialog.assistant.store.menu.truncate_files = Dateien leeren (lokal + remote)
+dialog.assistant.store.menu.all = Alle Speicher...
+dialog.assistant.store.menu.current = Aktueller Speicher...
+dialog.assistant.store.menu.all.import_all = Alles importieren (alle, Speicher + Dateien)
+dialog.assistant.store.menu.all.import_files = Nur Dateien importieren (alle)
+dialog.assistant.store.menu.all.refresh_store = Alle Status aktualisieren
+dialog.assistant.store.menu.all.clear_store = Vektor-Speicher leeren (alle, nur lokal)
+dialog.assistant.store.menu.all.clear_files = Dateien löschen (alle, nur lokal)
+dialog.assistant.store.menu.all.truncate_store = Vektor-Speicher kürzen (alle, lokal + fern)
+dialog.assistant.store.menu.all.truncate_files = Dateien kürzen (alle, lokal + fern)
+dialog.assistant.store.menu.current.refresh_store = Status aktualisieren
+dialog.assistant.store.menu.current.import_files = Dateien importieren
+dialog.assistant.store.menu.current.clear_files = Dateien löschen (nur lokal)
+dialog.assistant.store.menu.current.delete = Speicher löschen (+ Dateien, lokal + fern)
+dialog.assistant.store.menu.current.truncate_files = Dateien kürzen (lokal + fern)
 dialog.changelog.title = Änderungsprotokoll
 dialog.confirm.no = Nein
 dialog.confirm.title = Bestätigung
 dialog.confirm.yes = Ja
 dialog.create.dismiss = Abbrechen
 dialog.create.title = Name
 dialog.create.update = Erstellen
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 attachments.header.path = Path
 attachments.header.size = Size
 attachments.header.store = Vector Store(s)
 attachments.send_clear = Clear list after send
 attachments.tab = Attachments
 attachments_uploaded.btn.clear = Clear files
 attachments_uploaded.btn.sync = Sync
+attachments_uploaded.btn.sync.current = Current only
+attachments_uploaded.btn.sync.all = All stores
 attachments_uploaded.clear.confirm = WARNING: are you sure to delete all this files from remote server?
 attachments_uploaded.delete.confirm = WARNING: are you sure to delete file from remote server?
 attachments_uploaded.sync.tip = Tip: click on 'Sync' to retrieve files list from OpenAI
 attachments_uploaded.tab = Uploaded files
 audio.magic_word.detected = Magic word detected!
 audio.magic_word.invalid = Not a magic word :(
 audio.magic_word.please = Magic word please...
@@ -148,22 +150,24 @@
 chat.name.bot = AI
 clipboard.copied = Copied to clipboard.
 clipboard.copied_to = Copied to clipboard:
 cmd.enabled = Execute commands
 cmd.tip = Tip: To enable the execution of commands from plugins that are prefixed with "Command:", you must enable the "Execute commands" option.
 coming_soon = Coming soon...
 confirm.assistant.delete = Delete assistant?
+confirm.assistant.files.clear = Clear files (local only)?
 confirm.assistant.files.truncate = Are you sure to remove all files from all Assistants?
+confirm.assistant.files.truncate.store = Are you sure to remove all files from selected store?
 confirm.assistant.import = Import all assistants from API?
 confirm.assistant.import_files = Import all files from API?
-confirm.assistant.store.import = Import all vector stores from API?
-confirm.assistant.store.truncate = Delete all vector stores in API?
+confirm.assistant.import_files.store = Import current store files from API?
 confirm.assistant.store.clear = Clear vector stores (local only)?
-confirm.assistant.files.clear = Clear files (local only)?
+confirm.assistant.store.import = Import all vector stores from API?
 confirm.assistant.store.refresh = Refresh all stores?
+confirm.assistant.store.truncate = Delete all vector stores in API?
 confirm.ctx.delete = Delete group?
 confirm.ctx.delete.all = Delete group and all items?
 confirm.img.delete = Delete file from disk?
 confirm.preset.clear = Are you sure to clear preset?
 confirm.preset.delete = Are you sure to delete this preset?
 confirm.preset.overwrite = Preset exists. Overwrite?
 confirm.preset.restore = Restore default preset for this mode?
@@ -216,27 +220,37 @@
 dialog.about.website = Official website
 dialog.assistant = Create / Edit assistant
 dialog.assistant.btn.current = Use current
 dialog.assistant.btn.close = Cancel
 dialog.assistant.btn.save = Save
 dialog.assistant.btn.store = Vector Stores
 dialog.assistant.store = Assistants Vector Stores
+dialog.assistant.store.alert.select = Please select vector store first.
+dialog.assistant.store.alert.assign = Please assign vector store for Assistant first.
 dialog.assistant.store.btn.close = Cancel
 dialog.assistant.store.btn.new = Create
 dialog.assistant.store.btn.save = Save
 dialog.assistant.store.btn.refresh_status = Refresh status
 dialog.assistant.store.btn.upload.files = + Files
 dialog.assistant.store.btn.upload.dir = + Directory
 dialog.assistant.store.delete.confirm = Are you sure to delete Assistants Vector Store?
-dialog.assistant.store.menu.import = Import all
-dialog.assistant.store.menu.refresh_store = Refresh all
-dialog.assistant.store.menu.clear_store = Clear vector stores (local only)
-dialog.assistant.store.menu.clear_files = Clear files (local only)
-dialog.assistant.store.menu.truncate_store = Truncate vector stores (local + remote)
-dialog.assistant.store.menu.truncate_files = Truncate files (local + remote)
+dialog.assistant.store.menu.all = All stores...
+dialog.assistant.store.menu.current = Current store...
+dialog.assistant.store.menu.all.import_all = Import everything (all, stores + files)
+dialog.assistant.store.menu.all.import_files = Import files only (all)
+dialog.assistant.store.menu.all.refresh_store = Refresh all statuses
+dialog.assistant.store.menu.all.clear_store = Clear vector stores (all, local only)
+dialog.assistant.store.menu.all.clear_files = Clear files (all, local only)
+dialog.assistant.store.menu.all.truncate_store = Truncate vector stores (all, local + remote)
+dialog.assistant.store.menu.all.truncate_files = Truncate files (all, local + remote)
+dialog.assistant.store.menu.current.refresh_store = Refresh status
+dialog.assistant.store.menu.current.import_files = Import files
+dialog.assistant.store.menu.current.clear_files = Clear files (local only)
+dialog.assistant.store.menu.current.delete = Delete store (+ files, local + remote)
+dialog.assistant.store.menu.current.truncate_files = Truncate files (local + remote)
 dialog.changelog.title = Changelog
 dialog.confirm.no = No
 dialog.confirm.title = Confirmation
 dialog.confirm.yes = Yes
 dialog.create.dismiss = Cancel
 dialog.create.title = Name
 dialog.create.update = Create
@@ -528,15 +542,15 @@
 menu.debug.presets = Presets...
 menu.debug.ui = UI...
 menu.file = File
 menu.file_clear_history = Clear history
 menu.file_clear_history_groups = Clear history (+ groups)
 menu.file.current = Select current
 menu.file.exit = Exit
-menu.file.group.new = New context group...
+menu.file.group.new = New group...
 menu.file.new = New context...
 menu.info = About
 menu.info.about = About
 menu.info.changelog = Changelog
 menu.info.docs = Documentation
 menu.info.donate = Support and donate
 menu.info.github = GitHub (source code)
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.es.ini`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Nombre
 attachments.header.path = Ruta
 attachments.header.size = Tamaño
 attachments.send_clear = Limpiar lista después de enviar
 attachments.tab = Adjuntos
 attachments_uploaded.btn.clear = Limpiar archivos
 attachments_uploaded.btn.sync = Sincronizar
+attachments_uploaded.btn.sync.current = Solo actual
+attachments_uploaded.btn.sync.all = Todas las bases
 attachments_uploaded.clear.confirm = ADVERTENCIA: ¿Está seguro de querer eliminar todos estos archivos del servidor remoto?
 attachments_uploaded.delete.confirm = ADVERTENCIA: ¿Está seguro de querer eliminar archivo del servidor remoto?
 attachments_uploaded.sync.tip = Consejo: clic en 'Sincronizar' para obtener la lista de archivos de OpenAI
 attachments_uploaded.tab = Archivos subidos
 audio.magic_word.detected = ¡Palabra mágica detectada!
 audio.magic_word.invalid = No es una palabra mágica :(
 audio.magic_word.please = Por favor, una palabra mágica...
@@ -139,22 +141,24 @@
 chat.name.bot = IA
 clipboard.copied = Copiado al portapapeles.
 clipboard.copied_to = Copiado al portapapeles:
 cmd.enabled = Ejecutar comandos
 cmd.tip = Consejo: Para habilitar la ejecución de comandos de los plugins que están prefijados con "Command:", debes activar la opción "Ejecutar comandos".
 coming_soon = Próximamente...
 confirm.assistant.delete = ¿Eliminar asistente?
+confirm.assistant.files.clear = ¿Limpiar archivos (solo local)?
+confirm.assistant.files.truncate = ¿Está seguro de eliminar todos los archivos de todas las bases?
+confirm.assistant.files.truncate.store = ¿Está seguro de eliminar todos los archivos de la base seleccionada?
 confirm.assistant.import = ¿Importar todos los asistentes desde la API?
-confirm.assistant.files.truncate = ¿Está seguro de quitar todos los archivos de todos los Asistentes?
 confirm.assistant.import_files = ¿Importar todos los archivos desde la API?
-confirm.assistant.store.import = ¿Importar todos los almacenes de vectores desde la API?
-confirm.assistant.store.truncate = ¿Eliminar todos los almacenes de vectores en la API?
-confirm.assistant.store.clear = Limpiar almacenes de vectores (solo local)?
-confirm.assistant.files.clear = Limpiar archivos (solo local)?
-confirm.assistant.store.refresh = Actualizar todos los almacenes de vectores?
+confirm.assistant.import_files.store = ¿Importar los archivos de la base actual desde la API?
+confirm.assistant.store.clear = ¿Limpiar bases vectoriales (solo local)?
+confirm.assistant.store.import = ¿Importar todas las bases vectoriales desde la API?
+confirm.assistant.store.refresh = ¿Actualizar todas las bases?
+confirm.assistant.store.truncate = ¿Eliminar todas las bases vectoriales en la API?
 confirm.img.delete = ¿Eliminar archivo del disco?
 confirm.preset.clear = ¿Está seguro de querer limpiar el ajuste preestablecido?
 confirm.preset.delete = ¿Está seguro de querer eliminar este ajuste preestablecido?
 confirm.preset.overwrite = El ajuste preestablecido existe. ¿Sobrescribir?
 confirm.preset.restore = ¿Restaurar el preset predeterminado para este modo?
 confirm.profile.delete = ¿Estás seguro de querer eliminar el perfil? Se eliminará solo de la lista.
 confirm.profile.delete_all = ¿Estás seguro de querer eliminar el perfil junto con todos los archivos de configuración y datos de usuario en el directorio de trabajo del perfil?
@@ -205,27 +209,37 @@
 dialog.about.website = Sitio web oficial
 dialog.assistant = Crear / Editar asistente
 dialog.assistant.btn.current = Usar actual
 dialog.assistant.btn.close = Cancelar
 dialog.assistant.btn.save = Guardar
 dialog.assistant.btn.store = Almacenes de vectores
 dialog.assistant.store = Almacenes de vectores de Asistentes
+dialog.assistant.store.alert.select = Por favor, seleccione primero la base vectorial.
+dialog.assistant.store.alert.assign = Por favor, asigne primero la base vectorial al Asistente.
 dialog.assistant.store.btn.close = Cancelar
 dialog.assistant.store.btn.new = Crear
 dialog.assistant.store.btn.save = Guardar
 dialog.assistant.store.btn.refresh_status = Actualizar estado
 dialog.assistant.store.btn.upload.files = + Archivos
 dialog.assistant.store.btn.upload.dir = + Directorio
 dialog.assistant.store.delete.confirm = ¿Está seguro de querer eliminar el Almacén de vectores de Asistentes?
-dialog.assistant.store.menu.import = Importar todo
-dialog.assistant.store.menu.refresh_store = Actualizar todo
-dialog.assistant.store.menu.clear_store = Limpiar almacenes de vectores (solo local)
-dialog.assistant.store.menu.clear_files = Limpiar archivos (solo local)
-dialog.assistant.store.menu.truncate_store = Vaciar almacenes (local + remoto)
-dialog.assistant.store.menu.truncate_files = Vaciar archivos (local + remoto)
+dialog.assistant.store.menu.all = Todas las bases...
+dialog.assistant.store.menu.current = Base actual...
+dialog.assistant.store.menu.all.import_all = Importar todo (todas, bases + archivos)
+dialog.assistant.store.menu.all.import_files = Importar solo archivos (todas)
+dialog.assistant.store.menu.all.refresh_store = Actualizar todos los estados
+dialog.assistant.store.menu.all.clear_store = Limpiar bases vectoriales (todas, solo local)
+dialog.assistant.store.menu.all.clear_files = Limpiar archivos (todas, solo local)
+dialog.assistant.store.menu.all.truncate_store = Vaciar bases vectoriales (todas, local + remoto)
+dialog.assistant.store.menu.all.truncate_files = Vaciar archivos (todas, local + remoto)
+dialog.assistant.store.menu.current.refresh_store = Actualizar estado
+dialog.assistant.menu.current.import_files = Importar archivos
+dialog.assistant.store.menu.current.clear_files = Limpiar archivos (solo local)
+dialog.assistant.store.menu.current.delete = Eliminar base (+ archivos, local + remoto)
+dialog.assistant.store.menu.current.truncate_files = Vaciar archivos (local + remoto)
 dialog.changelog.title = Registro de cambios
 dialog.confirm.no = No
 dialog.confirm.title = Confirmación
 dialog.confirm.yes = Sí
 dialog.create.dismiss = Cancelar
 dialog.create.title = Nombre
 dialog.create.update = Crear
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Nom
 attachments.header.path = Chemin
 attachments.header.size = Taille
 attachments.send_clear = Effacer la liste après envoi
 attachments.tab = Pièces jointes
 attachments_uploaded.btn.clear = Effacer les fichiers
 attachments_uploaded.btn.sync = Synchroniser
+attachments_uploaded.btn.sync.current = Uniquement le courant
+attachments_uploaded.btn.sync.all = Toutes les bases
 attachments_uploaded.clear.confirm = ATTENTION : êtes-vous sûr de vouloir supprimer tous ces fichiers du serveur distant ?
 attachments_uploaded.delete.confirm = ATTENTION : êtes-vous sûr de vouloir supprimer le fichier du serveur distant ?
 attachments_uploaded.sync.tip = Astuce : cliquez sur 'Synchroniser' pour récupérer la liste des fichiers depuis OpenAI
 attachments_uploaded.tab = Fichiers téléchargés
 audio.magic_word.detected = Mot magique détecté !
 audio.magic_word.invalid = Pas un mot magique :(
 audio.magic_word.please = S'il vous plaît, le mot magique...
@@ -139,22 +141,24 @@
 chat.name.bot = IA
 clipboard.copied = Copié dans le presse-papiers.
 clipboard.copied_to = Copié dans le presse-papiers:
 cmd.enabled = Exécuter des commandes
 cmd.tip = Astuce : Pour activer l'exécution des commandes provenant des plugins préfixés par "Command:", vous devez activer l'option "Exécuter des commandes".
 coming_soon = À venir...
 confirm.assistant.delete = Supprimer l'assistant ?
-confirm.assistant.import = Importer tous les assistants depuis l'API ?
-confirm.assistant.files.truncate = Êtes-vous sûr de vouloir supprimer tous les fichiers de tous les Assistants?
-confirm.assistant.import_files = Importer tous les fichiers depuis l'API?
-confirm.assistant.store.import = Importer toutes les bases vectorielles depuis l'API?
-confirm.assistant.store.truncate = Supprimer toutes les bases vectorielles dans l'API?
-confirm.assistant.store.clear = Effacer les bases vectorielles (local uniquement)?
-confirm.assistant.files.clear = Effacer les fichiers (local uniquement)?
-confirm.assistant.store.refresh = Actualiser toutes les bases vectorielles?
+confirm.assistant.files.clear = Effacer les fichiers (seulement local) ?
+confirm.assistant.files.truncate = Êtes-vous sûr de vouloir supprimer tous les fichiers de toutes les bases ?
+confirm.assistant.files.truncate.store = Êtes-vous sûr de vouloir supprimer tous les fichiers de la base sélectionnée ?
+confirm.assistant.import = Importer tous les assistants de l'API ?
+confirm.assistant.import_files = Importer tous les fichiers de l'API ?
+confirm.assistant.import_files.store = Importer les fichiers de la base actuelle de l'API ?
+confirm.assistant.store.clear = Effacer les bases vectorielles (seulement local) ?
+confirm.assistant.store.import = Importer toutes les bases vectorielles de l'API ?
+confirm.assistant.store.refresh = Actualiser toutes les bases ?
+confirm.assistant.store.truncate = Supprimer toutes les bases vectorielles dans l'API ?
 confirm.img.delete = Supprimer le fichier du disque ?
 confirm.preset.clear = Êtes-vous sûr de vouloir effacer le préréglage ?
 confirm.preset.delete = Êtes-vous sûr de vouloir supprimer ce préréglage ?
 confirm.preset.overwrite = Le préréglage existe. Remplacer ?
 confirm.preset.restore = Restaurer le préréglage par défaut pour ce mode?
 confirm.profile.delete = Êtes-vous sûr de vouloir supprimer le profil ? Il sera retiré de la liste uniquement.
 confirm.profile.delete_all = Êtes-vous sûr de vouloir supprimer le profil avec tous les fichiers de configuration et les fichiers de données utilisateur dans le répertoire de travail du profil ?
@@ -205,27 +209,37 @@
 dialog.about.website = Site officiel
 dialog.assistant = Créer / Éditer un assistant
 dialog.assistant.btn.current = Utiliser l'actuel
 dialog.assistant.btn.close = Annuler
 dialog.assistant.btn.save = Sauvegarder
 dialog.assistant.btn.store = Bases vectorielles
 dialog.assistant.store = Bases vectorielles des Assistants
+dialog.assistant.store.alert.select = Veuillez d'abord sélectionner une base vectorielle.
+dialog.assistant.store.alert.assign = Veuillez d'abord attribuer une base vectorielle à l'Assistant.
 dialog.assistant.store.btn.close = Annuler
 dialog.assistant.store.btn.new = Créer
 dialog.assistant.store.btn.save = Sauvegarder
 dialog.assistant.store.btn.refresh_status = Actualiser le statut
 dialog.assistant.store.btn.upload.files = + Fichiers
 dialog.assistant.store.btn.upload.dir = + Dossier
 dialog.assistant.store.delete.confirm = Êtes-vous sûr de vouloir supprimer la Base vectorielle des Assistants?
-dialog.assistant.store.menu.import = Importer tout
-dialog.assistant.store.menu.refresh_store = Actualiser tout
-dialog.assistant.store.menu.clear_store = Effacer les bases vectorielles (local uniquement)
-dialog.assistant.store.menu.clear_files = Effacer les fichiers (local uniquement)
-dialog.assistant.store.menu.truncate_store = Tronquer les bases (local + à distance)
-dialog.assistant.store.menu.truncate_files = Tronquer les fichiers (local + à distance)
+dialog.assistant.store.menu.all = Toutes les bases...
+dialog.assistant.store.menu.current = Base actuelle...
+dialog.assistant.store.menu.all.import_all = Tout importer (tout, bases + fichiers)
+dialog.assistant.store.menu.all.import_files = Importer seulement les fichiers (tout)
+dialog.assistant.store.menu.all.refresh_store = Actualiser tous les statuts
+dialog.assistant.store.menu.all.clear_store = Effacer les bases vectorielles (tout, seulement local)
+dialog.assistant.store.menu.all.clear_files = Effacer les fichiers (tout, seulement local)
+dialog.assistant.store.menu.all.truncate_store = Tronquer les bases vectorielles (tout, local + à distance)
+dialog.assistant.store.menu.all.truncate_files = Tronquer les fichiers (tout, local + à distance)
+dialog.assistant.store.menu.current.refresh_store = Actualiser le statut
+dialog.assistant.store.menu.current.import_files = Importer les fichiers
+dialog.assistant.store.menu.current.clear_files = Effacer les fichiers (seulement local)
+dialog.assistant.store.menu.current.delete = Supprimer la base (+ fichiers, local + à distance)
+dialog.assistant.store.menu.current.truncate_files = Tronquer les fichiers (local + à distance)
 dialog.changelog.title = Historique des changements
 dialog.confirm.no = Non
 dialog.confirm.title = Confirmation
 dialog.confirm.yes = Oui
 dialog.create.dismiss = Annuler
 dialog.create.title = Nom
 dialog.create.update = Créer
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.it.ini`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Nome
 attachments.header.path = Percorso
 attachments.header.size = Dimensione
 attachments.send_clear = Pulire l'elenco dopo l'invio
 attachments.tab = Allegati
 attachments_uploaded.btn.clear = Pulisci file
 attachments_uploaded.btn.sync = Sincronizza
+attachments_uploaded.btn.sync.current = Solo corrente
+attachments_uploaded.btn.sync.all = Tutte le basi
 attachments_uploaded.clear.confirm = ATTENZIONE: sei sicuro di voler eliminare tutti questi file dal server remoto?
 attachments_uploaded.delete.confirm = ATTENZIONE: sei sicuro di voler eliminare il file dal server remoto?
 attachments_uploaded.sync.tip = Suggerimento: clicca su 'Sincronizza' per recuperare l'elenco dei file da OpenAI
 attachments_uploaded.tab = File caricati
 audio.magic_word.detected = Parola magica rilevata!
 audio.magic_word.invalid = Non è una parola magica :(
 audio.magic_word.please = Per favore, parola magica...
@@ -139,22 +141,24 @@
 chat.name.bot = IA
 clipboard.copied = Copiato negli appunti.
 clipboard.copied_to = Copiato negli appunti:
 cmd.enabled = Esegui comandi
 cmd.tip = Suggerimento: Per abilitare l'esecuzione dei comandi dai plugin che sono prefissati con "Command:", devi attivare l'opzione "Esegui comandi".
 coming_soon = Prossimamente...
 confirm.assistant.delete = Eliminare l'assistente?
-confirm.assistant.import = Importare tutti gli assistenti dall'API?
-confirm.assistant.files.truncate = Sei sicuro di voler rimuovere tutti i file da tutti gli Assistenti?
-confirm.assistant.import_files = Importare tutti i file dall'API?
-confirm.assistant.store.import = Importare tutti gli archivi vettoriali dall'API?
-confirm.assistant.store.truncate = Eliminare tutti gli archivi vettoriali nell'API?
-confirm.assistant.store.clear = Pulire gli archivi vettoriali (solo locale)?
-confirm.assistant.files.clear = Pulire i file (solo locale)?
-confirm.assistant.store.refresh = Aggiornare tutti gli archivi vettoriali?
+confirm.assistant.files.clear = Vuoi cancellare i file (solo locale)?
+confirm.assistant.files.truncate = Sei sicuro di voler rimuovere tutti i file da tutte le basi?
+confirm.assistant.files.truncate.store = Sei sicuro di voler rimuovere tutti i file dalla base selezionata?
+confirm.assistant.import = Importare tutti gli assistenti da API?
+confirm.assistant.import_files = Importare tutti i file da API?
+confirm.assistant.import_files.store = Importare i file della base corrente da API?
+confirm.assistant.store.clear = Vuoi cancellare le basi vettoriali (solo locale)?
+confirm.assistant.store.import = Importare tutte le basi vettoriali da API?
+confirm.assistant.store.refresh = Aggiornare tutte le basi?
+confirm.assistant.store.truncate = Cancellare tutte le basi vettoriali in API?
 confirm.img.delete = Eliminare il file dal disco?
 confirm.preset.clear = Sei sicuro di voler cancellare il preset?
 confirm.preset.delete = Sei sicuro di voler cancellare questo preset?
 confirm.preset.overwrite = Il preset esiste. Sovrascrivere?
 confirm.preset.restore = Ripristinare il preset di default per questa modalità?
 confirm.profile.delete = Sei sicuro di voler eliminare il profilo? Sarà rimosso solo dall'elenco.
 confirm.profile.delete_all = Sei sicuro di voler eliminare il profilo insieme a tutti i file di configurazione e i file dati utente nella directory di lavoro del profilo?
@@ -205,27 +209,37 @@
 dialog.about.website = Sito ufficiale
 dialog.assistant = Crea / Modifica assistente
 dialog.assistant.btn.current = Usa attuale
 dialog.assistant.btn.close = Annulla
 dialog.assistant.btn.save = Salva
 dialog.assistant.btn.store = Archivi vettoriali
 dialog.assistant.store = Archivi vettoriali degli Assistenti
+dialog.assistant.store.alert.select = Selezionare prima una base vettoriale.
+dialog.assistant.store.alert.assign = Assegnare prima una base vettoriale all'Assistente.
 dialog.assistant.store.btn.close = Annulla
 dialog.assistant.store.btn.new = Crea
 dialog.assistant.store.btn.save = Salva
 dialog.assistant.store.btn.refresh_status = Aggiorna stato
 dialog.assistant.store.btn.upload.files = + File
 dialog.assistant.store.btn.upload.dir = + Cartella
 dialog.assistant.store.delete.confirm = Sei sicuro di voler eliminare l'Archivio vettoriale degli Assistenti?
-dialog.assistant.store.menu.import = Importa tutto
-dialog.assistant.store.menu.refresh_store = Aggiorna tutto
-dialog.assistant.store.menu.clear_store = Pulisci archivi vettoriali (solo locale)
-dialog.assistant.store.menu.clear_files = Pulisci file (solo locale)
-dialog.assistant.store.menu.truncate_store = Svuota archivi (locale + remoto)
-dialog.assistant.store.menu.truncate_files = Svuota file (locale + remoto)
+dialog.assistant.store.menu.all = Tutte le basi...
+dialog.assistant.store.menu.current = Base corrente...
+dialog.assistant.store.menu.all.import_all = Importa tutto (tutte, basi + file)
+dialog.assistant.store.menu.all.import_files = Importa solo file (tutte)
+dialog.assistant.store.menu.all.refresh_store = Aggiorna tutti gli stati
+dialog.assistant.store.menu.all.clear_store = Cancella le basi vettoriali (tutte, solo locale)
+dialog.assistant.store.menu.all.clear_files = Cancella i file (tutte, solo locale)
+dialog.assistant.store.menu.all.truncate_store = Elimina le basi vettoriali (tutte, locale + remoto)
+dialog.assistant.store.menu.all.truncate_files = Elimina i file (tutte, locale + remoto)
+dialog.assistant.store.menu.current.refresh_store = Aggiorna stato
+dialog.assistant.store.menu.current.import_files = Importa file
+dialog.assistant.store.menu.current.clear_files = Cancella i file (solo locale)
+dialog.assistant.store.menu.current.delete = Elimina base (+ file, locale + remoto)
+dialog.assistant.store.menu.current.truncate_files = Elimina i file (locale + remoto)
 dialog.changelog.title = Cronologia modifiche
 dialog.confirm.no = No
 dialog.confirm.title = Conferma
 dialog.confirm.yes = Sì
 dialog.create.dismiss = Annulla
 dialog.create.title = Nome
 dialog.create.update = Crea
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Nazwa
 attachments.header.path = Ścieżka
 attachments.header.size = Rozmiar
 attachments.send_clear = Wyczyść listę po wysłaniu
 attachments.tab = Załączniki
 attachments_uploaded.btn.clear = Wyczyść
 attachments_uploaded.btn.sync = Synchronizuj
+attachments_uploaded.btn.sync.current = Tylko bieżące
+attachments_uploaded.btn.sync.all = Wszystkie bazy
 attachments_uploaded.clear.confirm = UWAGA: Czy na pewno usunąć wszystkie te pliki ze zdalnego serwera?
 attachments_uploaded.delete.confirm = UWAGA: Czy na pewno usunąć plik ze zdalnego serwera?
 attachments_uploaded.sync.tip = Tip: kliknij na 'Synchronizuj', aby pobrać listę plików z OpenAI
 attachments_uploaded.tab = Wgrane pliki
 audio.magic_word.detected = Wykryto magiczne słowo!
 audio.magic_word.invalid = To nie magiczne słowo :(
 audio.magic_word.please = Podaj magiczne słowo...
@@ -139,22 +141,24 @@
 chat.name.bot = AI
 clipboard.copied = Skopiowano do schowka.
 clipboard.copied_to = Skopiowano do schowka:
 cmd.enabled = Uruchamianie poleceń
 cmd.tip = Tip: Aby umożliwić wykonanie poleceń z pluginów z prefixem "Command/Polecenie:", musisz włączyć opcję "Uruchamianie poleceń".
 coming_soon = Dostępne wkrótce...
 confirm.assistant.delete = Na pewno usunąć asystenta?
-confirm.assistant.import = Na pewno zaimportować listę asystentów z API?
-confirm.assistant.files.truncate = Czy na pewno chcesz usunąć wszystkie pliki we wszystkich asystentach?
+confirm.assistant.files.clear = Wyczyścić pliki (tylko lokalnie)?
+confirm.assistant.files.truncate = Czy na pewno usunąć wszystkie pliki ze wszystkich baz?
+confirm.assistant.files.truncate.store = Czy na pewno usunąć wszystkie pliki z wybranej bazy?
+confirm.assistant.import = Zaimportować wszystkich asystentów z API?
 confirm.assistant.import_files = Zaimportować wszystkie pliki z API?
+confirm.assistant.import_files.store = Zaimportować bieżące pliki bazy z API?
+confirm.assistant.store.clear = Wyczyścić bazy wektorowe (tylko lokalnie)?
 confirm.assistant.store.import = Zaimportować wszystkie bazy wektorowe z API?
+confirm.assistant.store.refresh = Odświeżyć wszystkie bazy?
 confirm.assistant.store.truncate = Usunąć wszystkie bazy wektorowe w API?
-confirm.assistant.store.clear = Wyczyścić bazy wektorowe (tylko lokalnie)?
-confirm.assistant.files.clear = Wyczyścić pliki (tylko lokalnie)?
-confirm.assistant.store.refresh = Odświeżyć wszystkie bazy wektorowe?
 confirm.img.delete = Usunąć obraz z dysku?
 confirm.preset.clear = Na pewno wyczyścić preset?
 confirm.preset.delete = Na pewno chcesz usunąć ten preset?
 confirm.preset.overwrite = Preset już istnieje. Czy zastąpić plik?
 confirm.preset.restore = Przywrócić domyślny preset dla tego trybu?
 confirm.profile.delete = Czy na pewno chcesz usunąć profil? Zostanie on usunięty tylko z listy.
 confirm.profile.delete_all = Czy jesteś pewien, że chcesz usunąć profil wraz ze wszystkimi plikami konfiguracyjnymi i plikami danych użytkownika w katalogu roboczym profilu?
@@ -205,27 +209,37 @@
 dialog.about.website = Strona WWW
 dialog.assistant = Dodawanie / Edycja asystenta
 dialog.assistant.btn.current = Użyj obecnego
 dialog.assistant.btn.close = Anuluj
 dialog.assistant.btn.save = Zapisz
 dialog.assistant.btn.store = Bazy wektorowe
 dialog.assistant.store = Bazy wektorowe asystentów
+dialog.assistant.store.alert.select = Proszę najpierw wybrać bazę wektorową.
+dialog.assistant.store.alert.assign = Proszę najpierw przypisać bazę wektorową dla Asystenta.
 dialog.assistant.store.btn.close = Anuluj
 dialog.assistant.store.btn.new = Utwórz
 dialog.assistant.store.btn.save = Zapisz
 dialog.assistant.store.btn.refresh_status = Odśwież status
 dialog.assistant.store.btn.upload.files = + Pliki
 dialog.assistant.store.btn.upload.dir = + Katalog
 dialog.assistant.store.delete.confirm = Czy na pewno chcesz usunąć bazę wektorową asystenta?
-dialog.assistant.store.menu.import = Zaimportuj wszystko
-dialog.assistant.store.menu.refresh_store = Odśwież wszystko
-dialog.assistant.store.menu.clear_store = Wyczyść bazy wektorowe (tylko lokalnie)
-dialog.assistant.store.menu.clear_files = Wyczyść pliki (tylko lokalnie)
-dialog.assistant.store.menu.truncate_store = Opróżnij bazy (lokalnie + zdalnie)
-dialog.assistant.store.menu.truncate_files = Opróżnij pliki (lokalnie + zdalnie)
+dialog.assistant.store.menu.all = Wszystkie bazy...
+dialog.assistant.store.menu.current = Bieżąca baza...
+dialog.assistant.store.menu.all.import_all = Zaimportuj wszystko (wszystkie, bazy + pliki)
+dialog.assistant.store.menu.all.import_files = Tylko import plików (wszystkie)
+dialog.assistant.store.menu.all.refresh_store = Odśwież wszystkie statusy
+dialog.assistant.store.menu.all.clear_store = Wyczyść bazy wektorowe (wszystkie, tylko lokalne)
+dialog.assistant.store.menu.all.clear_files = Wyczyść pliki (wszystkie, tylko lokalne)
+dialog.assistant.store.menu.all.truncate_store = Opróżnij bazy wektorowe (wszystkie, lokalne + zdalne)
+dialog.assistant.store.menu.all.truncate_files = Opróżnij pliki (wszystkie, lokalne + zdalne)
+dialog.assistant.store.menu.current.refresh_store = Odśwież status
+dialog.assistant.store.menu.current.import_files = Import plików
+dialog.assistant.store.menu.current.clear_files = Wyczyść pliki (tylko lokalnie)
+dialog.assistant.store.menu.current.delete = Usuń bazę (+ pliki, lokalne + zdalne)
+dialog.assistant.store.menu.current.truncate_files = Opróżnij pliki (lokalne + zdalne)
 dialog.changelog.title = Dziennik zmian
 dialog.confirm.no = Nie
 dialog.confirm.title = Potwierdź
 dialog.confirm.yes = Tak
 dialog.create.dismiss = Anuluj
 dialog.create.title = Nazwa
 dialog.create.update = Utwórz
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 attachments.header.name = Ім'я
 attachments.header.path = Шлях
 attachments.header.size = Розмір
 attachments.send_clear = Очистити список після відправлення
 attachments.tab = Вкладення
 attachments_uploaded.btn.clear = Очистити файли
 attachments_uploaded.btn.sync = Синхронізація
+attachments_uploaded.btn.sync.current = Лише поточний
+attachments_uploaded.btn.sync.all = Усі бази
 attachments_uploaded.clear.confirm = ПОПЕРЕДЖЕННЯ: ви впевнені, що хочете видалити всі ці файли з віддаленого сервера?
 attachments_uploaded.delete.confirm = ПОПЕРЕДЖЕННЯ: ви впевнені, що хочете видалити файл з віддаленого сервера?
 attachments_uploaded.sync.tip = Підказка: натисніть "Синхронізація", щоб отримати список файлів з OpenAI
 attachments_uploaded.tab = Завантажені файли
 audio.magic_word.detected = Магічне слово виявлено!
 audio.magic_word.invalid = Не магічне слово :(
 audio.magic_word.please = Магічне слово, будь ласка...
@@ -139,22 +141,24 @@
 chat.name.bot = ШІ
 clipboard.copied = Скопійовано до буфера обміну.
 clipboard.copied_to = Скопійовано до буфера обміну:
 cmd.enabled = Виконувати команди
 cmd.tip = Порада: Щоб дозволити виконання команд з плагінів, які починаються з "Command:", ви повинні увімкнути опцію "Виконувати команди".
 coming_soon = Незабаром...
 confirm.assistant.delete = Видалити помічника?
-confirm.assistant.import = Імпортувати всіх помічників з API?
-confirm.assistant.files.truncate = Ви впевнені, що хочете видалити всі файли з усіх помічників?
+confirm.assistant.files.clear = Очистити файли (лише локально)?
+confirm.assistant.files.truncate = Ви впевнені, що хочете видалити усі файли з усіх баз?
+confirm.assistant.files.truncate.store = Ви впевнені, що хочете видалити усі файли з обраної бази?
+confirm.assistant.import = Імпортувати всіх асистентів з API?
 confirm.assistant.import_files = Імпортувати всі файли з API?
-confirm.assistant.store.import = Імпортувати всі векторні сховища з API?
-confirm.assistant.store.truncate = Видалити всі векторні сховища в API?
-confirm.assistant.store.clear = Очистити векторні сховища (тільки локально)?
-confirm.assistant.files.clear = Очистити файли (тільки локально)?
-confirm.assistant.store.refresh = Оновити всі векторні сховища?
+confirm.assistant.import_files.store = Імпортувати файли поточної бази з API?
+confirm.assistant.store.clear = Очистити векторні бази (лише локально)?
+confirm.assistant.store.import = Імпортувати всі векторні бази з API?
+confirm.assistant.store.refresh = Оновити всі бази?
+confirm.assistant.store.truncate = Видалити всі векторні бази в API?
 confirm.img.delete = Видалити файл з диска?
 confirm.preset.clear = Ви впевнені, що хочете очистити пресет?
 confirm.preset.delete = Ви впевнені, що хочете видалити цей пресет?
 confirm.preset.overwrite = Пресет існує. Перезаписати?
 confirm.preset.restore = Відновити стандартний пресет для цього режиму?
 confirm.profile.delete = Ви впевнені, що хочете видалити профіль? Він буде видалений лише зі списку.
 confirm.profile.delete_all = Ви впевнені, що хочете видалити профіль разом зі всіма конфігураційними файлами та файлами даних користувача у робочій директорії профілю?
@@ -205,27 +209,37 @@
 dialog.about.website = Офіційний сайт
 dialog.assistant = Створити / Редагувати помічника
 dialog.assistant.btn.current = Використовувати поточний
 dialog.assistant.btn.close = Скасувати
 dialog.assistant.btn.save = Зберегти
 dialog.assistant.btn.store = Векторні сховища
 dialog.assistant.store = Векторні сховища помічників
+dialog.assistant.store.alert.select = Будь ласка, спочатку виберіть векторну базу.
+dialog.assistant.store.alert.assign = Будь ласка, спочатку призначте векторну базу Асистенту.
 dialog.assistant.store.btn.close = Скасувати
 dialog.assistant.store.btn.new = Створити
 dialog.assistant.store.btn.save = Зберегти
 dialog.assistant.store.btn.refresh_status = Оновити статус
 dialog.assistant.store.btn.upload.files = + Файли
 dialog.assistant.store.btn.upload.dir = + Каталог
 dialog.assistant.store.delete.confirm = Ви впевнені, що хочете видалити векторне сховище помічника?
-dialog.assistant.store.menu.import = Імпортувати все
-dialog.assistant.store.menu.refresh_store = Оновити все
-dialog.assistant.store.menu.clear_store = Очистити векторні сховища (тільки локально)
-dialog.assistant.store.menu.clear_files = Очистити файли (тільки локально)
-dialog.assistant.store.menu.truncate_store = Очистити сховища (локально + віддалено)
-dialog.assistant.store.menu.truncate_files = Очистити файли (локально + віддалено)
+dialog.assistant.store.menu.all = Всі бази...
+dialog.assistant.store.menu.current = Поточна база...
+dialog.assistant.store.menu.all.import_all = Імпортувати все (всі, бази + файли)
+dialog.assistant.store.menu.all.import_files = Імпортувати лише файли (всі)
+dialog.assistant.store.menu.all.refresh_store = Оновити всі статуси
+dialog.assistant.store.menu.all.clear_store = Очистити векторні бази (всі, лише локально)
+dialog.assistant.store.menu.all.clear_files = Очистити файли (всі, лише локально)
+dialog.assistant.store.menu.all.truncate_store = Очистити векторні бази повністю (всі, локально + віддалено)
+dialog.assistant.store.menu.all.truncate_files = Очистити файли повністю (всі, локально + віддалено)
+dialog.assistant.store.menu.current.refresh_store = Оновити статус
+dialog.assistant.store.menu.current.import_files = Імпортувати файли
+dialog.assistant.store.menu.current.clear_files = Очистити файли (лише локально)
+dialog.assistant.store.menu.current.delete = Видалити базу (+ файли, локально + віддалено)
+dialog.assistant.store.menu.current.truncate_files = Очистити файли повністю (локально + віддалено)
 dialog.changelog.title = Список змін
 dialog.confirm.no = Ні
 dialog.confirm.title = Підтвердження
 dialog.confirm.yes = Так
 dialog.create.dismiss = Скасувати
 dialog.create.title = Назва
 dialog.create.update = Створити
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 action.profile.delete_all = 删除个人资料（及所有用户文件）
 action.unpin = 取消置頂
 action.refresh = 刷新
 action.rename = 重命名
 action.reset = 重置
 action.restore = 恢復
 action.redo = 重做
-action.restore = 恢复
 action.save = 保存
 action.save_as = 另存為...
 action.save_selection_as = 将选择保存为...
 action.select_all = 选择全部
 action.touch = 創建文件...
 action.truncate = 截斷
 action.undo = 撤銷
@@ -92,14 +91,16 @@
 attachments.header.name = 名稱
 attachments.header.path = 路徑
 attachments.header.size = 尺寸
 attachments.send_clear = 發送後清除列表
 attachments.tab = 附件
 attachments_uploaded.btn.clear = 清除文件
 attachments_uploaded.btn.sync = 同步
+attachments_uploaded.btn.sync.current = 仅当前
+attachments_uploaded.btn.sync.all = 所有存储
 attachments_uploaded.clear.confirm = 警告：您確定要從遠程服務器刪除所有這些文件嗎？
 attachments_uploaded.delete.confirm = 警告：您確定要從遠程服務器刪除文件嗎？
 attachments_uploaded.sync.tip = 提示：點擊“同步”以從OpenAI檢索文件列表。
 attachments_uploaded.tab = 已上傳的文件
 audio.magic_word.detected = 檢測到魔法詞！
 audio.magic_word.invalid= 不是魔法詞 :(
 audio.magic_word.please= 請說出魔法詞...
@@ -140,23 +141,24 @@
 chat.name.user = 您
 chat.name.bot = AI
 clipboard.copied = 已複製到剪貼板。
 clipboard.copied_to = 已複製到剪貼板：
 cmd.enabled = 執行命令
 cmd.tip = 提示：要啟用從插件執行的以“命令：”為前綴的命令，您必須啟用“執行命令”選項。
 coming_soon = 即將推出...
-confirm.assistant.delete = 刪除助手？
-confirm.assistant.import = 從API導入所有助手？
-confirm.assistant.files.truncate = 确定要从所有助手中删除所有文件吗？
-confirm.assistant.import_files = 从API导入所有文件？
-confirm.assistant.store.import = 从API导入所有向量存储库？
-confirm.assistant.store.truncate = 删除API中的所有向量存储库？
-confirm.assistant.store.clear = 清除向量存储库（仅限本地）？
-confirm.assistant.files.clear = 清除文件（仅限本地）？
-confirm.assistant.store.refresh = 刷新所有向量存储库？
+confirm.assistant.files.clear = 清除文件（仅本地）？
+confirm.assistant.files.truncate = 确定要从所有存储中移除所有文件吗？
+confirm.assistant.files.truncate.store = 确定要从所选存储中移除所有文件吗？
+confirm.assistant.import = 从 API 导入所有助手？
+confirm.assistant.import_files = 从 API 导入所有文件？
+confirm.assistant.import_files.store = 从 API 导入当前存储的文件？
+confirm.assistant.store.clear = 清空矢量存储（仅本地）？
+confirm.assistant.store.import = 从 API 导入所有矢量存储？
+confirm.assistant.store.refresh = 刷新所有存储？
+confirm.assistant.store.truncate = 删除 API 中的所有矢量存储？
 confirm.img.delete = 從磁盤刪除文件？
 confirm.preset.clear = 您確定要清除預設嗎？
 confirm.preset.delete = 您確定要刪除此預設嗎？
 confirm.preset.overwrite = 預設已存在。覆蓋？
 confirm.preset.restore = 恢復此模式的默認預設？
 confirm.profile.delete = 您确定要删除个人资料吗？ 仅将从列表中移除。
 confirm.profile.delete_all = 您确定要删除个人资料及其工作目录中的所有配置文件和用户数据文件吗？
@@ -207,27 +209,37 @@
 dialog.about.website = 官方網站
 dialog.assistant = 創建/編輯助手
 dialog.assistant.btn.current = 使用當前的
 dialog.assistant.btn.close = 取消
 dialog.assistant.btn.save = 保存
 dialog.assistant.btn.store = 向量存储库
 dialog.assistant.store = 助手的向量存储库
+dialog.assistant.store.alert.select = 请先选择矢量存储。
+dialog.assistant.store.alert.assign = 请先为助手分配矢量存储。
 dialog.assistant.store.btn.close = 取消
 dialog.assistant.store.btn.new = 创建
 dialog.assistant.store.btn.save = 保存
 dialog.assistant.store.btn.refresh_status = 刷新状态
 dialog.assistant.store.btn.upload.files = + 文件
 dialog.assistant.store.btn.upload.dir = + 目录
 dialog.assistant.store.delete.confirm = 确定要删除助手的向量存储库吗？
-dialog.assistant.store.menu.import = 导入所有
-dialog.assistant.store.menu.refresh_store = 刷新全部
-dialog.assistant.store.menu.clear_store = 清除向量存储库（仅限本地）
-dialog.assistant.store.menu.clear_files = 清除文件（仅限本地）
-dialog.assistant.store.menu.truncate_store = 清空存储库（本地+远程）
-dialog.assistant.store.menu.truncate_files = 清空文件（本地+远程）
+dialog.assistant.store.menu.all = 所有存储...
+dialog.assistant.store.menu.current = 当前存储...
+dialog.assistant.store.menu.all.import_all = 导入所有内容（所有存储+文件）
+dialog.assistant.store.menu.all.import_files = 只导入文件（全部）
+dialog.assistant.store.menu.all.refresh_store = 刷新所有状态
+dialog.assistant.store.menu.all.clear_store = 清除矢量存储（所有，仅本地）
+dialog.assistant.store.menu.all.clear_files = 清除文件（所有，仅本地）
+dialog.assistant.store.menu.all.truncate_store = 清空矢量存储（所有，本地+远程）
+dialog.assistant.store.menu.all.truncate_files = 清空文件（所有，本地+远程）
+dialog.assistant.store.menu.current.refresh_store = 刷新状态
+dialog.assistant.store.menu.current.import_files = 导入文件
+dialog.assistant.store.menu.current.clear_files = 清除文件（仅本地）
+dialog.assistant.store.menu.current.delete = 删除存储（+文件，本地+远程）
+dialog.assistant.store.menu.current.truncate_files = 清空文件（本地+远程）
 dialog.changelog.title = 更新日誌
 dialog.confirm.no = 否
 dialog.confirm.title = 確認
 dialog.confirm.yes = 是的
 dialog.create.dismiss = 取消
 dialog.create.title = 名稱
 dialog.create.update = 創建
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.4/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.4/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.4/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.4/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.4/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.4/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.4/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.4/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.4/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.4/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.4/src/pygpt_net/item/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/index.py` & `pygpt_net-2.2.4/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.4/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/model.py` & `pygpt_net-2.2.4/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.4/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.4/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/launcher.py` & `pygpt_net-2.2.4/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.4/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import uuid
 
 from packaging.version import Version
 
 from pygpt_net.item.assistant import AssistantFileItem
@@ -176,16 +176,25 @@
 
         :param record_id: record ID
         :param name: new name
         :return: True if renamed
         """
         return self.storage.rename_file(record_id, name)
 
-    def truncate(self) -> bool:
+    def truncate_all(self) -> bool:
         """
         Truncate all files
 
         :return: True if truncated
         """
         return self.storage.truncate_all()
 
+    def truncate_by_store(self, store_id: str) -> bool:
+        """
+        Truncate all files
+
+        :param store_id: store ID
+        :return: True if truncated
+        """
+        return self.storage.truncate_by_store(store_id)
+
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import time
 
 from sqlalchemy import text
 
 from pygpt_net.item.assistant import AssistantFileItem
@@ -173,14 +173,29 @@
         """
         db = self.window.core.db.get_db()
         with db.begin() as conn:
             conn.execute(text("DELETE FROM remote_file"))
             conn.execute(text("DELETE FROM sqlite_sequence WHERE name='remote_file'"))
         return True
 
+    def truncate_by_store(self, store_id: str) -> bool:
+        """
+        Truncate all files items by store ID
+
+        :param store_id: store ID
+        :return: True if truncated
+        """
+        stmt = text("""
+            DELETE FROM remote_file WHERE store_id = :store_id
+        """).bindparams(store_id=store_id)
+        db = self.window.core.db.get_db()
+        with db.begin() as conn:
+            conn.execute(stmt)
+            return True
+
     def delete_by_id(self, id: int) -> bool:
         """
         Delete file item by record ID
 
         :param id: record ID
         :return: True if deleted
         """
@@ -211,29 +226,29 @@
         """
         Clear store from files
 
         :param store_id: store ID
         :return: True if cleared
         """
         stmt = text("""
-            UPDATE remote_file SET store_id = NULL WHERE store_id = :store_id
+            DELETE FROM remote_file WHERE store_id = :store_id
         """).bindparams(store_id=store_id)
         db = self.window.core.db.get_db()
         with db.begin() as conn:
             conn.execute(stmt)
             return True
 
     def clear_all_stores_from_files(self) -> bool:
         """
         Clear all stores from files
 
         :return: True if cleared
         """
         stmt = text("""
-            UPDATE remote_file SET store_id = NULL
+            DELETE FROM remote_file WHERE store_id IS NOT NULL
         """)
         db = self.window.core.db.get_db()
         with db.begin() as conn:
             conn.execute(stmt)
             return True
 
     def rename_file(self, record_id: int, name: str) -> bool:
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/assistants.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import json
 import os
 
 from pygpt_net.item.assistant import AssistantItem, AssistantStoreItem
 from pygpt_net.item.ctx import CtxItem
@@ -453,16 +453,37 @@
 
         :return: number of deleted files
         """
         i = 0
         files = self.files_get_ids()
         for file_id in files:
             print("Removing file: " + file_id)
-            self.file_delete(file_id)
-            i += 1
+            try:
+                self.file_delete(file_id)
+                i += 1
+            except Exception as e:
+                print("Error removing file {}: {}".format(file_id, str(e)))
+        return i
+
+    def files_truncate_store(self, store_id: str) -> int:
+        """
+        Truncate all files from store
+
+        :param store_id: store ID
+        :return: number of deleted files
+        """
+        i = 0
+        files = self.vs_get_store_files_list(store_id, [])
+        for file_id in files:
+            print("Removing file: " + file_id)
+            try:
+                self.file_delete(file_id)
+                i += 1
+            except Exception as e:
+                print("Error removing file {}: {}".format(file_id, str(e)))
         return i
 
     def import_assistants(
             self,
             items: dict,
             order: str = "asc",
             limit: int = 100,
@@ -564,14 +585,15 @@
                     items[id].is_thread = True  # tmp store for thread
                     tmp_name = ""
                 items[id].id = id
                 items[id].name = tmp_name
                 items[id].file_ids = []
                 items[id].status = self.window.core.assistants.store.parse_status(remote)
                 self.window.core.assistants.store.append_status(items[id], items[id].status)
+                print("Imported vector store: " + id)
             # next page
             if stores.has_more:
                 return self.import_vector_stores(items, order, limit, stores.last_id)
         return items
 
     def get_tools(self, assistant: AssistantItem) -> list:
         """
@@ -777,26 +799,44 @@
             files = self.vs_get_all_files_ids(store_id, [])
             for file_id in files:
                 print("Removing file from vector store [{}]:{} ".format(store_id, file_id))
                 self.vs_delete_file(store_id, file_id)
                 i += 1
         return i
 
+    def vs_remove_files_from_store(self, store_id: str) -> int:
+        """
+        Remove all files from vector store
+
+        :param store_id: store ID
+        :return: number of deleted files
+        """
+        files = self.vs_get_all_files_ids(store_id, [])
+        i = 0
+        for file_id in files:
+            print("Removing file from vector store [{}]:{} ".format(store_id, file_id))
+            self.vs_delete_file(store_id, file_id)
+            i += 1
+        return i
+
     def vs_truncate_stores(self) -> int:
         """
         Truncate all vector stores
 
         :return: number of deleted stores
         """
         i = 0
         stores = self.vs_get_all_ids([])
         for store_id in stores:
             print("Removing vector store: " + store_id)
-            self.vs_delete(store_id)
-            i += 1
+            try:
+                self.vs_delete(store_id)
+                i += 1
+            except Exception as e:
+                print("Error removing vector store {}: {}".format(store_id, str(e)))
         return i
 
 
     def vs_add_file(self, store_id: str, file_id: str):
         """
         Add file to vector store
 
@@ -834,15 +874,18 @@
 
         :return: result
         """
         store_ids = self.vs_get_all_ids([])
         sum = 0
         for store_id in store_ids:
             items = []
-            items = self.vs_import_store_files(store_id, items)
+            try:
+                items = self.vs_import_store_files(store_id, items)
+            except Exception as e:
+                print("Error importing store {} files list: {}".format(store_id, str(e)))
             sum += len(items)
         return sum
 
     def vs_import_store_files(
             self,
             store_id: str,
             items: list,
@@ -867,18 +910,58 @@
             "limit": limit,
         }
         if after is not None:
             args['after'] = after
         files = client.beta.vector_stores.files.list(**args)
         if files is not None:
             for remote in files.data:
+                try:
+                    id = remote.id
+                    if id not in items:
+                        items.append(id)
+                        # add remote file to DB
+                        data = self.file_info(remote.id)
+                        self.window.core.assistants.files.insert(store_id, data)
+                        print("Imported file ID {} to store {}".format(remote.id, store_id))
+                except Exception as e:
+                    print("Error importing file {} to store {}: {}".format(remote.id, store_id, str(e)))
+
+            if files.has_more:
+                return self.vs_import_store_files(store_id, items, order, limit, files.last_id)
+        return items
+
+    def vs_get_store_files_list(
+            self,
+            store_id: str,
+            items: list,
+            order: str = "asc",
+            limit: int = 100,
+            after: str = None,
+    ) -> list:
+        """
+        Get all vector store files IDs
+
+        :param store_id: store ID
+        :param items: items
+        :param order: order
+        :param limit: limit
+        :param after: next page after ID
+        :return: items dict
+        """
+        client = self.window.core.gpt.get_client()
+        args = {
+            "vector_store_id": store_id,
+            "order": order,
+            "limit": limit,
+        }
+        if after is not None:
+            args['after'] = after
+        files = client.beta.vector_stores.files.list(**args)
+        if files is not None:
+            for remote in files.data:
                 id = remote.id
                 if id not in items:
                     items.append(id)
-                    # add remote file to DB
-                    data = self.file_info(remote.id)
-                    self.window.core.assistants.files.insert(store_id, data)
-                    print("Imported file ID {} to store {}".format(remote.id, store_id))
 
             if files.has_more:
-                return self.vs_import_store_files(store_id, items, order, limit, files.last_id)
+                return self.vs_get_store_files_list(store_id, items, order, limit, files.last_id)
         return items
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtCore import QObject, Signal, QRunnable, Slot
 
-from pygpt_net.item.assistant import AssistantItem
-
 
 class Importer:
     def __init__(self, window=None):
         """
         Importer core
 
         :param window: Window instance
@@ -31,41 +29,42 @@
         Handle thread error signal
 
         :param mode: mode
         :param err: error message
         """
         if mode == "assistants":
             self.window.controller.assistant.batch.handle_imported_assistants_failed(err)
-        elif mode == "files":
+        elif mode == "import_files":
             self.window.controller.assistant.batch.handle_imported_files_failed(err)
         elif mode == "truncate_files":
             self.window.controller.assistant.batch.handle_truncated_files_failed(err)
         elif mode == "upload_files":
             self.window.controller.assistant.batch.handle_uploaded_files_failed(err)
         elif mode in "vector_stores":
             self.window.controller.assistant.batch.handle_imported_stores_failed(err)
         elif mode in "truncate_vector_stores":
             self.window.controller.assistant.batch.handle_truncated_stores_failed(err)
         elif mode in "refresh_vector_stores":
             self.window.controller.assistant.batch.handle_refreshed_stores_failed(err)
 
-    @Slot(str, int)
-    def handle_finished(self, mode: str, num: int):
+    @Slot(str, str, int)
+    def handle_finished(self, mode: str, store_id: str = None, num: int = 0):
         """
         Handle thread finished signal
 
         :param mode: mode
-        :param num: number of imported items
+        :param store_id: store ID
+        :param num: number of affected items
         """
         if mode == "assistants":
             self.window.controller.assistant.batch.handle_imported_assistants(num)
-        elif mode == "files":
+        elif mode == "import_files":
             self.window.controller.assistant.batch.handle_imported_files(num)
         elif mode == "truncate_files":
-            self.window.controller.assistant.batch.handle_truncated_files(num)
+            self.window.controller.assistant.batch.handle_truncated_files(store_id, num)
         elif mode == "upload_files":
             self.window.controller.assistant.batch.handle_uploaded_files(num)
         elif mode == "vector_stores":
             self.window.controller.assistant.batch.handle_imported_stores(num)
         elif mode == "truncate_vector_stores":
             self.window.controller.assistant.batch.handle_truncated_stores(num)
         elif mode == "refresh_vector_stores":
@@ -104,29 +103,34 @@
         worker = ImportWorker()
         worker.window = self.window
         worker.mode = "truncate_vector_stores"
         worker.signals.finished.connect(self.handle_finished)
         worker.signals.error.connect(self.handle_error)
         self.window.threadpool.start(worker)
 
-    def truncate_files(self):
-        """Truncate files"""
+    def truncate_files(self, store_id: str = None):
+        """
+        Truncate files
+
+        :param store_id: store ID
+        """
         worker = ImportWorker()
         worker.window = self.window
         worker.mode = "truncate_files"
+        worker.store_id = store_id
         worker.signals.finished.connect(self.handle_finished)
         worker.signals.error.connect(self.handle_error)
         self.window.threadpool.start(worker)
 
     def upload_files(self, store_id: str, files: list = None):
         """
         Upload files
 
-        :param files: files
         :param store_id: store ID
+        :param files: files
         """
         worker = ImportWorker()
         worker.window = self.window
         worker.mode = "upload_files"
         worker.store_id = store_id
         worker.files = files
         worker.signals.finished.connect(self.handle_finished)
@@ -139,32 +143,33 @@
         worker = ImportWorker()
         worker.window = self.window
         worker.mode = "refresh_vector_stores"
         worker.signals.finished.connect(self.handle_finished)
         worker.signals.error.connect(self.handle_error)
         self.window.threadpool.start(worker)
 
-    def import_files(self, assistant: AssistantItem):
+    def import_files(self, store_id: str = None):
         """
         Import assistant files
 
-        :param assistant: assistant
+        :param store_id: store ID
         """
         worker = ImportWorker()
         worker.window = self.window
-        worker.mode = "files"
-        worker.assistant = assistant
+        worker.mode = "import_files"
+        worker.store_id = store_id
         worker.signals.finished.connect(self.handle_finished)
         worker.signals.error.connect(self.handle_error)
         self.window.threadpool.start(worker)
 
 
 class ImportWorkerSignals(QObject):
+    """Import worker signals"""
     status = Signal(str, str)
-    finished = Signal(str, int)
+    finished = Signal(str, str, int)
     error = Signal(str, object)
 
 
 class ImportWorker(QRunnable):
     """Import worker"""
     def __init__(self, *args, **kwargs):
         super(ImportWorker, self).__init__()
@@ -186,15 +191,15 @@
                 self.import_vector_stores()
             elif self.mode == "truncate_vector_stores":
                 self.truncate_vector_stores()
             elif self.mode == "refresh_vector_stores":
                 self.refresh_vector_stores()
             elif self.mode == "truncate_files":
                 self.truncate_files()
-            elif self.mode == "files":
+            elif self.mode == "import_files":
                 self.import_files()
             elif self.mode == "upload_files":
                 self.upload_files()
         except Exception as e:
             self.signals.error.emit(self.mode, e)
 
     def import_assistants(self, silent: bool = False) -> bool:
@@ -216,99 +221,119 @@
             # import vector stores
             self.import_vector_stores(True)
 
             # import files
             self.import_files(True)
 
             if not silent:
-                self.signals.finished.emit("assistants", len(items))
+                self.signals.finished.emit("assistants", self.store_id, len(items))
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("assistants", e)
             return False
 
     def import_vector_stores(self, silent: bool = False) -> bool:
         """
         Import vector stores from API
 
+        :param silent: silent mode (no signals)
         :return: result
         """
         try:
             print("Importing vector stores...")
             self.window.core.assistants.store.clear()
-            items = self.window.core.assistants.store.get_all()
+            items = {}
             self.window.core.gpt.assistants.import_vector_stores(items)
             self.window.core.assistants.store.import_items(items)
             if not silent:
-                self.signals.finished.emit("vector_stores", len(items))
+                self.signals.finished.emit("vector_stores", self.store_id, len(items))
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("vector_stores", e)
             return False
 
     def truncate_vector_stores(self, silent: bool = False) -> bool:
         """
         Truncate all vector stores in API
 
+        :param silent: silent mode (no signals)
         :return: result
         """
         try:
             print("Truncating stores...")
             num = self.window.core.gpt.assistants.vs_truncate_stores()
             self.window.core.assistants.store.items = {}
             self.window.core.assistants.store.save()
             if not silent:
-                self.signals.finished.emit("truncate_vector_stores", num)
+                self.signals.finished.emit("truncate_vector_stores", self.store_id, num)
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("truncate_vector_stores", e)
             return False
 
     def refresh_vector_stores(self, silent: bool = False) -> bool:
         """
         Refresh all vector stores in API
 
+        :param silent: silent mode (no signals)
         :return: result
         """
         try:
             print("Refreshing stores...")
             num = 0
             stores = self.window.core.assistants.store.items
             for id in stores:
                 store = stores[id]
-                self.window.controller.assistant.store.refresh_store(store, update=False)
-                num += 1
+                try:
+                    self.window.controller.assistant.store.refresh_store(store, update=False)
+                    num += 1
+                except Exception as e:
+                    print("Failed to refresh store: {}".format(id))
+                    self.window.core.debug.log(e)
             if not silent:
-                self.signals.finished.emit("refresh_vector_stores", num)
+                self.signals.finished.emit("refresh_vector_stores", self.store_id, num)
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("refresh_vector_stores", e)
             return False
 
     def truncate_files(self, silent: bool = False) -> bool:
         """
-        Truncate all files in API
+        Truncate files in API
 
+        :param silent: silent mode (no signals)
         :return: result
         """
         try:
-            print("Truncating files...")
-            self.window.core.assistants.files.truncate()  # clear all files, remove from stores and DB
-            num = self.window.core.gpt.assistants.files_truncate()  # remove files in API
+            # if empty store_id, truncate all files, otherwise truncate only store files
+            if self.store_id is None:
+                print("Truncating all files...")
+                self.window.core.assistants.files.truncate() # clear all files
+                num = self.window.core.gpt.assistants.files_truncate()  # remove all files in API
+            else:
+                print("Truncating files for store: {}".format(self.store_id))
+                self.window.core.assistants.files.truncate(self.store_id)  # clear store files, remove from stores and DB
+                num = self.window.core.gpt.assistants.files_truncate_store(self.store_id)  # remove store files in API
             if not silent:
-                self.signals.finished.emit("truncate_files", num)  # in DB (local) handled after
+                self.signals.finished.emit("truncate_files", self.store_id, num)
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("truncate_files", e)
             return False
 
     def upload_files(self, silent: bool = False) -> bool:
         """
         Upload files to API
 
+        :param silent: silent mode (no signals)
         :return: result
         """
         num = 0
         try:
             print("Uploading files...")
             for file in self.files:
                 try:
@@ -324,30 +349,38 @@
                             self.signals.status.emit("upload_files",
                                                      "Uploaded file: {}/{}".format((num + 1), len(self.files)))
                             num = num + 1
                 except Exception as e:
                     self.window.core.debug.log(e)
                     self.signals.status.emit("upload_files", "Failed to upload file: {}".format(os.path.basename(file)))
             if not silent:
-                self.signals.finished.emit("upload_files", num)
+                self.signals.finished.emit("upload_files", self.store_id, num)
             return True
         except Exception as e:
+            print("API error: {}".format(e))
             self.signals.error.emit("upload_files", e)
             return False
 
     def import_files(self, silent: bool = False) -> bool:
         """
         Import assistant files from API
 
         :param silent: silent mode (no signals)
         :return: result
         """
         try:
-            print("Importing all files...")
-            self.window.core.assistants.files.truncate_local()  # clear local DB
-            num = self.window.core.gpt.assistants.vs_import_all_files()
+            if self.store_id is None:
+                print("Importing all files...")
+                self.window.core.assistants.files.truncate_local()  # clear local DB (all)
+                num = self.window.core.gpt.assistants.vs_import_all_files()  # import all files
+            else:
+                print("Importing files for store: {}".format(self.store_id))
+                self.window.core.assistants.files.truncate_local(self.store_id)  # clear local DB (all)
+                items = self.window.core.gpt.assistants.vs_import_store_files(self.store_id, [])  # import store files
+                num = len(items)
             if not silent:
-                self.signals.finished.emit("files", num)
+                self.signals.finished.emit("import_files", self.store_id, num)
             return True
         except Exception as e:
-            self.signals.error.emit("files", e)
+            print("API error: {}".format(e))
+            self.signals.error.emit("import_files", e)
         return False
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.4/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import copy
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QStandardItemModel, QAction, QIcon
 from PySide6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QScrollArea, QWidget, QTabWidget, QFrame, \
@@ -231,62 +231,127 @@
         """
         Setup menu bar
 
         :return: QMenuBar
         """
         self.actions = {}
         self.menu_bar = QMenuBar()
-        self.file_menu = self.menu_bar.addMenu(trans("menu.file"))
 
-        # open
-        self.actions["import"] = QAction(QIcon(":/icons/download.svg"), trans("dialog.assistant.store.menu.import"))
-        self.actions["import"].triggered.connect(
+        self.menu = {}
+        self.menu["current"] = self.menu_bar.addMenu(trans("dialog.assistant.store.menu.current"))
+        self.menu["all"] = self.menu_bar.addMenu(trans("dialog.assistant.store.menu.all"))
+
+        # --------------------------------------------
+
+        # import files (current)
+        self.actions["current.import_files"] = QAction(QIcon(":/icons/download.svg"),
+                                                   trans("dialog.assistant.store.menu.current.import_files"))
+        self.actions["current.import_files"].triggered.connect(
+            lambda: self.window.controller.assistant.batch.import_store_files(
+                self.window.controller.assistant.store.current  # current selected store
+            )
+        )
+
+        # refresh (current)
+        self.actions["current.refresh_store"] = QAction(QIcon(":/icons/reload.svg"),
+                                                     trans("dialog.assistant.store.menu.current.refresh_store"))
+        self.actions["current.refresh_store"].triggered.connect(
+            lambda: self.window.controller.assistant.store.refresh_status()
+        )
+
+        # clear files (current, local)
+        self.actions["current.clear_files"] = QAction(QIcon(":/icons/close.svg"),
+                                                  trans("dialog.assistant.store.menu.current.clear_files"))
+        self.actions["current.clear_files"].triggered.connect(
+            lambda: self.window.controller.assistant.batch.clear_store_files(
+                self.window.controller.assistant.store.current  # current selected store
+            )
+        )
+
+        # truncate files (current, local + remote)
+        self.actions["current.truncate_files"] = QAction(QIcon(":/icons/delete.svg"),
+                                                     trans("dialog.assistant.store.menu.current.truncate_files"))
+        self.actions["current.truncate_files"].triggered.connect(
+            lambda: self.window.controller.assistant.batch.truncate_store_files(
+                self.window.controller.assistant.store.current  # current selected store
+            )
+        )
+
+        # delete (current, local + remote)
+        self.actions["current.delete"] = QAction(QIcon(":/icons/delete.svg"),
+                                                         trans("dialog.assistant.store.menu.current.delete"))
+        self.actions["current.delete"].triggered.connect(
+            lambda: self.window.controller.assistant.store.delete(
+                self.window.controller.assistant.store.current  # current selected store
+            )
+        )
+
+        # --------------------------------------------
+
+        # import all (stores + files)
+        self.actions["all.import_all"] = QAction(QIcon(":/icons/download.svg"), trans("dialog.assistant.store.menu.all.import_all"))
+        self.actions["all.import_all"].triggered.connect(
             lambda: self.window.controller.assistant.batch.import_stores()
         )
 
-        # refresh stores (local)
-        self.actions["refresh_stores"] = QAction(QIcon(":/icons/reload.svg"),
-                                               trans("dialog.assistant.store.menu.refresh_store"))
-        self.actions["refresh_stores"].triggered.connect(
+        # import files (all)
+        self.actions["all.import_files"] = QAction(QIcon(":/icons/download.svg"),
+                                             trans("dialog.assistant.store.menu.all.import_files"))
+        self.actions["all.import_files"].triggered.connect(
+            lambda: self.window.controller.assistant.batch.import_files()
+        )
+
+        # refresh (local)
+        self.actions["all.refresh_stores"] = QAction(QIcon(":/icons/reload.svg"),
+                                               trans("dialog.assistant.store.menu.all.refresh_store"))
+        self.actions["all.refresh_stores"].triggered.connect(
             lambda: self.window.controller.assistant.batch.refresh_stores()
         )
 
-        # clear stores (local)
-        self.actions["clear_stores"] = QAction(QIcon(":/icons/close.svg"),
-                                                  trans("dialog.assistant.store.menu.clear_store"))
-        self.actions["clear_stores"].triggered.connect(
+        # clear stores (all, local)
+        self.actions["all.clear_stores"] = QAction(QIcon(":/icons/close.svg"),
+                                                  trans("dialog.assistant.store.menu.all.clear_store"))
+        self.actions["all.clear_stores"].triggered.connect(
             lambda: self.window.controller.assistant.batch.clear_stores()
         )
 
-        # clear files (local)
-        self.actions["clear_files"] = QAction(QIcon(":/icons/close.svg"),
-                                               trans("dialog.assistant.store.menu.clear_files"))
-        self.actions["clear_files"].triggered.connect(
+        # clear files (all, local)
+        self.actions["all.clear_files"] = QAction(QIcon(":/icons/close.svg"),
+                                               trans("dialog.assistant.store.menu.all.clear_files"))
+        self.actions["all.clear_files"].triggered.connect(
             lambda: self.window.controller.assistant.batch.clear_files()
         )
 
-        # truncate stores
-        self.actions["truncate_stores"] = QAction(QIcon(":/icons/delete.svg"), trans("dialog.assistant.store.menu.truncate_store"))
-        self.actions["truncate_stores"].triggered.connect(
+        # truncate stores (all, local + remote)
+        self.actions["all.truncate_stores"] = QAction(QIcon(":/icons/delete.svg"), trans("dialog.assistant.store.menu.all.truncate_store"))
+        self.actions["all.truncate_stores"].triggered.connect(
             lambda: self.window.controller.assistant.batch.truncate_stores()
         )
 
-        # truncate files
-        self.actions["truncate_files"] = QAction(QIcon(":/icons/delete.svg"), trans("dialog.assistant.store.menu.truncate_files"))
-        self.actions["truncate_files"].triggered.connect(
+        # truncate files (all, local + remote)
+        self.actions["all.truncate_files"] = QAction(QIcon(":/icons/delete.svg"), trans("dialog.assistant.store.menu.all.truncate_files"))
+        self.actions["all.truncate_files"].triggered.connect(
             lambda: self.window.controller.assistant.batch.truncate_files()
         )
 
-        # add actions
-        self.file_menu.addAction(self.actions["import"])
-        self.file_menu.addAction(self.actions["refresh_stores"])
-        self.file_menu.addAction(self.actions["clear_stores"])
-        self.file_menu.addAction(self.actions["clear_files"])
-        self.file_menu.addAction(self.actions["truncate_stores"])
-        self.file_menu.addAction(self.actions["truncate_files"])
+        # current
+        self.menu["current"].addAction(self.actions["current.import_files"])
+        self.menu["current"].addAction(self.actions["current.refresh_store"])
+        self.menu["current"].addAction(self.actions["current.clear_files"])
+        self.menu["current"].addAction(self.actions["current.truncate_files"])
+        self.menu["current"].addAction(self.actions["current.delete"])
+
+        # all
+        self.menu["all"].addAction(self.actions["all.import_all"])
+        self.menu["all"].addAction(self.actions["all.import_files"])
+        self.menu["all"].addAction(self.actions["all.refresh_stores"])
+        self.menu["all"].addAction(self.actions["all.clear_stores"])
+        self.menu["all"].addAction(self.actions["all.clear_files"])
+        self.menu["all"].addAction(self.actions["all.truncate_stores"])
+        self.menu["all"].addAction(self.actions["all.truncate_files"])
 
         return self.menu_bar
 
     def build_widgets(self, options: dict) -> dict:
         """
         Build settings options widgets
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 10:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6 import QtCore
 from PySide6.QtGui import QStandardItemModel, Qt
 from PySide6.QtWidgets import QVBoxLayout, QPushButton, QHBoxLayout, QCheckBox, QLabel, QWidget
 
+from pygpt_net.ui.widget.element.button import SyncButton
 from pygpt_net.ui.widget.element.labels import HelpLabel
 from pygpt_net.ui.widget.lists.uploaded import UploadedFileList
 from pygpt_net.utils import trans
 
 
 class AttachmentsUploaded:
     def __init__(self, window=None):
@@ -64,21 +65,19 @@
         """
         Setup attachments uploaded list
         """
         # attachments
         self.window.ui.nodes[self.id] = UploadedFileList(self.window)
 
         # buttons
-        self.window.ui.nodes['attachments_uploaded.btn.sync'] = QPushButton(trans('attachments_uploaded.btn.sync'))
+        self.window.ui.nodes['attachments_uploaded.btn.sync'] = SyncButton(trans('attachments_uploaded.btn.sync'), self.window)
         self.window.ui.nodes['attachments_uploaded.btn.clear'] = QPushButton(trans('attachments_uploaded.btn.clear'))
-
-        self.window.ui.nodes['attachments_uploaded.btn.sync'].clicked.connect(
-            lambda: self.window.controller.assistant.batch.import_files())
         self.window.ui.nodes['attachments_uploaded.btn.clear'].clicked.connect(
-            lambda: self.window.controller.assistant.files.clear())
+            lambda: self.window.controller.assistant.files.clear()
+        )
 
         self.window.ui.models[self.id] = self.create_model(self.window)
         self.window.ui.nodes[self.id].setModel(self.window.ui.models[self.id])
 
     def create_model(self, parent) -> QStandardItemModel:
         """
         Create list model
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 10:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 from PySide6 import QtCore
 from PySide6.QtGui import QStandardItemModel, Qt
 from PySide6.QtWidgets import QVBoxLayout, QHBoxLayout, QPushButton, QWidget
 
 from pygpt_net.ui.widget.element.labels import HelpLabel, TitleLabel
@@ -52,15 +52,15 @@
         self.window.ui.nodes['assistants.new'] = QPushButton(trans('assistant.new'))
         self.window.ui.nodes['assistants.new'].clicked.connect(
             lambda: self.window.controller.assistant.editor.edit())
 
         # import
         self.window.ui.nodes['assistants.import'] = QPushButton(trans('assistant.import'))
         self.window.ui.nodes['assistants.import'].clicked.connect(
-            lambda: self.window.controller.assistant.batch.import_assistants())
+            lambda: self.window.controller.assistant.batch.import_all())
 
         # label
         self.window.ui.nodes['assistants.label'] = TitleLabel(trans("toolbox.assistants.label"))
 
         # header
         header = QHBoxLayout()
         header.addWidget(self.window.ui.nodes['assistants.label'])
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/button.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.14 20:00:00                  #
+# Updated Date: 2024.04.29 16:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QPushButton, QMenu
 
 from pygpt_net.utils import trans
@@ -67,8 +67,44 @@
             lambda: self.window.controller.ctx.new_group()
         )
 
         if group_id is not None and group_id > 0:
             menu.addAction(actions['new_in_group'])
         menu.addAction(actions['new'])
         menu.addAction(actions['new_group'])
+        menu.exec_(parent.mapToGlobal(pos))
+
+
+class SyncButton(QPushButton):
+    def __init__(self, title: str = None, window=None):
+        super().__init__(title)
+        self.window = window
+        self.clicked.connect(
+            lambda: self.window.controller.assistant.batch.import_files_current()
+        )
+
+    def mousePressEvent(self, event):
+        if event.button() == Qt.RightButton:
+            self.new_context_menu(self, event.pos())
+        else:
+            super().mousePressEvent(event)
+
+    def new_context_menu(self, parent, pos):
+        """
+        Index all btn context menu
+
+        :param parent: parent widget
+        :param pos: mouse  position
+        """
+        menu = QMenu(self)
+        actions = {}
+        actions['current'] = QAction(QIcon(":/icons/download.svg"), trans('attachments_uploaded.btn.sync.current'), self)
+        actions['current'].triggered.connect(
+            lambda: self.window.controller.assistant.batch.import_files_current()
+        )
+        actions['all'] = QAction(QIcon(":/icons/download.svg"), trans('attachments_uploaded.btn.sync.all'), self)
+        actions['all'].triggered.connect(
+            lambda: self.window.controller.assistant.batch.import_files()
+        )
+        menu.addAction(actions['current'])
+        menu.addAction(actions['all'])
         menu.exec_(parent.mapToGlobal(pos))
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,64 +2,63 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.01.29 14:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.ui.widget.lists.base import BaseList
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
 
 
-class AssistantVectorStoreEditorList(BaseList):
+class ModelList(BaseList):
     def __init__(self, window=None, id=None):
         """
-        Store select menu (in editor)
+        Presets select menu
 
         :param window: main window
-        :param id: parent id
+        :param id: input id
         """
-        super(AssistantVectorStoreEditorList, self).__init__(window)
+        super(ModelList, self).__init__(window)
         self.window = window
         self.id = id
 
     def click(self, val):
-        idx = val.row()
-        self.window.controller.assistant.store.select(idx)
+        self.window.controller.model.select(val.row())
+        self.selection = self.selectionModel().selection()
 
     def contextMenuEvent(self, event):
         """
         Context menu event
 
         :param event: context menu event
         """
         actions = {}
-        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.delete'), self)
-        actions['delete'].triggered.connect(
-            lambda: self.action_delete(event))
+        actions['edit'] = QAction(QIcon(":/icons/edit.svg"), trans('action.edit'), self)
+        actions['edit'].triggered.connect(
+            lambda: self.action_edit(event))
 
         menu = QMenu(self)
-        menu.addAction(actions['delete'])
+        menu.addAction(actions['edit'])
 
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
             menu.exec_(event.globalPos())
 
-    def action_delete(self, event):
+    def action_edit(self, event):
         """
-        Delete action handler
+        Edit action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.assistant.store.delete_by_idx(idx)
-
+            self.window.controller.model.editor.open_by_idx(idx)
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,61 +4,61 @@
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Updated Date: 2024.01.29 14:00:00                  #
 # ================================================== #
-
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.ui.widget.lists.base import BaseList
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
 
 
-class ModelList(BaseList):
+class ModelEditorList(BaseList):
     def __init__(self, window=None, id=None):
         """
-        Presets select menu
+        Model select menu (in editor)
 
         :param window: main window
-        :param id: input id
+        :param id: parent id
         """
-        super(ModelList, self).__init__(window)
+        super(ModelEditorList, self).__init__(window)
         self.window = window
         self.id = id
 
     def click(self, val):
-        self.window.controller.model.select(val.row())
-        self.selection = self.selectionModel().selection()
+        idx = val.row()
+        self.window.controller.model.editor.select(idx)
 
     def contextMenuEvent(self, event):
         """
         Context menu event
 
         :param event: context menu event
         """
         actions = {}
-        actions['edit'] = QAction(QIcon(":/icons/edit.svg"), trans('action.edit'), self)
-        actions['edit'].triggered.connect(
-            lambda: self.action_edit(event))
+        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.delete'), self)
+        actions['delete'].triggered.connect(
+            lambda: self.action_delete(event))
 
         menu = QMenu(self)
-        menu.addAction(actions['edit'])
+        menu.addAction(actions['delete'])
 
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
             menu.exec_(event.globalPos())
 
-    def action_edit(self, event):
+    def action_delete(self, event):
         """
-        Edit action handler
+        Delete action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.model.editor.open_by_idx(idx)
+            self.window.controller.model.editor.delete_by_idx(idx)
+
```

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/src/pygpt_net/utils.py` & `pygpt_net-2.2.4/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.3/PKG-INFO` & `pygpt_net-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.3
+Version: 2.2.4
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -70,15 +70,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.3** | build: **2024.04.29** | Python: **>=3.10, <3.12**
+Release: **2.2.4** | build: **2024.04.29** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -3126,14 +3126,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.4 (2024-04-29)**
+
+- Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
+- Added sync current/all context menu options to Sync button.
+- Improved remote stores handling.
+
 **2.2.3 (2024-04-29)**
 
 - Fixed Assistants files sync btn.
 - Added batch upload files or directory in Assistants vector stores dialog.
 
 **2.2.2 (2024-04-29)**
```

