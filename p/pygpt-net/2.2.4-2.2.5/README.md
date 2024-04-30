# Comparing `tmp/pygpt_net-2.2.4.tar.gz` & `tmp/pygpt_net-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.4.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.5.tar", max compression
```

## Comparing `pygpt_net-2.2.4.tar` & `pygpt_net-2.2.5.tar`

### file list

```diff
@@ -1,844 +1,845 @@
--rwxr-xr-x   0        0        0    58137 2024-04-29 15:13:32.567516 pygpt_net-2.2.4/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.4/LICENSE
--rwxr-xr-x   0        0        0   132359 2024-04-29 15:13:32.567516 pygpt_net-2.2.4/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.4/icon.png
--rw-r--r--   0        0        0     2979 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/pyproject.toml
--rwxr-xr-x   0        0        0    57113 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.4/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    15484 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.4/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.4/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    19949 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    13989 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    15446 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15540 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.4/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2144 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.4/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.4/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.4/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.4/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.4/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.4/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.4/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    13539 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15668 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.4/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.4/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.4/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.4/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    20106 2024-04-29 10:51:04.365787 pygpt_net-2.2.4/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.4/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.4/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.4/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.4/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.4/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.4/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.4/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.4/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.4/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.4/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9839 2024-04-29 15:13:32.571516 pygpt_net-2.2.4/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7998 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.4/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.4/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.4/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.4/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.4/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.4/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.4/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.4/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.4/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.4/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/dispatcher.py
--rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.4/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.4/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.4/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.4/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.4/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.4/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.4/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.4/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.4/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.4/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.4/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.4/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    42853 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.4/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.4/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.4/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0    10603 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    18526 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1440 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.completion.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.4/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.4/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.4/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.4/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.4/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.4/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.4/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.4/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.4/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.4/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.4/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    46483 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    54728 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    46620 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    48330 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    45664 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    45600 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    64199 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    49212 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.4/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.4/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.4/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.4/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.4/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.4/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.4/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.4/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.4/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.4/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.4/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.4/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.4/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     6961 2024-03-08 00:36:17.343108 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    29315 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    19981 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    14743 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.4/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.4/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.4/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.4/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.4/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.4/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.4/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    22284 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.4/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4420 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.4/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.4/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.4/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.4/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.4/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.4/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.4/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.4/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.4/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   136075 1970-01-01 00:00:00.000000 pygpt_net-2.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0    58298 2024-04-30 02:35:43.570878 pygpt_net-2.2.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.5/LICENSE
+-rwxr-xr-x   0        0        0   132522 2024-04-30 02:35:43.570878 pygpt_net-2.2.5/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.5/icon.png
+-rw-r--r--   0        0        0     2979 2024-04-30 02:35:43.574879 pygpt_net-2.2.5/pyproject.toml
+-rwxr-xr-x   0        0        0    57272 2024-04-30 02:35:43.574879 pygpt_net-2.2.5/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.5/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/__init__.py
+-rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.5/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.5/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    20263 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15524 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.5/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.5/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.5/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.5/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.5/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.5/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.5/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.5/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.5/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.5/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.5/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.5/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.5/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.5/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.5/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.5/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.5/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.5/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.5/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.5/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    20220 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.5/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.5/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.5/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.5/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.5/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.5/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.5/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.5/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.5/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.5/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.5/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.5/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.5/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.5/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.5/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.5/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.5/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.5/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.5/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.5/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.5/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.5/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.5/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.5/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.5/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.5/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.5/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.5/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.5/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.5/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.5/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.5/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.5/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.5/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.5/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.5/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.5/src/pygpt_net/core/dispatcher.py
+-rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.5/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.5/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.5/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.5/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.5/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.5/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.5/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.5/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.5/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.5/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.5/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.5/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.5/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.5/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.5/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.5/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.5/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.5/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.5/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.5/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.5/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.5/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.5/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.5/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.5/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    42853 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.5/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.5/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.5/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.5/src/pygpt_net/core/worker.py
+-rwxr-xr-x   0        0        0    10603 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    18526 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1440 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.completion.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.5/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.5/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.5/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.5/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.5/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.5/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.5/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.5/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.5/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.5/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.5/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.5/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.5/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    46483 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    54728 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    46620 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    48330 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    45664 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    45600 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    64199 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    49212 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.5/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.5/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.5/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.5/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.5/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.5/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.5/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.5/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.5/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.5/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.5/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.5/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.5/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.5/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.5/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.5/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.5/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.5/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.5/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.5/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.5/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.5/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.5/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.5/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.5/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     7282 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    13070 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0    15246 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/store.py
+-rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    14656 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.5/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.5/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.5/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.5/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.5/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.5/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.5/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.5/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.5/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.5/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.5/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.5/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.5/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.5/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.5/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.5/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.5/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.5/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.5/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.5/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.5/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.5/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.5/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.5/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.5/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.5/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.5/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.5/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.5/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.5/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.5/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.5/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   136238 1970-01-01 00:00:00.000000 pygpt_net-2.2.5/PKG-INFO
```

### Comparing `pygpt_net-2.2.4/CHANGELOG.md` & `pygpt_net-2.2.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+# 2.2.5 (2024-04-30)
+
+- Fix: import button handler in Assistants.
+- Refactored and improved stores batch actions events handling.
+- Added missing translations.
+
 # 2.2.4 (2024-04-29)
 
 - Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
 - Added sync current/all context menu options to Sync button.
 - Improved remote stores handling.
 
 # 2.2.3 (2024-04-29)
```

### Comparing `pygpt_net-2.2.4/LICENSE` & `pygpt_net-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/README.md` & `pygpt_net-2.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.4** | build: **2024.04.29** | Python: **>=3.10, <3.12**
+Release: **2.2.5** | build: **2024.04.30** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -3054,14 +3054,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.5 (2024-04-30)**
+
+- Fix: import button handler in Assistants.
+- Refactored and improved stores batch actions events handling.
+- Added missing translations.
+
 **2.2.4 (2024-04-29)**
 
 - Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
 - Added sync current/all context menu options to Sync button.
 - Improved remote stores handling.
 
 **2.2.3 (2024-04-29)**
```

### Comparing `pygpt_net-2.2.4/icon.png` & `pygpt_net-2.2.5/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/pyproject.toml` & `pygpt_net-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.4"
+version = "2.2.5"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.5/src/pygpt_net/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.2.5 (2024-04-30)
+
+- Fix: import button handler in Assistants.
+- Refactored and improved stores batch actions events handling.
+- Added missing translations.
+
 2.2.4 (2024-04-29)
 
 - Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
 - Added sync current/all context menu options to Sync button.
 - Improved remote stores handling.
 
 2.2.3 (2024-04-29)
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/LICENSE` & `pygpt_net-2.2.5/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.4"
-__build__ = "2024.04.29"
+__version__ = "2.2.5"
+__build__ = "2024.04.30"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
 __documentation__ = "https://pygpt.readthedocs.io"
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/app.py` & `pygpt_net-2.2.5/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/config.py` & `pygpt_net-2.2.5/src/pygpt_net/config.py`

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
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import os
 import re
 
@@ -517,15 +517,15 @@
             try:
                 value = str(item['value'].format(**self.all()))
                 os.environ[item['name']] = value
                 list_loaded.append(item['name'])
             except Exception as e:
                 print("Error setting env var: {}".format(e))
         if list_loaded:
-            print("Loaded environment vars: {}".format(", ".join(list_loaded)))
+            print("Setting environment vars: {}".format(", ".join(list_loaded)))
 
     def save(self, filename: str = "config.json"):
         """
         Save config
 
         :param filename: filename
         """
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/container.py` & `pygpt_net-2.2.5/src/pygpt_net/container.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/batch.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 
 from PySide6.QtWidgets import QApplication, QFileDialog
 
 from pygpt_net.utils import trans
 
@@ -195,14 +195,15 @@
             self.window.ui.dialogs.confirm(
                 type='assistant.files.clear.store',
                 id=store_id,
                 msg=trans('confirm.assistant.files.clear'),
             )
             return
         self.window.ui.status("Clearing store files...please wait...")
+        QApplication.processEvents()
         self.window.core.assistants.files.truncate_local(store_id)  # clear files local
         self.window.controller.assistant.files.update()
         self.window.ui.status("OK. All store files cleared.")
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def clear_files(self, force: bool = False):
         """
@@ -214,14 +215,15 @@
             self.window.ui.dialogs.confirm(
                 type='assistant.files.clear.all',
                 id='',
                 msg=trans('confirm.assistant.files.clear'),
             )
             return
         self.window.ui.status("Clearing files...please wait...")
+        QApplication.processEvents()
         self.window.core.assistants.files.truncate_local()  # clear files local
         self.window.controller.assistant.files.update()
         self.window.ui.status("OK. All files cleared.")
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def clear_stores(self, force: bool = False):
         """
@@ -233,14 +235,15 @@
             self.window.ui.dialogs.confirm(
                 type='assistant.store.clear',
                 id='',
                 msg=trans('confirm.assistant.store.clear'),
             )
             return
         self.window.ui.status("Clearing vector stores...please wait...")
+        QApplication.processEvents()
         self.window.core.assistants.store.truncate()  # clear all stores
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
         self.window.ui.status("OK. All stores cleared.")
         self.window.controller.assistant.store.current = None
         self.window.controller.assistant.store.init()
 
@@ -255,14 +258,15 @@
                 type='assistant.store.truncate',
                 id='',
                 msg=trans('confirm.assistant.store.truncate'),
             )
             return
         # run asynchronous
         self.window.ui.status("Removing vector stores...please wait...")
+        QApplication.processEvents()
         self.window.core.assistants.store.truncate()  # clear all stores
         self.window.core.gpt.assistants.importer.truncate_vector_stores()
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
         self.window.controller.assistant.store.current = None
         self.window.controller.assistant.store.init()
 
@@ -285,30 +289,31 @@
 
     def handle_imported_assistants(self, num: int):
         """
         Handle imported assistants
 
         :param num: number of imported assistants
         """
-        self.window.ui.status("OK. Imported assistants: " + str(num) + ".")
         self.window.controller.assistant.update()
         self.window.controller.assistant.store.update()
         self.window.controller.assistant.files.update()
+        self.window.ui.status("OK. Imported assistants: " + str(num) + ".")
+        self.window.ui.dialogs.alert(trans("status.finished"))
 
     def handle_imported_assistants_failed(self, error: any):
         """
         Handle error on importing assistants
 
         :param error: error message
         """
         self.window.core.debug.log(error)
         print("Error importing assistants")
+        self.window.controller.assistant.update()
         self.window.ui.status("Error importing assistants.")
         self.window.ui.dialogs.alert(error)
-        self.window.controller.assistant.update()
 
     def handle_refreshed_stores(self, num: int):
         """
         Handle refreshed stores
 
         :param num: number of refreshed files
         """
@@ -321,92 +326,92 @@
         """
         Handle error on refreshing stores
 
         :param error: error message
         """
         self.window.core.debug.log(error)
         print("Error refreshing stores", error)
-        self.window.ui.status("Error refreshing stores.")
-        self.window.ui.dialogs.alert(error)
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
+        self.window.ui.status("Error refreshing stores.")
+        self.window.ui.dialogs.alert(error)
 
     def handle_imported_stores(self, num: int):
         """
         Handle imported stores
 
         :param num: number of imported files
         """
-        self.window.ui.status("OK. Imported stores: " + str(num) + ".")
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
+        self.window.ui.status("OK. Imported stores: " + str(num) + ".")
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def handle_imported_stores_failed(self, error: any):
         """
         Handle error on importing stores
 
         :param error: error message
         """
         self.window.core.debug.log(error)
+        self.window.controller.assistant.files.update()
+        self.window.controller.assistant.store.update()
         print("Error importing stores", error)
         self.window.ui.status("Error importing stores.")
         self.window.ui.dialogs.alert(error)
-        self.window.controller.assistant.files.update()
-        self.window.controller.assistant.store.update()
 
     def handle_truncated_stores(self, num: int):
         """
         Handle truncated stores
 
         :param num: number of removed files
         """
         self.window.core.assistants.store.truncate()
         self.remove_all_stores_from_assistants()
-        self.window.ui.status("OK. Removed stores: " + str(num) + ".")
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
         self.window.controller.assistant.store.current = None
         self.window.controller.assistant.store.init()
+        self.window.ui.status("OK. Removed stores: " + str(num) + ".")
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def handle_truncated_stores_failed(self, error: any):
         """
         Handle error on truncating stores
 
         :param error: error message
         """
         self.window.core.debug.log(error)
         print("Error removing stores", error)
-        self.window.ui.status("Error removing stores.")
-        self.window.ui.dialogs.alert(error)
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.update()
+        self.window.ui.status("Error removing stores.")
+        self.window.ui.dialogs.alert(error)
 
     def handle_imported_files(self, num: int):
         """
         Handle imported files
 
         :param num: number of imported files
         """
-        self.window.ui.status("OK. Imported files: " + str(num) + ".")
         self.window.controller.assistant.files.update()
+        self.window.ui.status("OK. Imported files: " + str(num) + ".")
         self.window.ui.dialogs.alert(trans("status.finished"))
 
     def handle_imported_files_failed(self, error: any):
         """
         Handle error on importing files
 
         :param error: error message
         """
         self.window.core.debug.log(error)
+        self.window.controller.assistant.files.update()
         print("Error importing files")
         self.window.ui.status("Error importing files.")
         self.window.ui.dialogs.alert(error)
-        self.window.controller.assistant.files.update()
 
     def handle_truncated_files(self, store_id: str = None, num: int = 0):
         """
         Handle truncated (in API) files
 
         :param store_id: vector store ID
         :param num: number of truncated files
@@ -421,17 +426,17 @@
         """
         Handle error on truncated files
 
         :param error: error message
         """
         self.window.core.debug.log(error)
         print("Error truncating files")
+        self.window.controller.assistant.files.update()
         self.window.ui.status("Error truncating files.")
         self.window.ui.dialogs.alert(error)
-        self.window.controller.assistant.files.update()
 
     def remove_store_from_assistants(self, store_id: str):
         """
         Remove vector store from all assistants after store deletion
 
         :param store_id: vector store ID
         """
@@ -510,40 +515,42 @@
         :param force: if true, uploads without confirmation
         """
         if self.window.controller.assistant.store.current is None:
             self.window.ui.dialogs.alert(trans("dialog.assistant.store.alert.select"))
             return
 
         store_id = self.window.controller.assistant.store.current
+        self.window.ui.status("Uploading files...please wait...")
+        QApplication.processEvents()
         self.window.core.gpt.assistants.importer.upload_files(store_id, self.files_to_upload)
         self.files_to_upload = []  # clear files
 
     def handle_uploaded_files(self, num: int):
         """
         Handle uploaded files
 
         :param num: number of uploaded files
         """
-        self.window.ui.status("OK. Uploaded files: " + str(num) + ".")
-        self.window.ui.dialogs.alert("OK. Uploaded files: " + str(num) + ".")
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.refresh_status()
+        self.window.ui.status("OK. Uploaded files: " + str(num) + ".")
+        self.window.ui.dialogs.alert("OK. Uploaded files: " + str(num) + ".")
 
     def handle_uploaded_files_failed(self, error: any):
         """
         Handle error on uploading files
 
         :param error: error message
         """
         self.window.core.debug.log(error)
         print("Error uploading files")
-        self.window.ui.status("Error uploading files.")
-        self.window.ui.dialogs.alert(error)
         self.window.controller.assistant.files.update()
         self.window.controller.assistant.store.refresh_status()
+        self.window.ui.status("Error uploading files.")
+        self.window.ui.dialogs.alert(error)
 
     def handle_status_change(self, mode: str, msg: str):
         """
         Handle status change
 
         :param mode: status mode
         :param msg: status message
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.item.assistant import AssistantItem
@@ -170,15 +170,20 @@
                 file = items[id]
                 try:
                     self.window.core.assistants.files.delete(file)  # delete from DB, API and vector stores
                 except Exception as e:
                     self.window.ui.status(trans('status.error'))
                     self.window.ui.dialogs.alert(e)
 
+            # update store status
+            if assistant.vector_store:
+                self.window.controller.assistant.store.refresh_by_store_id(assistant.vector_store)
+
             self.window.ui.status(trans('status.deleted'))
+
         self.update()
 
     def delete(self, idx: int, force: bool = False):
         """
         Delete file
 
         :param idx: file idx
@@ -207,14 +212,19 @@
             return
 
         # delete file in API
         self.window.ui.status(trans('status.sending'))
         QApplication.processEvents()
         try:
             self.window.core.assistants.files.delete(file)  # delete from DB, API and vector stores
+
+            # update store status
+            if assistant.vector_store:
+                self.window.controller.assistant.store.refresh_by_store_id(assistant.vector_store)
+
             self.window.ui.status(trans('status.deleted'))
         except Exception as e:
             self.window.core.debug.log(e)
             self.window.ui.dialogs.alert(e)
             self.window.ui.status(trans('status.error'))
 
         self.update()
@@ -255,34 +265,33 @@
                 msg = "Uploading file: {}".format(attachment.path)
                 self.window.core.debug.info(msg, False)
                 # check if file exists
                 if not os.path.exists(attachment.path):
                     continue
 
                 # upload local attachment file and get new ID (file_id)
-                new_id = self.window.core.gpt.assistants.file_upload(
-                    assistant_id,  # unused, deprecated
+                new_id = self.window.core.gpt.store.upload(
                     attachment.path,
                 )
                 if new_id is not None:
                     # mark as already uploaded
                     attachment.send = True
                     attachment.id = new_id
                     attachment.remote = new_id
 
                     """
                     if assistant.vector_store is None or assistant.vector_store == "":
-                        assistant.vector_store = self.window.core.gpt.assistants.vs_create(
+                        assistant.vector_store = self.window.core.gpt.store.create_store(
                             "thread-" + thread_id,
                         )
                     """
 
                     # add to vector store if defined in assistant, otherwise file will be added to thread store
                     if assistant.vector_store:
-                        self.window.core.gpt.assistants.vs_add_file(
+                        self.window.core.gpt.store.add_file(
                             assistant.vector_store,
                             new_id,
                         )
 
                     # replace old ID with new one
                     self.window.core.attachments.replace_id(
                         mode,
@@ -312,14 +321,18 @@
         self.window.core.assistants.save()
 
         # update attachments UI
         self.window.controller.attachment.update()
 
         # update uploaded list
         if num > 0:
+            # update store status
+            if assistant.vector_store:
+                self.window.controller.assistant.store.refresh_by_store_id(assistant.vector_store)
+
             self.update_list()  # update uploaded list UI
 
         return num
 
     def append(self, assistant: AssistantItem, attachment: AttachmentItem):
         """
         Append attachment to assistant
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/store.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import copy
 import json
 
 from PySide6.QtWidgets import QApplication
 
@@ -183,15 +183,15 @@
 
     def refresh_by_store_id(self, store_id: str):
         """
         Refresh store by ID
 
         :param store_id: store id
         """
-        if store_id is not None:
+        if store_id is not None and store_id in self.window.core.assistants.store.items:
             store = self.window.core.assistants.store.items[store_id]
             if store is not None:
                 self.window.ui.status(trans('status.sending'))
                 QApplication.processEvents()
                 self.refresh_store(store)
                 self.window.ui.status(trans('status.assistant.saved'))
                 self.update()
@@ -295,14 +295,15 @@
 
         # switch to created store
         self.current = store.id
         idx = self.get_tab_by_id(self.current)
         self.set_by_tab(idx)
         self.init()
         self.restore_selection()
+        self.refresh_by_store_id(store.id)
 
     def delete_by_idx(self, idx: int, force: bool = False):
         """
         Delete store by idx
 
         :param idx: store idx
         :param force: force delete
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/attachment.py`

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
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import os
 from datetime import datetime
 
 from PySide6.QtGui import QImage
 from PySide6.QtWidgets import QFileDialog, QApplication
@@ -335,15 +335,15 @@
 
         :param file_id: file id to download (id in OpenAI API)
         :param ext: file extension to add (optional)
         :return: path to downloaded file
         """
         try:
             # get file info from assistant API
-            data = self.window.core.gpt.assistants.file_info(file_id)
+            data = self.window.core.gpt.store.get_file(file_id)
             if data is None:
                 return
 
             # prepare path to download file
             data.filename = os.path.basename(data.filename)
 
             # add extension if provided
@@ -361,15 +361,15 @@
             # check if file exists, if yes, append timestamp prefix
             if os.path.exists(path):
                 # append timestamp prefix to filename
                 filename = f'{datetime.now().strftime("%Y%m%d%H%M%S")}_{data.filename}'
                 path = self.get_download_path(filename)
 
             # download file
-            self.window.core.gpt.assistants.file_download(
+            self.window.core.gpt.store.download(
                 file_id=file_id,
                 path=path,
             )
             return path  # return path to downloaded file
         except Exception as e:
             self.window.core.debug.log(e)
             self.window.ui.dialogs.alert(e)
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,58 +2,50 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.15 10:00:00                  #
+# Updated Date: 2024.03.17 13:00:00                  #
 # ================================================== #
 
-from pygpt_net.utils import trans
+from pygpt_net.item.ctx import CtxItem
 
 
-class Files:
+class Summarizer:
     def __init__(self, window=None):
         """
-        Chat files/attachments controller
+        Summarizer
 
         :param window: Window instance
         """
         self.window = window
 
-    def upload(self, mode: str) -> dict:
+    def summary_ctx(self, ctx: CtxItem) -> str:
         """
-        Upload attachments
+        Summarize conversation begin
 
-        :param mode: mode
-        :return: uploaded attachments list
+        :param ctx: context item (CtxItem)
+        :return: response text (generated summary)
         """
-        self.window.core.gpt.assistants.file_ids = []  # clear file ids
-        attachments_list = {}
-
-        if mode == 'assistant':
-            is_upload = False
-            num_uploaded = 0
-            try:
-                # upload only new attachments (not uploaded yet to remote)
-                attachments = self.window.core.attachments.get_all(mode)
-                c = self.window.controller.assistant.files.count_upload(attachments)
-                if c > 0:
-                    is_upload = True
-                    self.window.ui.status(trans('status.uploading'))
-                    num_uploaded = self.window.controller.assistant.files.upload(
-                        mode,
-                        attachments,
-                    )
-                    self.window.core.gpt.assistants.file_ids = self.window.core.attachments.get_ids(mode)
-                    attachments_list = self.window.core.attachments.make_json_list(attachments)
-
-                # show uploaded status
-                if is_upload and num_uploaded > 0:
-                    self.window.ui.status(trans('status.uploaded'))
-
-            except Exception as e:
-                self.window.core.debug.log(e)
-                self.window.ui.dialogs.alert(e)
-
-        return attachments_list
+        model = self.window.core.models.from_defaults()
+        system_prompt = self.window.core.prompt.get('ctx.auto_summary.system')
+        text = (self.window.core.prompt.get('ctx.auto_summary.user').
+                replace("{input}", str(ctx.input)).
+                replace("{output}", str(ctx.output)))
+
+        if self.window.core.config.get('ctx.auto_summary.model') is not None \
+                and self.window.core.config.get('ctx.auto_summary.model') != "":
+            tmp_model = self.window.core.config.get('ctx.auto_summary.model')
+            if self.window.core.models.has(tmp_model):
+                model = self.window.core.models.get(tmp_model)
+
+        # quick call OpenAI API
+        response = self.window.core.bridge.quick_call(
+            prompt=text,
+            system_prompt=system_prompt,
+            max_tokens=500,
+            model=model,
+        )
+        if response is not None:
+            return response
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/text.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/config/placeholder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ctx/extra.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/confirm.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 class Confirm:
     def __init__(self, window=None):
         """
         Confirmation dialogs controller
 
@@ -148,15 +148,15 @@
         elif type == 'editor.changed.restore':
             self.window.tools.get("editor").restore(id=id, force=True, save=True)
 
         # assistants
         elif type == 'assistant.delete':
             self.window.controller.assistant.delete(id, True)
         elif type == 'assistant.import':
-            self.window.controller.assistant.batch.import_all(True)
+            self.window.controller.assistant.batch.import_assistants(True)
         elif type == 'assistant.files.import.all':
             self.window.controller.assistant.batch.import_files(True)
         elif type == 'assistant.files.import.store':
             self.window.controller.assistant.batch.import_store_files(id, True)  # by store_id
         elif type == 'assistant.files.truncate':
             self.window.controller.assistant.batch.truncate_files(True)
         elif type == 'assistant.files.truncate.store':
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/files.py`

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
-# Updated Date: 2024.01.31 18:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import datetime
 import os
 import shutil
 
 from PySide6.QtCore import QUrl
@@ -27,14 +27,15 @@
     def __init__(self, window=None):
         """
         Files controller
 
         :param window: Window instance
         """
         self.window = window
+        self.uploaded_ids = []
 
     def selection_change(self):
         """Select on list change"""
         # TODO: implement this
         pass
 
     def delete_recursive(self, path: str, force: bool = False):
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/lang/mapping.py`

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
-# Updated Date: 2024.04.29 12:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 from pygpt_net.utils import trans
 
 
 class Mapping:
     def __init__(self, window=None):
@@ -114,14 +114,15 @@
         nodes['input.send_none'] = 'input.radio.none'
         nodes['input.send_clear'] = 'input.send_clear'
         nodes['input.send_btn'] = 'input.btn.send'
         nodes['input.update_btn'] = 'input.btn.update'
         nodes['input.cancel_btn'] = 'input.btn.cancel'
         nodes['input.stop_btn'] = 'input.btn.stop'
         nodes['input.stream'] = 'input.stream'
+        nodes['inline.vision'] = 'inline.vision'
 
         # interpreter
         nodes['interpreter.all'] = 'interpreter.all'
         nodes['interpreter.auto_clear'] = 'interpreter.auto_clear'
         nodes['interpreter.output_label'] = 'interpreter.edit_label.output'
         nodes['interpreter.edit_label'] = 'interpreter.edit_label.edit'
         nodes['interpreter.btn.clear'] = 'dialog.logger.btn.clear'
@@ -139,15 +140,14 @@
         nodes['assistant.model.label'] = 'assistant.model'
         nodes['assistant.description.label'] = 'assistant.description'
         nodes['assistant.tool.function.label'] = 'assistant.functions.label'
 
         # assistants: vector store
         nodes['assistant.store.btn.new'] = 'dialog.assistant.store.btn.new'
         nodes['assistant.store.btn.save'] = 'dialog.assistant.store.btn.save'
-        nodes['assistant.store.btn.refresh_status'] = 'dialog.assistant.store.btn.refresh_status'
         nodes['assistant.store.btn.upload.files'] = 'dialog.assistant.store.btn.upload.files'
         nodes['assistant.store.btn.upload.dir'] = 'dialog.assistant.store.btn.upload.dir'
         nodes['assistant.store.btn.close'] = 'dialog.assistant.store.btn.close'
         nodes['assistant.store.hide_thread'] = 'assistant.store.hide_threads'
 
         # nodes['assistant.id_tip'] = 'assistant.new.id_tip'
         # nodes['assistant.api.tip'] = 'assistant.api.tip'
@@ -383,14 +383,16 @@
         tooltips['inline.vision'] = 'vision.checkbox.tooltip'
         # tooltips['vision.capture.enable'] = 'vision.capture.enable.tooltip'
         # tooltips['vision.capture.auto'] = 'vision.capture.auto.tooltip'
         tooltips['cmd.enabled'] = 'cmd.tip'
         tooltips['icon.video.capture'] = 'icon.video.capture'
         tooltips['icon.audio.output'] = 'icon.audio.output'
         tooltips['icon.audio.input'] = 'icon.audio.input'
+        tooltips['assistant.store.btn.refresh_status'] = 'dialog.assistant.store.btn.refresh_status'
+        tooltips['inline.vision'] = 'vision.checkbox.tooltip'
 
         # menu tooltips
         menu_tooltips = {}
         menu_tooltips['video.capture'] = 'vision.capture.enable.tooltip'
         menu_tooltips['video.capture.auto'] = 'vision.capture.auto.tooltip'
 
         # placeholders
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/settings/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.5/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.5/src/pygpt_net/core/assistants/files.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 from packaging.version import Version
 
 from pygpt_net.item.assistant import AssistantFileItem, AssistantItem
 from pygpt_net.provider.core.assistant_file.db_sqlite import DbSqliteProvider
 
@@ -218,20 +218,20 @@
         file_id = file.file_id
         items = self.get_all_by_file_id(file_id)  # get store_ids
         for id in items:
             store_id = items[id].store_id
             if store_id is None or store_id == "":
                 continue  # skip if no store_id
             try:
-                self.window.core.gpt.assistants.vs_delete_file(store_id, file_id)  # remove from vector store
+                self.window.core.gpt.store.delete_store_file(store_id, file_id)  # remove from vector store
             except Exception as e:
                 self.window.core.debug.log("Failed to delete file from vector store: " + str(e))
         self.provider.delete_by_id(file.record_id)  # delete file in DB
         try:
-            self.window.core.gpt.assistants.file_delete(file.file_id)  # delete file in API
+            self.window.core.gpt.store.delete_file(file.file_id)  # delete file in API
         except Exception as e:
             self.window.core.debug.log("Failed to delete remote file: " + str(e))
         if file.record_id in self.items:
             del self.items[file.record_id]
         return True
 
     def on_store_deleted(self, store_id: str):
@@ -263,17 +263,17 @@
         """
         Truncate all files
 
         :param store_id: store ID
         :return: True if truncated
         """
         if store_id is not None:
-            self.window.core.gpt.assistants.vs_remove_files_from_store(store_id)  # remove files from vector store
+            self.window.core.gpt.store.remove_from_store(store_id)  # remove files from vector store
         else:
-            self.window.core.gpt.assistants.vs_remove_files_from_stores()  # remove files from all vector stores
+            self.window.core.gpt.store.remove_from_stores()  # remove files from all vector stores
         return self.truncate_local(store_id)  # truncate files in DB
 
     def truncate_local(self, store_id: str = None) -> bool:
         """
         Truncate all files (local only)
 
         :param store_id: store ID
@@ -289,15 +289,15 @@
     def import_from_store(self, store_id: str) -> bool:
         """
         Import files from store
 
         :param store_id: store ID
         :return: True if imported
         """
-        files = self.window.core.gpt.assistants.vs_import_store_files(store_id)
+        files = self.window.core.gpt.store.import_store_files(store_id)
         for file in files:
             self.create(file.assistant, file.thread_id, file.file_id, file.name, file.path, file.size)
         return True
 
     def insert(self, store_id: str, data) -> AssistantFileItem:
         """
         Insert file object
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.5/src/pygpt_net/core/assistants/store.py`

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
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 import datetime
 
 from packaging.version import Version
 
 from pygpt_net.item.assistant import AssistantStoreItem, AssistantItem
 from pygpt_net.provider.core.assistant_store.db_sqlite import DbSqliteProvider
@@ -100,15 +100,15 @@
     def create(self) -> AssistantStoreItem or None:
         """
         Create new store
 
         :return: store item
         """
         name = "New vector store"
-        vector_store = self.window.core.gpt.assistants.vs_create(name, 0)
+        vector_store = self.window.core.gpt.store.create_store(name, 0)
         if vector_store is None:
             return None
         store = AssistantStoreItem()
         store.id = vector_store.id
         store.name = name
         store.is_thread = False
         store.record_id = self.provider.create(store)
@@ -118,30 +118,30 @@
     def update(self, store: AssistantStoreItem) -> AssistantStoreItem or None:
         """
         Update store
 
         :param store: store
         :return: updated store or None if failed
         """
-        vector_store = self.window.core.gpt.assistants.vs_update(store.id, store.name, store.expire_days)
+        vector_store = self.window.core.gpt.store.update_store(store.id, store.name, store.expire_days)
         if vector_store is None:
             return None
         self.items[store.id] = store
         self.provider.save(store)
         return store
 
     def get_status_data(self, id: str):
         """
         Get store status data
 
         :param id: store id
         :return: status data, store data
         """
         status = {}
-        data = self.window.core.gpt.assistants.vs_get(id)
+        data = self.window.core.gpt.store.get_store(id)
         if data is not None:
             status = self.parse_status(data)
         return status, data
 
     def parse_status(self, store) -> dict:
         """
         Parse store status
@@ -226,15 +226,15 @@
 
         :param id: store id
         :return: True if store was deleted
         """
         if id in self.items:
             store = self.items[id]
             self.provider.delete_by_id(store.record_id)
-            self.window.core.gpt.assistants.vs_delete(id)
+            self.window.core.gpt.store.remove_store(id)
             del self.items[id]
             return True
         return False
 
     def import_items(self, items: dict):
         """
         Insert items
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.5/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.5/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.5/src/pygpt_net/core/bridge.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.5/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.5/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.5/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/command.py` & `pygpt_net-2.2.5/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.5/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.5/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.5/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.5/src/pygpt_net/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.5/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.5/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.5/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/history.py` & `pygpt_net-2.2.5/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/image.py` & `pygpt_net-2.2.5/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/info.py` & `pygpt_net-2.2.5/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.5/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.5/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/models.py` & `pygpt_net-2.2.5/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.5/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.5/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.5/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.5/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.5/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.5/src/pygpt_net/core/prompt/template.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.5/src/pygpt_net/core/render/web/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.5/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.5/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.5/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/web.py` & `pygpt_net-2.2.5/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/config.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984076433121019%*

 * *Differences: {"'__meta__'": "{'version': '2.2.5', 'app.version': '2.2.5', 'updated_at': '2024-04-30T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.4",
-        "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.4"
+        "app.version": "2.2.5",
+        "updated_at": "2024-04-30T00:00:00",
+        "version": "2.2.5"
     },
     "agent.auto_stop": true,
     "agent.goal.notify": true,
     "agent.idx": "base",
     "agent.iterations": 3,
     "agent.mode": "chat",
     "ai_name": "",
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/models.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.5', 'app.version': '2.2.5', 'updated_at': '2024-04-30T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.4",
-        "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.4"
+        "app.version": "2.2.5",
+        "updated_at": "2024-04-30T00:00:00",
+        "version": "2.2.5"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/modes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.5', 'app.version': '2.2.5', 'updated_at': '2024-04-30T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.4",
-        "updated_at": "2024-04-29T00:00:00",
-        "version": "2.2.4"
+        "app.version": "2.2.5",
+        "updated_at": "2024-04-30T00:00:00",
+        "version": "2.2.5"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/presets/current.agent.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/presets/current.agent.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/settings.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.5/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.5/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.5/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.5/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.5/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.5/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.de.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.es.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.it.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.5/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.5/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.5/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.5/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.5/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.5/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.5/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.5/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.5/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.5/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.5/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.5/src/pygpt_net/item/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/index.py` & `pygpt_net-2.2.5/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.5/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/model.py` & `pygpt_net-2.2.5/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.5/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.5/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/launcher.py` & `pygpt_net-2.2.5/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.5/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/config/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.21 01:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 from openai import OpenAI
 
 from pygpt_net.item.ctx import CtxItem
 
 from .assistants import Assistants
 from .chat import Chat
 from .completion import Completion
 from .image import Image
+from .store import Store
 from .summarizer import Summarizer
 from .vision import Vision
 
 
 class Gpt:
     def __init__(self, window=None):
         """
@@ -29,14 +30,15 @@
         :param window: Window instance
         """
         self.window = window
         self.assistants = Assistants(window)
         self.chat = Chat(window)
         self.completion = Completion(window)
         self.image = Image(window)
+        self.store = Store(window)
         self.summarizer = Summarizer(window)
         self.vision = Vision(window)
 
     def get_client(self) -> OpenAI:
         """
         Return OpenAI client
 
@@ -70,26 +72,32 @@
         ctx = kwargs.get("ctx", CtxItem())
         ai_name = ctx.output_name
         thread_id = ctx.thread
 
         # prepare max tokens
         max_tokens = self.window.core.config.get('max_output_tokens')
 
+        model_id = None
+        if model is not None:
+            model_id = model.id
+
         # check max output tokens
         if max_tokens > model.tokens:
             max_tokens = model.tokens
 
         # minimum 1 token is required
         if max_tokens < 1:
             max_tokens = 1
 
         response = None
         used_tokens = 0
         kwargs['max_tokens'] = max_tokens  # append max output tokens to kwargs
 
+        file_ids = self.window.controller.files.uploaded_ids  # uploaded files IDs
+
         # get response
         if mode == "completion":
             response = self.completion.send(**kwargs)
             used_tokens = self.completion.get_used_tokens()
 
         elif mode == "chat":
             response = self.chat.send(**kwargs)
@@ -112,22 +120,25 @@
                 ctx.urls = urls
 
         elif mode == "assistant":
             # check if assistant is already running and has tools outputs, then submit them, async handled
             if ctx.run_id is not None and len(tools_outputs) > 0:
                 self.assistants.worker.tools_submit(
                     ctx,
+                    model_id,
                     tools_outputs,  # list of tools outputs
                 )
             else:
                 # if not running, then send msg and create new assistant run, async handled
                 self.assistants.worker.msg_send(
                     ctx,
                     thread_id,
                     assistant_id,
+                    model_id,
+                    file_ids,
                     prompt,
                     system_prompt,
                 )
             return True  # if assistant mode then return here, will be handled async
 
         # if stream
         if stream:
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files 4% similar despite different names*

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
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 from openai import AssistantEventHandler
 
 from PySide6.QtCore import QObject, Signal, QRunnable, Slot
 from typing_extensions import override
 
@@ -58,52 +58,61 @@
         self.window.threadpool.start(worker)
 
     def msg_send(
             self,
             ctx: CtxItem,
             thread_id: str,
             assistant_id: str,
+            model: str,
+            file_ids: list,
             prompt: str,
             system_prompt: str
     ):
         """
         Send message to assistant thread
 
         :param ctx: context item
         :param thread_id: thread id
         :param assistant_id: assistant id
+        :param model: model ID
+        :param file_ids: uploaded file IDs
         :param prompt: prompt
         :param system_prompt: system prompt
         """
         worker = Worker()
         worker.window = self.window
         worker.mode = "msg_send"
+        worker.model = model
         worker.ctx = ctx
         worker.thread_id = thread_id
         worker.assistant_id = assistant_id
         worker.prompt = prompt
+        worker.file_ids = file_ids
         worker.system_prompt = system_prompt
         worker.stream = self.window.core.config.get("stream")
         self.connect_signals(worker)
         self.window.threadpool.start(worker)
 
     def tools_submit(
             self,
             ctx: CtxItem,
+            model: str,
             tools_outputs: list,
     ):
         """
         Send tools outputs to assistant thread
 
         :param ctx: context item
+        :param model: model ID
         :param tools_outputs: list of tools outputs
         """
         worker = Worker()
         worker.window = self.window
         worker.mode = "tools_submit"
+        worker.model = model
         worker.ctx = ctx
         worker.tools_outputs = tools_outputs
         worker.stream = self.window.core.config.get("stream")
         self.connect_signals(worker)
         self.window.threadpool.start(worker)
 
     def connect_signals(self, worker):
@@ -503,16 +512,18 @@
 class Worker(QRunnable):
     """Assistants worker"""
     def __init__(self, *args, **kwargs):
         super(Worker, self).__init__()
         self.signals = WorkerSignals()
         self.window = None
         self.mode = None
+        self.model = None
         self.thread_id = None
         self.assistant_id = None
+        self.file_ids = []
         self.prompt = None
         self.system_prompt = None
         self.tools_outputs = None
         self.ctx = None
         self.stream = False
 
     @Slot()
@@ -534,21 +545,23 @@
         try:
             if self.stream:  # stream mode
                 run = self.window.core.gpt.assistants.run_create_stream(
                     self.signals,
                     self.ctx,
                     self.thread_id,
                     self.assistant_id,
+                    self.model,
                     self.system_prompt,
                 )
             else:
                 # not stream mode
                 run = self.window.core.gpt.assistants.run_create(
                     self.thread_id,
                     self.assistant_id,
+                    self.model,
                     self.system_prompt,
                 )
             # handle run (stream or not)
             if run is not None:
                 self.signals.finished.emit(self.ctx, run, self.stream)
                 return True
         except Exception as e:
@@ -561,14 +574,15 @@
 
         :return: result
         """
         try:
             response = self.window.core.gpt.assistants.msg_send(
                 self.thread_id,
                 self.prompt,
+                self.file_ids,
             )
             if response is not None:
                 self.ctx.msg_id = response.id
                 return self.run_create()
         except Exception as e:
             self.signals.error.emit(self.ctx, e)
         return False
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtCore import QObject, Signal, QRunnable, Slot
 
 
@@ -210,15 +210,15 @@
         :return: result
         """
         try:
             # import assistants
             print("Importing assistants...")
             self.window.core.assistants.clear()
             items = self.window.core.assistants.get_all()
-            self.window.core.gpt.assistants.import_assistants(items)
+            self.window.core.gpt.assistants.import_all(items)
             self.window.core.assistants.items = items
             self.window.core.assistants.save()
 
             # import vector stores
             self.import_vector_stores(True)
 
             # import files
@@ -239,15 +239,15 @@
         :param silent: silent mode (no signals)
         :return: result
         """
         try:
             print("Importing vector stores...")
             self.window.core.assistants.store.clear()
             items = {}
-            self.window.core.gpt.assistants.import_vector_stores(items)
+            self.window.core.gpt.store.import_stores(items)
             self.window.core.assistants.store.import_items(items)
             if not silent:
                 self.signals.finished.emit("vector_stores", self.store_id, len(items))
             return True
         except Exception as e:
             print("API error: {}".format(e))
             self.signals.error.emit("vector_stores", e)
@@ -258,15 +258,15 @@
         Truncate all vector stores in API
 
         :param silent: silent mode (no signals)
         :return: result
         """
         try:
             print("Truncating stores...")
-            num = self.window.core.gpt.assistants.vs_truncate_stores()
+            num = self.window.core.gpt.store.remove_all()
             self.window.core.assistants.store.items = {}
             self.window.core.assistants.store.save()
             if not silent:
                 self.signals.finished.emit("truncate_vector_stores", self.store_id, num)
             return True
         except Exception as e:
             print("API error: {}".format(e))
@@ -308,19 +308,19 @@
         :return: result
         """
         try:
             # if empty store_id, truncate all files, otherwise truncate only store files
             if self.store_id is None:
                 print("Truncating all files...")
                 self.window.core.assistants.files.truncate() # clear all files
-                num = self.window.core.gpt.assistants.files_truncate()  # remove all files in API
+                num = self.window.core.gpt.store.remove_files()  # remove all files in API
             else:
                 print("Truncating files for store: {}".format(self.store_id))
                 self.window.core.assistants.files.truncate(self.store_id)  # clear store files, remove from stores and DB
-                num = self.window.core.gpt.assistants.files_truncate_store(self.store_id)  # remove store files in API
+                num = self.window.core.gpt.store.remove_store_files(self.store_id)  # remove store files in API
             if not silent:
                 self.signals.finished.emit("truncate_files", self.store_id, num)
             return True
         except Exception as e:
             print("API error: {}".format(e))
             self.signals.error.emit("truncate_files", e)
             return False
@@ -333,22 +333,22 @@
         :return: result
         """
         num = 0
         try:
             print("Uploading files...")
             for file in self.files:
                 try:
-                    file_id = self.window.core.gpt.assistants.file_upload("", file)
+                    file_id = self.window.core.gpt.store.upload(file)
                     if file_id is not None:
-                        stored_file = self.window.core.gpt.assistants.vs_add_file(
+                        stored_file = self.window.core.gpt.store.add_file(
                             self.store_id,
                             file_id,
                         )
                         if stored_file is not None:
-                            data = self.window.core.gpt.assistants.file_info(file_id)
+                            data = self.window.core.gpt.store.get_file(file_id)
                             self.window.core.assistants.files.insert(self.store_id, data)  # insert to DB
                             self.signals.status.emit("upload_files",
                                                      "Uploaded file: {}/{}".format((num + 1), len(self.files)))
                             num = num + 1
                 except Exception as e:
                     self.window.core.debug.log(e)
                     self.signals.status.emit("upload_files", "Failed to upload file: {}".format(os.path.basename(file)))
@@ -367,19 +367,19 @@
         :param silent: silent mode (no signals)
         :return: result
         """
         try:
             if self.store_id is None:
                 print("Importing all files...")
                 self.window.core.assistants.files.truncate_local()  # clear local DB (all)
-                num = self.window.core.gpt.assistants.vs_import_all_files()  # import all files
+                num = self.window.core.gpt.store.import_stores_files()  # import all files
             else:
                 print("Importing files for store: {}".format(self.store_id))
                 self.window.core.assistants.files.truncate_local(self.store_id)  # clear local DB (all)
-                items = self.window.core.gpt.assistants.vs_import_store_files(self.store_id, [])  # import store files
+                items = self.window.core.gpt.store.import_store_files(self.store_id, [])  # import store files
                 num = len(items)
             if not silent:
                 self.signals.finished.emit("import_files", self.store_id, num)
             return True
         except Exception as e:
             print("API error: {}".format(e))
             self.signals.error.emit("import_files", e)
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.5/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.5/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/assistant_store.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 import copy
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QStandardItemModel, QAction, QIcon
 from PySide6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QScrollArea, QWidget, QTabWidget, QFrame, \
@@ -46,18 +46,23 @@
         :param idx: current model tab index
         """
         self.window.ui.nodes['assistant.store.btn.new'] = \
             QPushButton(trans("dialog.assistant.store.btn.new"))
         self.window.ui.nodes['assistant.store.btn.save'] = \
             QPushButton(trans("dialog.assistant.store.btn.save"))
         self.window.ui.nodes['assistant.store.btn.refresh_status'] = \
-            QPushButton(trans("dialog.assistant.store.btn.refresh_status"))
+            QPushButton(QIcon(":/icons/reload.svg"), "")
         self.window.ui.nodes['assistant.store.btn.close'] = \
             QPushButton(trans("dialog.assistant.store.btn.close"))
 
+        self.window.ui.nodes['assistant.store.btn.refresh_status'].setToolTip(
+            trans("dialog.assistant.store.btn.refresh_status")
+        )
+        self.window.ui.nodes['assistant.store.btn.refresh_status'].setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+
         self.window.ui.nodes['assistant.store.btn.upload.files'] = \
             QPushButton(trans("dialog.assistant.store.btn.upload.files"))
         self.window.ui.nodes['assistant.store.btn.upload.dir'] = \
             QPushButton(trans("dialog.assistant.store.btn.upload.dir"))
 
         self.window.ui.nodes['assistant.store.hide_thread'] = QCheckBox(trans("assistant.store.hide_threads"))
         self.window.ui.nodes['assistant.store.hide_thread'].setChecked(True)
@@ -96,14 +101,15 @@
         # footer buttons
         footer = QHBoxLayout()
         footer.addWidget(self.window.ui.nodes['assistant.store.btn.close'])
         footer.addWidget(self.window.ui.nodes['assistant.store.btn.save'])
 
         # upload buttons
         upload_layout = QHBoxLayout()
+        upload_layout.addWidget(self.window.ui.nodes['assistant.store.btn.refresh_status'])  # reload status btn
         upload_layout.addWidget(self.window.ui.nodes['assistant.store.btn.upload.files'])
         upload_layout.addWidget(self.window.ui.nodes['assistant.store.btn.upload.dir'])
         upload_layout.setContentsMargins(0, 0, 0, 0)
 
         # editor tabs
         self.window.ui.tabs['assistant.store'] = QTabWidget()
 
@@ -148,15 +154,14 @@
                 self.window.ui.groups[group_id].add_layout(option)  # add option to group
 
             # add advanced options group to scroll
             content.addWidget(self.window.ui.groups[group_id])
 
 
         content.addLayout(upload_layout)  # upload buttons
-        content.addWidget(self.window.ui.nodes['assistant.store.btn.refresh_status'])  # reload status btn at the end
         content.setContentsMargins(0, 0, 0, 0)
 
         # scroll widget
         scroll_widget = QWidget()
         scroll_widget.setLayout(content)
         scroll.setWidget(scroll_widget)
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/assistants.py`

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
-# Updated Date: 2024.04.29 16:00:00                  #
+# Updated Date: 2024.04.30 04:00:00                  #
 # ================================================== #
 
 from PySide6 import QtCore
 from PySide6.QtGui import QStandardItemModel, Qt
 from PySide6.QtWidgets import QVBoxLayout, QHBoxLayout, QPushButton, QWidget
 
 from pygpt_net.ui.widget.element.labels import HelpLabel, TitleLabel
@@ -52,15 +52,16 @@
         self.window.ui.nodes['assistants.new'] = QPushButton(trans('assistant.new'))
         self.window.ui.nodes['assistants.new'].clicked.connect(
             lambda: self.window.controller.assistant.editor.edit())
 
         # import
         self.window.ui.nodes['assistants.import'] = QPushButton(trans('assistant.import'))
         self.window.ui.nodes['assistants.import'].clicked.connect(
-            lambda: self.window.controller.assistant.batch.import_all())
+            lambda: self.window.controller.assistant.batch.import_assistants()
+        )
 
         # label
         self.window.ui.nodes['assistants.label'] = TitleLabel(trans("toolbox.assistants.label"))
 
         # header
         header = QHBoxLayout()
         header.addWidget(self.window.ui.nodes['assistants.label'])
```

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.5/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/src/pygpt_net/utils.py` & `pygpt_net-2.2.5/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.4/PKG-INFO` & `pygpt_net-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.4
+Version: 2.2.5
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
 
-Release: **2.2.4** | build: **2024.04.29** | Python: **>=3.10, <3.12**
+Release: **2.2.5** | build: **2024.04.30** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -3126,14 +3126,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.5 (2024-04-30)**
+
+- Fix: import button handler in Assistants.
+- Refactored and improved stores batch actions events handling.
+- Added missing translations.
+
 **2.2.4 (2024-04-29)**
 
 - Batch actions splitted into 'Current store' and 'All stores' in Assistants remote vector stores importer.
 - Added sync current/all context menu options to Sync button.
 - Improved remote stores handling.
 
 **2.2.3 (2024-04-29)**
```

