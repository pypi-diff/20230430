# Comparing `tmp/interactions.py-5.1.0.tar.gz` & `tmp/interactions.py-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions.py-5.1.0.tar", last modified: Sat Apr 22 06:01:32 2023, max compression
+gzip compressed data, was "interactions.py-5.2.0.tar", last modified: Sun Apr 30 10:06:52 2023, max compression
```

## Comparing `interactions.py-5.1.0.tar` & `interactions.py-5.2.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.968174 interactions.py-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-22 06:00:58.000000 interactions.py-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-22 06:00:58.000000 interactions.py-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-22 06:01:32.968174 interactions.py-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-22 06:00:58.000000 interactions.py-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22791 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88115 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   102171 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30028 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    95041 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    37369 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55399 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-22 06:00:58.000000 interactions.py-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 06:00:58.000000 interactions.py-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-22 06:01:32.968174 interactions.py-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-22 06:01:26.000000 interactions.py-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.968174 interactions.py-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.122444 interactions.py-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-30 10:06:02.000000 interactions.py-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 10:06:02.000000 interactions.py-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-30 10:06:52.122444 interactions.py-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-30 10:06:02.000000 interactions.py-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.070445 interactions.py-5.2.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.074445 interactions.py-5.2.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.074445 interactions.py-5.2.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.082445 interactions.py-5.2.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.086445 interactions.py-5.2.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.086445 interactions.py-5.2.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.094445 interactions.py-5.2.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.098445 interactions.py-5.2.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.098445 interactions.py-5.2.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.102445 interactions.py-5.2.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88416 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.102445 interactions.py-5.2.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.106445 interactions.py-5.2.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.114445 interactions.py-5.2.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102768 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30028 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37383 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.118445 interactions.py-5.2.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.118445 interactions.py-5.2.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55413 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.118445 interactions.py-5.2.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.118445 interactions.py-5.2.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 interactions.py-5.2.0/interactions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.074445 interactions.py-5.2.0/interactions.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-30 10:06:52.000000 interactions.py-5.2.0/interactions.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-30 10:06:52.000000 interactions.py-5.2.0/interactions.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:06:52.000000 interactions.py-5.2.0/interactions.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 10:06:52.000000 interactions.py-5.2.0/interactions.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 10:06:52.000000 interactions.py-5.2.0/interactions.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-30 10:06:02.000000 interactions.py-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-30 10:06:02.000000 interactions.py-5.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-30 10:06:52.122444 interactions.py-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-30 10:06:42.000000 interactions.py-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:52.122444 interactions.py-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-30 10:06:02.000000 interactions.py-5.2.0/tests/utils.py
```

### Comparing `interactions.py-5.1.0/LICENSE` & `interactions.py-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/PKG-INFO` & `interactions.py-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.1.0
+Version: 5.2.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.1.0/README.md` & `interactions.py-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/__init__.py` & `interactions.py-5.2.0/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/__init__.py` & `interactions.py-5.2.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/base.py` & `interactions.py-5.2.0/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/discord.py` & `interactions.py-5.2.0/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/internal.py` & `interactions.py-5.2.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/__init__.py` & `interactions.py-5.2.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/_template.py` & `interactions.py-5.2.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/auto_mod.py` & `interactions.py-5.2.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/channel_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/guild_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/integrations.py` & `interactions.py-5.2.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/member_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/message_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/reaction_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/role_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/stage_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/thread_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/user_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/events/processors/voice_events.py` & `interactions.py-5.2.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/gateway/gateway.py` & `interactions.py-5.2.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/gateway/state.py` & `interactions.py-5.2.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/gateway/websocket.py` & `interactions.py-5.2.0/interactions/api/gateway/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             data: The data to send
             bypass: Should the rate limit be ignored for this send (used for heartbeats)
 
         """
         serialized = FastJson.dumps(data)
         await self.send(serialized, bypass)
 
-    async def receive(self, force: bool = False) -> str:
+    async def receive(self, force: bool = False) -> str:  # noqa: C901
         """
         Receive a full event payload from the WebSocket.
 
         Args:
             force:
                 Whether to force the receiving, ignoring safety measures such as the read-lock.
                 This option also means that exceptions are raised when a reconnection would normally
```

### Comparing `interactions.py-5.1.0/interactions/api/http/http_client.py` & `interactions.py-5.2.0/interactions/api/http/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                 )
         if attachments:
             payload["attachments"] = attachments
 
         form_data.add_field("payload_json", FastJson.dumps(payload))
         return form_data
 
-    async def request(
+    async def request(  # noqa: C901
         self,
         route: Route,
         payload: list | dict | None = None,
         files: list[UPLOADABLE_TYPE] | None = None,
         reason: str | None = None,
         params: dict | None = None,
         **kwargs: dict,
@@ -399,52 +399,52 @@
                                     f"Bot has exceeded global ratelimit, locking REST API for {result['retry_after']} seconds",
                                 )
                                 self.global_lock.set_reset_time(float(result["retry_after"]))
                             elif result.get("message") == "The resource is being rate limited.":
                                 # resource ratelimit is reached
                                 self.log_ratelimit(
                                     self.logger.warning,
-                                    f"{route.endpoint} The resource is being rate limited! "
+                                    f"{route.resolved_endpoint} The resource is being rate limited! "
                                     f"Reset in {result.get('retry_after')} seconds",
                                 )
                                 # lock this resource and wait for unlock
                                 await lock.lock_for_duration(float(result["retry_after"]), block=True)
                             else:
                                 # endpoint ratelimit is reached
                                 # 429's are unfortunately unavoidable, but we can attempt to avoid them
                                 # so long as these are infrequent we're doing well
                                 self.log_ratelimit(
                                     self.logger.warning,
-                                    f"{route.endpoint} Has exceeded it's ratelimit ({lock.limit})! Reset in {lock.delta} seconds",
+                                    f"{route.resolved_endpoint} Has exceeded its ratelimit ({lock.limit})! Reset in {lock.delta} seconds",
                                 )
                                 await lock.lock_for_duration(lock.delta, block=True)
                             continue
                         if lock.remaining == 0:
                             # Last call available in the bucket, lock until reset
                             self.log_ratelimit(
                                 self.logger.debug,
-                                f"{route.endpoint} Has exhausted its ratelimit ({lock.limit})! Locking route for {lock.delta} seconds",
+                                f"{route.resolved_endpoint} Has exhausted its ratelimit ({lock.limit})! Locking route for {lock.delta} seconds",
                             )
                             await lock.lock_for_duration(
                                 lock.delta
                             )  # lock this route, but continue processing the current response
 
                         elif response.status in {500, 502, 504}:
                             # Server issues, retry
                             self.logger.warning(
-                                f"{route.endpoint} Received {response.status}... retrying in {1 + attempt * 2} seconds"
+                                f"{route.resolved_endpoint} Received {response.status}... retrying in {1 + attempt * 2} seconds"
                             )
                             await asyncio.sleep(1 + attempt * 2)
                             continue
 
                         if not 300 > response.status >= 200:
                             await self._raise_exception(response, route, result)
 
                         self.logger.debug(
-                            f"{route.endpoint} Received {response.status} :: [{lock.remaining}/{lock.limit} calls remaining]"
+                            f"{route.resolved_endpoint} Received {response.status} :: [{lock.remaining}/{lock.limit} calls remaining]"
                         )
                         return result
                 except OSError as e:
                     if attempt < self._max_attempts - 1 and e.errno in (54, 10054):
                         await asyncio.sleep(1 + attempt * 2)
                         continue
                     raise
```

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/__init__.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/bot.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/channels.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
             "invite_code": invite_code,
             "with_counts": with_counts,
             "with_expiration": with_expiration,
             "guild_scheduled_event_id": int(scheduled_event_id) if scheduled_event_id else None,
         }
         params = dict_filter_none(params)
 
-        result = await self.request(Route("GET", "/invites/{invite_code}", params=params))
+        result = await self.request(Route("GET", "/invites/{invite_code}", invite_code=invite_code, params=params))
         return cast(discord_typings.InviteData, result)
 
     async def delete_invite(self, invite_code: str, reason: str | None = None) -> discord_typings.InviteData:
         """
         Delete an invite.
 
         Args:
```

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/emojis.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/guild.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/interactions.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/members.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/messages.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/reactions.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/scheduled_events.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/stickers.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/threads.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/threads.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,34 +176,40 @@
     async def create_thread(
         self,
         channel_id: "Snowflake_Type",
         name: str,
         auto_archive_duration: int,
         thread_type: Absent[int] = MISSING,
         invitable: Absent[bool] = MISSING,
+        rate_limit_per_user: Absent[int] = MISSING,
         message_id: Absent["Snowflake_Type"] = MISSING,
         reason: Absent[str] = MISSING,
     ) -> discord_typings.ThreadChannelData:
         """
         Create a thread in the given channel. Can either create a thread with or without a message.
 
         Args:
             channel_id: The ID of the channel to create this thread in
             name: The name of the thread
             auto_archive_duration: duration in minutes to automatically archive the thread after recent activity, can be set to: 60, 1440, 4320, 10080
             thread_type: The type of thread, defaults to public. ignored if creating thread from a message
-            invitable:
+            invitable: Whether non-moderators can add other non-moderators to a thread; only available when creating a private thread
+            rate_limit_per_user: The time users must wait between sending messages (0-21600)
             message_id: An optional message to create a thread from.
             reason: An optional reason for the audit log
 
         Returns:
             The created thread
 
         """
-        payload = {"name": name, "auto_archive_duration": auto_archive_duration}
+        payload = {
+            "name": name,
+            "auto_archive_duration": auto_archive_duration,
+            "rate_limit_per_user": rate_limit_per_user,
+        }
         if message_id:
             return await self.request(
                 Route(
                     "POST",
                     "/channels/{channel_id}/messages/{message_id}/threads",
                     channel_id=channel_id,
                     message_id=message_id,
```

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/users.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/http_requests/webhooks.py` & `interactions.py-5.2.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/http/route.py` & `interactions.py-5.2.0/interactions/api/http/route.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,17 +52,39 @@
             return self.known_bucket
 
         if self.webhook_token:
             return f"{self.webhook_id}{self.webhook_token}:{self.channel_id}:{self.guild_id}:{self.endpoint}"
         return f"{self.channel_id}:{self.guild_id}:{self.endpoint}"
 
     @property
+    def major_params(self) -> dict[str, str | int]:
+        """The major parameters for this route"""
+        return {
+            "channel_id": self.channel_id,
+            "guild_id": self.guild_id,
+            "webhook_id": self.webhook_id,
+            "webhook_token": self.webhook_token,
+        }
+
+    @property
+    def resolved_path(self) -> str:
+        """The endpoint for this route, with all parameters resolved"""
+        return self.path.format_map({k: _uriquote(v) if isinstance(v, str) else v for k, v in self.params.items()})
+
+    @property
     def endpoint(self) -> str:
         """The endpoint for this route"""
         return f"{self.method} {self.path}"
 
     @property
+    def resolved_endpoint(self) -> str:
+        """The endpoint for this route, with all major parameters resolved"""
+        path = self.path
+        for key, value in self.major_params.items():
+            path = path.replace(f"{{{key}}}", str(value))
+
+        return f"{self.method} {path}"
+
+    @property
     def url(self) -> str:
         """The full url for this route"""
-        return f"{self.BASE}{self.path}".format_map(
-            {k: _uriquote(v) if isinstance(v, str) else v for k, v in self.params.items()}
-        )
+        return f"{self.BASE}{self.resolved_path}"
```

### Comparing `interactions.py-5.1.0/interactions/api/voice/audio.py` & `interactions.py-5.2.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/audio_writer.py` & `interactions.py-5.2.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/encryption.py` & `interactions.py-5.2.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/opus.py` & `interactions.py-5.2.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/player.py` & `interactions.py-5.2.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/recorder.py` & `interactions.py-5.2.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/api/voice/voice_gateway.py` & `interactions.py-5.2.0/interactions/api/voice/voice_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 self.sequence = seq
 
             # This may try to reconnect the connection so it is best to wait
             # for it to complete before receiving more - that way there's less
             # possible race conditions to consider.
             await self.dispatch_opcode(data, op)
 
-    async def receive(self, force=False) -> str:
+    async def receive(self, force=False) -> str:  # noqa: C901
         buffer = bytearray()
 
         while True:
             if not force:
                 await self._closed.wait()
 
             resp = await self.ws.receive()
```

### Comparing `interactions.py-5.1.0/interactions/bin/opus-x64.dll` & `interactions.py-5.2.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/bin/opus-x86.dll` & `interactions.py-5.2.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/__init__.py` & `interactions.py-5.2.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/auto_shard_client.py` & `interactions.py-5.2.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/client.py` & `interactions.py-5.2.0/interactions/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1594,20 +1594,22 @@
             cmd_id: The ID of the command
             scope: Optionally specify a scope to search in
 
         Returns:
             The command, if one with the given ID exists internally, otherwise None
 
         """
+        cmd_id = to_snowflake(cmd_id)
+        scope = to_snowflake(scope) if scope is not None else None
+
         if scope is not None:
-            return self.interactions_by_scope.get(scope, {}).get(cmd_id)
-        return next(
-            (scope[cmd_id] for scope in self.interactions_by_scope.values() if cmd_id in scope),
-            None,
-        )
+            return next(
+                (cmd for cmd in self.interactions_by_scope[scope].values() if cmd.get_cmd_id(scope) == cmd_id), None
+            )
+        return next(cmd for cmd in self._interaction_lookup.values() if cmd_id in cmd.cmd_id.values())
 
     def _raise_sync_exception(self, e: HTTPException, cmds_json: dict, cmd_scope: "Snowflake_Type") -> NoReturn:
         try:
             if isinstance(e.errors, dict):
                 for cmd_num in e.errors.keys():
                     cmd = cmds_json[cmd_scope][int(cmd_num)]
                     output = e.search_for_message(e.errors[cmd_num], cmd)
@@ -1687,24 +1689,28 @@
         return cls
 
     async def _run_slash_command(self, command: SlashCommand, ctx: "InteractionContext") -> Any:
         """Overrideable method that executes slash commands, can be used to wrap callback execution"""
         return await command(ctx, **ctx.kwargs)
 
     @processors.Processor.define("raw_interaction_create")
-    async def _dispatch_interaction(self, event: RawGatewayEvent) -> None:
+    async def _dispatch_interaction(self, event: RawGatewayEvent) -> None:  # noqa: C901
         """
         Identify and dispatch interaction of slash commands or components.
 
         Args:
             raw interaction event
 
         """
         interaction_data = event.data
 
+        if not self._startup:
+            self.logger.warning("Received interaction before startup completed, ignoring")
+            return
+
         if interaction_data["type"] in (
             InteractionType.APPLICATION_COMMAND,
             InteractionType.AUTOCOMPLETE,
         ):
             interaction_id = interaction_data["data"]["id"]
             name = interaction_data["data"]["name"]
```

### Comparing `interactions.py-5.1.0/interactions/client/const.py` & `interactions.py-5.2.0/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/errors.py` & `interactions.py-5.2.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/mixins/modal.py` & `interactions.py-5.2.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/mixins/send.py` & `interactions.py-5.2.0/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/mixins/serialization.py` & `interactions.py-5.2.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/smart_cache.py` & `interactions.py-5.2.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/__init__.py` & `interactions.py-5.2.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/attr_converters.py` & `interactions.py-5.2.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/attr_utils.py` & `interactions.py-5.2.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/attr_utils.pyi` & `interactions.py-5.2.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/cache.py` & `interactions.py-5.2.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/deserialise_app_cmds.py` & `interactions.py-5.2.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/formatting.py` & `interactions.py-5.2.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/input_utils.py` & `interactions.py-5.2.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/misc_utils.py` & `interactions.py-5.2.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/serializer.py` & `interactions.py-5.2.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/client/utils/text_utils.py` & `interactions.py-5.2.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/console.py` & `interactions.py-5.2.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/debug_extension/__init__.py` & `interactions.py-5.2.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/debug_extension/debug_application_cmd.py` & `interactions.py-5.2.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,19 @@
                     file=File(
                         io.BytesIO(pprint.pformat(cmd_json, 2).encode("utf-8")),
                         f"{cmd_json.get('name')}.json",
                     )
                 )
 
             if not remote:
-                data = application_commands_to_dict(self.bot.interactions, self.bot)[scope]
+                data = application_commands_to_dict(self.bot.interactions_by_scope, self.bot)[scope]
                 cmd_obj = self.bot.get_application_cmd_by_id(cmd_id)
-                for cmd in data:
-                    if cmd["name"] == cmd_obj.name:
-                        return await send(cmd)
-
+                cmd_data = next((c for c in data if c["name"] == str(cmd_obj.name)), None)
+                if cmd_data:
+                    return await send(cmd_data)
             else:
                 data = await self.bot.http.get_application_commands(self.bot.app.id, scope)
                 try:
                     perm_scope = scope
                     if scope == GLOBAL_SCOPE:
                         perm_scope = ctx.guild_id
                     perms = await self.bot.http.get_application_command_permissions(self.bot.app.id, perm_scope, cmd_id)
```

### Comparing `interactions.py-5.1.0/interactions/ext/debug_extension/debug_exec.py` & `interactions.py-5.2.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,23 +39,21 @@
             "author": ctx.author,
             "server": ctx.guild,
             "guild": ctx.guild,
             "message": ctx.message,
         } | globals()
 
         modal = Modal(
+            ParagraphText(
+                label="Code to run",
+                value=last_code,
+                custom_id="body",
+                placeholder="Write your code here!",
+            ),
             title="Debug-Exec",
-            components=[
-                ParagraphText(
-                    label="Code to run",
-                    value=last_code,
-                    custom_id="body",
-                    placeholder="Write your code here!",
-                )
-            ],
         )
         await ctx.send_modal(modal)
 
         m_ctx = await self.bot.wait_for_modal(modal, ctx.author)
         await m_ctx.defer()
 
         body = m_ctx.kwargs["body"]
@@ -91,35 +89,35 @@
         else:
             paginator = Paginator.create_from_string(self.bot, body, prefix="```py", suffix="```", page_size=4000)
             await paginator.send(ctx)
 
         if result is None:
             result = value or "No Output!"
 
-        if isinstance(result, Message):
+        elif isinstance(result, Message):
             try:
                 e = debug_embed("Exec", timestamp=result.created_at, url=result.jump_url)
                 e.description = result.content
                 e.set_author(
                     result.author.tag,
                     icon_url=(result.author.guild_avatar or result.author.avatar).url,
                 )
                 e.add_field("\u200b", f"[Jump To]({result.jump_url})\n{result.channel.mention}")
 
                 return await ctx.send(embeds=e)
             except Exception:
                 return await ctx.send(result.jump_url)
 
-        if isinstance(result, Embed):
+        elif isinstance(result, Embed):
             return await ctx.send(embeds=[result])
 
-        if isinstance(result, File):
+        elif isinstance(result, File):
             return await ctx.send(file=result)
 
-        if isinstance(result, Paginator):
+        elif isinstance(result, Paginator):
             return await result.send(ctx)
 
         if hasattr(result, "__iter__"):
             l_result = list(result)
             if all(isinstance(r, Embed) for r in result):
                 paginator = Paginator.create_from_embeds(self.bot, *l_result)
                 return await paginator.send(ctx)
```

### Comparing `interactions.py-5.1.0/interactions/ext/debug_extension/debug_exts.py` & `interactions.py-5.2.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/debug_extension/utils.py` & `interactions.py-5.2.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/jurigged.py` & `interactions.py-5.2.0/interactions/ext/jurigged.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from pathlib import Path
 from types import ModuleType
 from typing import Callable, Dict
 
-from interactions import Extension, SlashCommand
+from interactions import Extension, SlashCommand, Client
 from interactions.client.errors import ExtensionLoadException, ExtensionNotFound
 from interactions.client.utils.misc_utils import find
 from interactions.client.const import get_logger
 
 try:
     from jurigged import watch, CodeFile
     from jurigged.live import WatchOperation
@@ -51,23 +51,27 @@
             exts.append(val)
         commands[f"{module.__name__}"] = exts
 
     return {k: v for k, v in commands.items() if v is not None}
 
 
 class Jurigged(Extension):
+    def __init__(self, *_, poll=False) -> None:
+        self.poll = poll
+        self.command_cache = {}
+        self.watcher = None
+
     async def async_start(self) -> None:
         """Jurigged starting utility."""
-        self.command_cache = {}
         self.bot.logger.warning("Setting sync_ext to True by default for syncing changes")
         self.bot.sync_ext = True
 
         self.bot.logger.info("Loading jurigged")
         path = Path().resolve()
-        self.watcher = watch(f"{path}/[!.]*.py", logger=self.jurigged_log)
+        self.watcher = watch(f"{path}/[!.]*.py", logger=self.jurigged_log, poll=self.poll)
         self.watcher.prerun.register(self.jurigged_prerun)
         self.watcher.postrun.register(self.jurigged_postrun)
 
     def jurigged_log(self, event: WatchOperation | AddOperation | DeleteOperation | UpdateOperation) -> None:
         """
         Log a jurigged event
 
@@ -108,15 +112,15 @@
             _path: Path to file
             cf: File information
         """
         if self.bot.get_ext(cf.module_name):
             self.bot.logger.debug(f"Caching {cf.module_name}")
             self.command_cache = get_all_commands(cf.module)
 
-    def jurigged_postrun(self, _path: str, cf: CodeFile) -> None:
+    def jurigged_postrun(self, _path: str, cf: CodeFile) -> None:  # noqa: C901
         """
         Jurigged postrun event.
 
         Args:
             _path: Path to file
             cf: File information
         """
@@ -199,9 +203,12 @@
                         except Exception:
                             self.bot.logger.exception(f"Failed to update module {module}", exc_info=True)
                     else:
                         self.bot.logger.debug("No changes detected")
         self.command_cache.clear()
 
 
-def setup(bot) -> None:
-    Jurigged(bot)
+def setup(
+    bot: Client,
+    poll: bool = False,
+) -> None:
+    Jurigged(bot, poll=poll)
```

### Comparing `interactions.py-5.1.0/interactions/ext/mypy/__init__.py` & `interactions.py-5.2.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/paginators.py` & `interactions.py-5.2.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/__init__.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/command.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         return " ".join(results)
 
     @property
     def is_subcommand(self) -> bool:
         """Return whether this command is a subcommand or not."""
         return bool(self.parent)
 
-    def _parse_parameters(self) -> None:
+    def _parse_parameters(self) -> None:  # noqa: C901
         """
         Parses the parameters that this command has into a form i.py can use.
 
         This is purposely separated like this to allow "lazy parsing" - parsing
         as the command is added to a bot rather than being parsed immediately.
         This allows variables like "self" to be filtered out, and is useful for
         potential future additions.
@@ -664,15 +664,15 @@
                 checks=self.checks if inherit_checks else [],
             )
             self.add_command(cmd)
             return cmd
 
         return wrapper
 
-    async def call_callback(self, callback: Callable, ctx: "PrefixedContext") -> None:
+    async def call_callback(self, callback: Callable, ctx: "PrefixedContext") -> None:  # noqa: C901
         """
         Runs the callback of this command.
 
         Args:
             callback (Callable: The callback to run. This is provided for compatibility with internal.
             ctx (internal.MessageContext): The context to use for this command.
         """
```

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/context.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/help.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/manager.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     @listen("extension_unload")
     async def _handle_ext_unload(self, event: ExtensionUnload) -> None:
         """Unregisters all prefixed commands in an extension as it is being unloaded."""
         for name in self._ext_command_list[event.extension.extension_name]:
             self.remove_command(name)
 
     @listen("raw_message_create", is_default_listener=True)
-    async def _dispatch_prefixed_commands(self, event: RawGatewayEvent) -> None:
+    async def _dispatch_prefixed_commands(self, event: RawGatewayEvent) -> None:  # noqa: C901
         """Determine if a prefixed command is being triggered, and dispatch it."""
         # don't waste time processing this if there are no prefixed commands
         if not self.commands:
             return
 
         data = event.data
```

### Comparing `interactions.py-5.1.0/interactions/ext/prefixed_commands/utils.py` & `interactions.py-5.2.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/ext/sentry.py` & `interactions.py-5.2.0/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/__init__.py` & `interactions.py-5.2.0/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/__init__.py` & `interactions.py-5.2.0/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/activity.py` & `interactions.py-5.2.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/app_perms.py` & `interactions.py-5.2.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/application.py` & `interactions.py-5.2.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/asset.py` & `interactions.py-5.2.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/auto_mod.py` & `interactions.py-5.2.0/interactions/models/discord/auto_mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,15 @@
     AutoModAction,
     AutoModEvent,
     AutoModLanuguageType,
 )
 from interactions.models.discord.snowflake import to_snowflake_list, to_snowflake
 
 if TYPE_CHECKING:
-    from interactions import (
-        Snowflake_Type,
-        Guild,
-        GuildText,
-        Message,
-        Client,
-        Member,
-    )
+    from interactions import Snowflake_Type, Guild, GuildText, Message, Client, Member, User
 
 __all__ = ("AutoModerationAction", "AutoModRule")
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class BaseAction(DictSerializationMixin):
     """
@@ -315,14 +308,15 @@
 
     _message_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
     _alert_system_message_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
     _channel_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
     _guild_id: "Snowflake_Type" = attrs.field(
         repr=False,
     )
+    _user_id: "Snowflake_Type" = attrs.field(repr=False)
 
     @classmethod
     def _process_dict(cls, data: dict, client: "Client") -> dict:
         data = super()._process_dict(data, client)
         data["action"] = BaseAction.from_dict_factory(data["action"])
         return data
 
@@ -334,14 +328,22 @@
     def channel(self) -> "Optional[GuildText]":
         return self._client.get_channel(self._channel_id)
 
     @property
     def message(self) -> "Optional[Message]":
         return self._client.cache.get_message(self._channel_id, self._message_id)
 
+    @property
+    def user(self) -> "User":
+        return self._client.cache.get_user(self._user_id)
+
+    @property
+    def member(self) -> "Optional[Member]":
+        return self._client.cache.get_member(self._guild_id, self._user_id)
+
 
 ACTION_MAPPING = {
     AutoModAction.BLOCK_MESSAGE: BlockMessage,
     AutoModAction.ALERT_MESSAGE: AlertMessage,
     AutoModAction.TIMEOUT_USER: TimeoutUser,
 }
```

### Comparing `interactions.py-5.1.0/interactions/models/discord/base.py` & `interactions.py-5.2.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/channel.py` & `interactions.py-5.2.0/interactions/models/discord/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,25 +552,27 @@
 class ThreadableMixin:
     async def create_thread(
         self,
         name: str,
         message: Absent[Snowflake_Type] = MISSING,
         thread_type: Absent[ChannelType] = MISSING,
         invitable: Absent[bool] = MISSING,
+        rate_limit_per_user: Absent[int] = MISSING,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
         reason: Absent[str] = None,
     ) -> "TYPE_THREAD_CHANNEL":
         """
         Creates a new thread in this channel. If a message is provided, it will be used as the initial message.
 
         Args:
             name: 1-100 character thread name
             message: The message to connect this thread to. Required for news channel.
             thread_type: Is the thread private or public. Not applicable to news channel, it will always be GUILD_NEWS_THREAD.
             invitable: whether non-moderators can add other non-moderators to a thread. Only applicable when creating a private thread.
+            rate_limit_per_user: The time users must wait between sending messages (0-21600).
             auto_archive_duration: Time before the thread will be automatically archived. Note 3 day and 7 day archive durations require the server to be boosted.
             reason: The reason for creating this thread.
 
         Returns:
             The created thread, if successful
 
         """
@@ -584,14 +586,15 @@
             raise ValueError("Invitable only applies to private threads.")
 
         thread_data = await self._client.http.create_thread(
             channel_id=self.id,
             name=name,
             thread_type=thread_type,
             invitable=invitable,
+            rate_limit_per_user=rate_limit_per_user,
             auto_archive_duration=auto_archive_duration,
             message_id=to_optional_snowflake(message),
             reason=reason,
         )
         return self._client.cache.place_channel_data(thread_data)
 
     async def fetch_public_archived_threads(
@@ -1736,59 +1739,65 @@
             **kwargs,
         )
 
     async def create_public_thread(
         self,
         name: str,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
+        rate_limit_per_user: Absent[int] = MISSING,
         reason: Absent[str] = None,
     ) -> "GuildPublicThread":
         """
         Creates a new public thread in this channel.
 
         Args:
             name: 1-100 character thread name.
             auto_archive_duration: Time before the thread will be automatically archived. Note 3 day and 7 day archive durations require the server to be boosted.
+            rate_limit_per_user: The time users must wait between sending messages (0-21600).
             reason: The reason for creating this thread.
 
         Returns:
             The created public thread, if successful
 
         """
         return await self.create_thread(
             name=name,
             thread_type=ChannelType.GUILD_PUBLIC_THREAD,
             auto_archive_duration=auto_archive_duration,
+            rate_limit_per_user=rate_limit_per_user,
             reason=reason,
         )
 
     async def create_private_thread(
         self,
         name: str,
         invitable: Absent[bool] = MISSING,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
+        rate_limit_per_user: Absent[int] = MISSING,
         reason: Absent[str] = None,
     ) -> "GuildPrivateThread":
         """
         Creates a new private thread in this channel.
 
         Args:
             name: 1-100 character thread name.
-            invitable: whether non-moderators can add other non-moderators to a thread.
+            invitable: Whether non-moderators can add other non-moderators to a thread.
+            rate_limit_per_user: The time users must wait between sending messages (0-21600).
             auto_archive_duration: Time before the thread will be automatically archived. Note 3 day and 7 day archive durations require the server to be boosted.
             reason: The reason for creating this thread.
 
         Returns:
             The created thread, if successful
 
         """
         return await self.create_thread(
             name=name,
             thread_type=ChannelType.GUILD_PRIVATE_THREAD,
             invitable=invitable,
+            rate_limit_per_user=rate_limit_per_user,
             auto_archive_duration=auto_archive_duration,
             reason=reason,
         )
 
     async def create_thread_from_message(
         self,
         name: str,
```

### Comparing `interactions.py-5.1.0/interactions/models/discord/color.py` & `interactions.py-5.2.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/components.py` & `interactions.py-5.2.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/embed.py` & `interactions.py-5.2.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/emoji.py` & `interactions.py-5.2.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/enums.py` & `interactions.py-5.2.0/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/file.py` & `interactions.py-5.2.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/guild.py` & `interactions.py-5.2.0/interactions/models/discord/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -1660,14 +1660,15 @@
             reason: The reason for the ban
 
         """
         if delete_message_days is not MISSING:
             warn(
                 "delete_message_days is deprecated and will be removed in a future update",
                 DeprecationWarning,
+                stacklevel=2,
             )
             delete_message_seconds = delete_message_days * 3600
         await self._client.http.create_guild_ban(self.id, to_snowflake(user), delete_message_seconds, reason=reason)
 
     async def fetch_ban(self, user: Union["models.User", "models.Member", Snowflake_Type]) -> Optional[GuildBan]:
         """
         Fetches the ban information for the specified user in the guild. You must have the `ban members` permission.
```

### Comparing `interactions.py-5.1.0/interactions/models/discord/invite.py` & `interactions.py-5.2.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/message.py` & `interactions.py-5.2.0/interactions/models/discord/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
 
         Returns:
             A boolean indicating whether the query could be found or not
         """
         return mentions(text=self.content or self.system_content, query=query, tag_as_mention=tag_as_mention)
 
     @classmethod
-    def _process_dict(cls, data: dict, client: "Client") -> dict:
+    def _process_dict(cls, data: dict, client: "Client") -> dict:  # noqa: C901
         if author_data := data.pop("author", None):
             if "guild_id" in data and "member" in data:
                 author_data["member"] = data.pop("member")
                 data["author_id"] = client.cache.place_member_data(data["guild_id"], author_data).id
             else:
                 data["author_id"] = client.cache.place_user_data(author_data).id
```

### Comparing `interactions.py-5.1.0/interactions/models/discord/modal.py` & `interactions.py-5.2.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/reaction.py` & `interactions.py-5.2.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/role.py` & `interactions.py-5.2.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/scheduled_event.py` & `interactions.py-5.2.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/snowflake.py` & `interactions.py-5.2.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/stage_instance.py` & `interactions.py-5.2.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/sticker.py` & `interactions.py-5.2.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/team.py` & `interactions.py-5.2.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/thread.py` & `interactions.py-5.2.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/timestamp.py` & `interactions.py-5.2.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/user.py` & `interactions.py-5.2.0/interactions/models/discord/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,10 +681,11 @@
             reason: The reason for this ban
 
         """
         if delete_message_days is not MISSING:
             warn(
                 "delete_message_days  is deprecated and will be removed in a future update",
                 DeprecationWarning,
+                stacklevel=2,
             )
             delete_message_seconds = delete_message_days * 3600
         await self._client.http.create_guild_ban(self._guild_id, self.id, delete_message_seconds, reason=reason)
```

### Comparing `interactions.py-5.1.0/interactions/models/discord/user.pyi` & `interactions.py-5.2.0/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/voice_state.py` & `interactions.py-5.2.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/discord/webhooks.py` & `interactions.py-5.2.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/__init__.py` & `interactions.py-5.2.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/active_voice_state.py` & `interactions.py-5.2.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/annotations/slash.py` & `interactions.py-5.2.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/application_commands.py` & `interactions.py-5.2.0/interactions/models/internal/application_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1273,15 +1273,15 @@
             raise ValueError("auto_defer decorators must be positioned under a slash_command decorator")
         func.auto_defer = AutoDefer(enabled=enabled, ephemeral=ephemeral, time_until_defer=time_until_defer)
         return func
 
     return wrapper
 
 
-def application_commands_to_dict(
+def application_commands_to_dict(  # noqa: C901
     commands: Dict["Snowflake_Type", Dict[str, InteractionCommand]], client: "Client"
 ) -> dict:
     """
     Convert the command list into a format that would be accepted by discord.
 
     `Client.interactions` should be the variable passed to this
```

### Comparing `interactions.py-5.1.0/interactions/models/internal/auto_defer.py` & `interactions.py-5.2.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/callback.py` & `interactions.py-5.2.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/checks.py` & `interactions.py-5.2.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/command.py` & `interactions.py-5.2.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/context.py` & `interactions.py-5.2.0/interactions/models/internal/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/converters.py` & `interactions.py-5.2.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/cooldowns.py` & `interactions.py-5.2.0/interactions/models/internal/cooldowns.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         cooldown_system: Type[CooldownSystem] = CooldownSystem,
     ) -> None:
         self.bucket: Buckets = cooldown_bucket
         self.cooldown_repositories = {}
         self.rate: int = rate
         self.interval: float = interval
 
-        self.cooldown_system: Type[CooldownSystem] = cooldown_system
+        self.cooldown_system: Type[CooldownSystem] = cooldown_system or CooldownSystem
 
     async def get_cooldown(self, context: "BaseContext") -> "CooldownSystem":
         key = await self.bucket(context)
 
         if key not in self.cooldown_repositories:
             cooldown = self.cooldown_system(self.rate, self.interval)
             self.cooldown_repositories[key] = cooldown
```

### Comparing `interactions.py-5.1.0/interactions/models/internal/extension.py` & `interactions.py-5.2.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/listener.py` & `interactions.py-5.2.0/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/localisation.py` & `interactions.py-5.2.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/protocols.py` & `interactions.py-5.2.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/tasks/task.py` & `interactions.py-5.2.0/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/tasks/triggers.py` & `interactions.py-5.2.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/internal/wait.py` & `interactions.py-5.2.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/misc/context_manager.py` & `interactions.py-5.2.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions/models/misc/iterator.py` & `interactions.py-5.2.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions.py.egg-info/PKG-INFO` & `interactions.py-5.2.0/interactions.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.1.0
+Version: 5.2.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.1.0/interactions.py.egg-info/SOURCES.txt` & `interactions.py-5.2.0/interactions.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/interactions.py.egg-info/requires.txt` & `interactions.py-5.2.0/interactions.py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/pyproject.toml` & `interactions.py-5.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.1.0"
+version = "5.2.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
@@ -196,8 +196,8 @@
 suppress-dummy-args = true
 suppress-none-returning = true
 
 [tool.ruff.flake8-errmsg]
 max-string-length = 20
 
 [tool.ruff.mccabe]
-max-complexity = 10
+max-complexity = 13
```

### Comparing `interactions.py-5.1.0/setup.py` & `interactions.py-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/consts.py` & `interactions.py-5.2.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/test_bot.py` & `interactions.py-5.2.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/test_cache.py` & `interactions.py-5.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/test_contexts.py` & `interactions.py-5.2.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/test_cooldowns.py` & `interactions.py-5.2.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/test_emoji.py` & `interactions.py-5.2.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.1.0/tests/utils.py` & `interactions.py-5.2.0/tests/utils.py`

 * *Files identical despite different names*

