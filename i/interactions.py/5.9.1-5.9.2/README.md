# Comparing `tmp/interactions.py-5.9.1.tar.gz` & `tmp/interactions.py-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions.py-5.9.1.tar", last modified: Tue Aug  8 16:20:09 2023, max compression
+gzip compressed data, was "interactions.py-5.9.2.tar", last modified: Tue Aug  8 19:13:48 2023, max compression
```

## Comparing `interactions.py-5.9.1.tar` & `interactions.py-5.9.2.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.290357 interactions.py-5.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-08 16:19:19.000000 interactions.py-5.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-08 16:19:19.000000 interactions.py-5.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-08 16:20:09.290357 interactions.py-5.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-08 16:19:19.000000 interactions.py-5.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.206356 interactions.py-5.9.1/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.210356 interactions.py-5.9.1/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.214356 interactions.py-5.9.1/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.222356 interactions.py-5.9.1/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.222356 interactions.py-5.9.1/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.226357 interactions.py-5.9.1/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.230357 interactions.py-5.9.1/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.234356 interactions.py-5.9.1/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.238357 interactions.py-5.9.1/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.242357 interactions.py-5.9.1/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    93178 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.242357 interactions.py-5.9.1/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.246357 interactions.py-5.9.1/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.250357 interactions.py-5.9.1/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.254357 interactions.py-5.9.1/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/debug_extension/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.254357 interactions.py-5.9.1/interactions/ext/hybrid_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/hybrid_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/hybrid_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/hybrid_commands/hybrid_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/hybrid_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.254357 interactions.py-5.9.1/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.258357 interactions.py-5.9.1/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29438 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.258357 interactions.py-5.9.1/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.274357 interactions.py-5.9.1/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   104644 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    31332 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    96566 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38476 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.282357 interactions.py-5.9.1/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.282357 interactions.py-5.9.1/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    57847 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    36926 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.286357 interactions.py-5.9.1/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.286357 interactions.py-5.9.1/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:19:19.000000 interactions.py-5.9.1/interactions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.210356 interactions.py-5.9.1/interactions.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-08 16:20:09.000000 interactions.py-5.9.1/interactions.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-08-08 16:20:09.000000 interactions.py-5.9.1/interactions.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:20:09.000000 interactions.py-5.9.1/interactions.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 16:20:09.000000 interactions.py-5.9.1/interactions.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 16:20:09.000000 interactions.py-5.9.1/interactions.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-08 16:19:19.000000 interactions.py-5.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 16:19:19.000000 interactions.py-5.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 16:20:09.290357 interactions.py-5.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-08 16:19:59.000000 interactions.py-5.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:09.290357 interactions.py-5.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 16:19:19.000000 interactions.py-5.9.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.657027 interactions.py-5.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-08 19:13:05.000000 interactions.py-5.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-08 19:13:05.000000 interactions.py-5.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-08 19:13:48.657027 interactions.py-5.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-08 19:13:05.000000 interactions.py-5.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.597024 interactions.py-5.9.2/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.601024 interactions.py-5.9.2/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.601024 interactions.py-5.9.2/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.605024 interactions.py-5.9.2/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.609025 interactions.py-5.9.2/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.609025 interactions.py-5.9.2/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.617025 interactions.py-5.9.2/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.617025 interactions.py-5.9.2/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.621025 interactions.py-5.9.2/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.621025 interactions.py-5.9.2/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93178 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.625025 interactions.py-5.9.2/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.625025 interactions.py-5.9.2/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.629026 interactions.py-5.9.2/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.629026 interactions.py-5.9.2/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/debug_extension/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.633026 interactions.py-5.9.2/interactions/ext/hybrid_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/hybrid_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/hybrid_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/hybrid_commands/hybrid_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/hybrid_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.633026 interactions.py-5.9.2/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.633026 interactions.py-5.9.2/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29438 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.633026 interactions.py-5.9.2/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.645027 interactions.py-5.9.2/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104644 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31332 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96566 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38476 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.649027 interactions.py-5.9.2/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.649027 interactions.py-5.9.2/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36926 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.653027 interactions.py-5.9.2/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.653027 interactions.py-5.9.2/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:05.000000 interactions.py-5.9.2/interactions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.601024 interactions.py-5.9.2/interactions.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-08 19:13:48.000000 interactions.py-5.9.2/interactions.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-08-08 19:13:48.000000 interactions.py-5.9.2/interactions.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:13:48.000000 interactions.py-5.9.2/interactions.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 19:13:48.000000 interactions.py-5.9.2/interactions.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 19:13:48.000000 interactions.py-5.9.2/interactions.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-08 19:13:05.000000 interactions.py-5.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 19:13:05.000000 interactions.py-5.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 19:13:48.657027 interactions.py-5.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-08 19:13:40.000000 interactions.py-5.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:48.657027 interactions.py-5.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 19:13:05.000000 interactions.py-5.9.2/tests/utils.py
```

### Comparing `interactions.py-5.9.1/LICENSE` & `interactions.py-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/PKG-INFO` & `interactions.py-5.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.9.1
+Version: 5.9.2
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.9.1/README.md` & `interactions.py-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/__init__.py` & `interactions.py-5.9.2/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/__init__.py` & `interactions.py-5.9.2/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/base.py` & `interactions.py-5.9.2/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/discord.py` & `interactions.py-5.9.2/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/internal.py` & `interactions.py-5.9.2/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/__init__.py` & `interactions.py-5.9.2/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/_template.py` & `interactions.py-5.9.2/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/auto_mod.py` & `interactions.py-5.9.2/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/channel_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/guild_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/integrations.py` & `interactions.py-5.9.2/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/member_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/message_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/reaction_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/role_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/scheduled_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/stage_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/thread_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/user_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/events/processors/voice_events.py` & `interactions.py-5.9.2/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/gateway/gateway.py` & `interactions.py-5.9.2/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/gateway/state.py` & `interactions.py-5.9.2/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/gateway/websocket.py` & `interactions.py-5.9.2/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_client.py` & `interactions.py-5.9.2/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/__init__.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/bot.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/channels.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/emojis.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/guild.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/interactions.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/members.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/messages.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/reactions.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/scheduled_events.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/stickers.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/threads.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/users.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/http_requests/webhooks.py` & `interactions.py-5.9.2/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/http/route.py` & `interactions.py-5.9.2/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/audio.py` & `interactions.py-5.9.2/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/audio_writer.py` & `interactions.py-5.9.2/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/encryption.py` & `interactions.py-5.9.2/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/opus.py` & `interactions.py-5.9.2/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/player.py` & `interactions.py-5.9.2/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/recorder.py` & `interactions.py-5.9.2/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/api/voice/voice_gateway.py` & `interactions.py-5.9.2/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/bin/opus-x64.dll` & `interactions.py-5.9.2/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/bin/opus-x86.dll` & `interactions.py-5.9.2/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/__init__.py` & `interactions.py-5.9.2/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/auto_shard_client.py` & `interactions.py-5.9.2/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/client.py` & `interactions.py-5.9.2/interactions/client/client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/const.py` & `interactions.py-5.9.2/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/errors.py` & `interactions.py-5.9.2/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/mixins/modal.py` & `interactions.py-5.9.2/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/mixins/send.py` & `interactions.py-5.9.2/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/mixins/serialization.py` & `interactions.py-5.9.2/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/smart_cache.py` & `interactions.py-5.9.2/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/__init__.py` & `interactions.py-5.9.2/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/attr_converters.py` & `interactions.py-5.9.2/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/attr_utils.py` & `interactions.py-5.9.2/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/attr_utils.pyi` & `interactions.py-5.9.2/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/cache.py` & `interactions.py-5.9.2/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/deserialise_app_cmds.py` & `interactions.py-5.9.2/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/formatting.py` & `interactions.py-5.9.2/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/input_utils.py` & `interactions.py-5.9.2/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/misc_utils.py` & `interactions.py-5.9.2/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/serializer.py` & `interactions.py-5.9.2/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/client/utils/text_utils.py` & `interactions.py-5.9.2/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/console.py` & `interactions.py-5.9.2/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/debug_extension/__init__.py` & `interactions.py-5.9.2/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/debug_extension/debug_application_cmd.py` & `interactions.py-5.9.2/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/debug_extension/debug_exec.py` & `interactions.py-5.9.2/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/debug_extension/debug_exts.py` & `interactions.py-5.9.2/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/debug_extension/utils.py` & `interactions.py-5.9.2/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/hybrid_commands/context.py` & `interactions.py-5.9.2/interactions/ext/hybrid_commands/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/hybrid_commands/hybrid_slash.py` & `interactions.py-5.9.2/interactions/ext/hybrid_commands/hybrid_slash.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/hybrid_commands/manager.py` & `interactions.py-5.9.2/interactions/ext/hybrid_commands/manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/jurigged.py` & `interactions.py-5.9.2/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/mypy/__init__.py` & `interactions.py-5.9.2/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/paginators.py` & `interactions.py-5.9.2/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/__init__.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/command.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/context.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/help.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/manager.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/prefixed_commands/utils.py` & `interactions.py-5.9.2/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/ext/sentry.py` & `interactions.py-5.9.2/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/__init__.py` & `interactions.py-5.9.2/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/__init__.py` & `interactions.py-5.9.2/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/activity.py` & `interactions.py-5.9.2/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/app_perms.py` & `interactions.py-5.9.2/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/application.py` & `interactions.py-5.9.2/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/asset.py` & `interactions.py-5.9.2/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/auto_mod.py` & `interactions.py-5.9.2/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/base.py` & `interactions.py-5.9.2/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/channel.py` & `interactions.py-5.9.2/interactions/models/discord/channel.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/color.py` & `interactions.py-5.9.2/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/components.py` & `interactions.py-5.9.2/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/embed.py` & `interactions.py-5.9.2/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/emoji.py` & `interactions.py-5.9.2/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/enums.py` & `interactions.py-5.9.2/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/file.py` & `interactions.py-5.9.2/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/guild.py` & `interactions.py-5.9.2/interactions/models/discord/guild.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/invite.py` & `interactions.py-5.9.2/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/message.py` & `interactions.py-5.9.2/interactions/models/discord/message.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/modal.py` & `interactions.py-5.9.2/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/reaction.py` & `interactions.py-5.9.2/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/role.py` & `interactions.py-5.9.2/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/scheduled_event.py` & `interactions.py-5.9.2/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/snowflake.py` & `interactions.py-5.9.2/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/stage_instance.py` & `interactions.py-5.9.2/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/sticker.py` & `interactions.py-5.9.2/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/team.py` & `interactions.py-5.9.2/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/thread.py` & `interactions.py-5.9.2/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/timestamp.py` & `interactions.py-5.9.2/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/user.py` & `interactions.py-5.9.2/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/user.pyi` & `interactions.py-5.9.2/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/voice_state.py` & `interactions.py-5.9.2/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/discord/webhooks.py` & `interactions.py-5.9.2/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/__init__.py` & `interactions.py-5.9.2/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/active_voice_state.py` & `interactions.py-5.9.2/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/annotations/slash.py` & `interactions.py-5.9.2/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/application_commands.py` & `interactions.py-5.9.2/interactions/models/internal/application_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1166,28 +1166,27 @@
 
         If you do not supply a `custom_id`, the name of the coroutine will be used instead.
 
     Args:
         *custom_id: The custom ID of the component to wait for
 
     """
-    resolved_custom_id: tuple[str | re.Pattern, ...] | list[str] = []
 
     def wrapper(func: AsyncCallable) -> ComponentCommand:
         resolved_custom_id = custom_id or [func.__name__]
 
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ComponentCommand(
             name=f"ComponentCallback::{resolved_custom_id}", callback=func, listeners=resolved_custom_id
         )
 
-    custom_id = _unpack_helper(resolved_custom_id)
-    custom_ids_validator(*resolved_custom_id)
+    custom_id = _unpack_helper(custom_id)
+    custom_ids_validator(*custom_id)
     return wrapper
 
 
 def modal_callback(*custom_id: str | re.Pattern) -> Callable[[AsyncCallable], ModalCommand]:
     """
     Register a coroutine as a modal callback.
 
@@ -1199,26 +1198,25 @@
 
         If you do not supply a `custom_id`, the name of the coroutine will be used instead.
 
 
     Args:
         *custom_id: The custom ID of the modal to wait for
     """
-    resolved_custom_id: tuple[str | re.Pattern, ...] | list[str] = []
 
     def wrapper(func: AsyncCallable) -> ModalCommand:
         resolved_custom_id = custom_id or [func.__name__]
 
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ModalCommand(name=f"ModalCallback::{resolved_custom_id}", callback=func, listeners=resolved_custom_id)
 
-    custom_id = _unpack_helper(resolved_custom_id)
-    custom_ids_validator(*resolved_custom_id)
+    custom_id = _unpack_helper(custom_id)
+    custom_ids_validator(*custom_id)
     return wrapper
 
 
 InterCommandT = TypeVar("InterCommandT", InteractionCommand, AsyncCallable)
 SlashCommandT = TypeVar("SlashCommandT", SlashCommand, AsyncCallable)
```

### Comparing `interactions.py-5.9.1/interactions/models/internal/auto_defer.py` & `interactions.py-5.9.2/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/callback.py` & `interactions.py-5.9.2/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/checks.py` & `interactions.py-5.9.2/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/command.py` & `interactions.py-5.9.2/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/context.py` & `interactions.py-5.9.2/interactions/models/internal/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/converters.py` & `interactions.py-5.9.2/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/cooldowns.py` & `interactions.py-5.9.2/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/extension.py` & `interactions.py-5.9.2/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/listener.py` & `interactions.py-5.9.2/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/localisation.py` & `interactions.py-5.9.2/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/protocols.py` & `interactions.py-5.9.2/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/tasks/task.py` & `interactions.py-5.9.2/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/tasks/triggers.py` & `interactions.py-5.9.2/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/internal/wait.py` & `interactions.py-5.9.2/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/misc/context_manager.py` & `interactions.py-5.9.2/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions/models/misc/iterator.py` & `interactions.py-5.9.2/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions.py.egg-info/PKG-INFO` & `interactions.py-5.9.2/interactions.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.9.1
+Version: 5.9.2
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.9.1/interactions.py.egg-info/SOURCES.txt` & `interactions.py-5.9.2/interactions.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/interactions.py.egg-info/requires.txt` & `interactions.py-5.9.2/interactions.py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/pyproject.toml` & `interactions.py-5.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.9.1"
+version = "5.9.2"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `interactions.py-5.9.1/setup.py` & `interactions.py-5.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/consts.py` & `interactions.py-5.9.2/tests/consts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/test_bot.py` & `interactions.py-5.9.2/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/test_cache.py` & `interactions.py-5.9.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/test_contexts.py` & `interactions.py-5.9.2/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/test_cooldowns.py` & `interactions.py-5.9.2/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/test_emoji.py` & `interactions.py-5.9.2/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.9.1/tests/utils.py` & `interactions.py-5.9.2/tests/utils.py`

 * *Files identical despite different names*

