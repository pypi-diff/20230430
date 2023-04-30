# Comparing `tmp/twnet_parser-0.4.0.tar.gz` & `tmp/twnet_parser-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twnet_parser-0.4.0.tar", last modified: Sun Apr  9 14:27:20 2023, max compression
+gzip compressed data, was "twnet_parser-0.5.0.tar", last modified: Sun Apr 30 11:12:07 2023, max compression
```

## Comparing `twnet_parser-0.4.0.tar` & `twnet_parser-0.5.0.tar`

### file list

```diff
@@ -1,130 +1,134 @@
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.4.0/LICENSE.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4557 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3824 2023-04-09 14:22:31.000000 twnet_parser-0.4.0/README.md
--rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.4.0/pyproject.toml
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/scripts/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)    23744 2023-04-09 10:11:42.000000 twnet_parser-0.4.0/scripts/generate_messages.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/setup.cfg
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/tests/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.4.0/tests/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.4.0/tests/control_packets7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)    12270 2023-04-07 08:45:32.000000 twnet_parser-0.4.0/tests/ctrl_packets_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.4.0/tests/int_packer_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.4.0/tests/invalid_packet_header7_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/tests/msg7/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.4.0/tests/msg7/sv_tune_params_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.4.0/tests/packet_header6_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9551 2023-04-09 14:21:22.000000 twnet_parser-0.4.0/tests/packet_header7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.4.0/tests/packet_invalid_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.4.0/tests/packet_with_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.4.0/tests/repack_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.4.0/tests/unpacker_state_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      991 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/chunk_header.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       25 2023-04-09 13:43:44.000000 twnet_parser-0.4.0/twnet_parser/constants.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      207 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/ctrl_message.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/external/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/external/huffman.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/message_parser.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/twnet_parser/messages7/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/messages7/control/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      317 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/accept.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      811 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/close.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      579 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/connect.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      303 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/keep_alive.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/token.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.153049 twnet_parser-0.4.0/twnet_parser/messages7/game/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1319 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_call_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_command.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      854 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      577 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_kill.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      592 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_ready_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1155 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_say.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1049 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      833 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1689 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2136 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_start_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      803 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1172 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1178 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_leave.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      836 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_broadcast.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1329 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_chat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      815 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_checkpoint.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1178 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_drop.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2751 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      863 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      890 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_extra_projectile.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1528 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      584 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1276 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_kill_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      826 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_motd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1491 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_race_finish.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      595 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_ready_to_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1703 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_server_settings.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1846 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1313 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7501 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_tune_params.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      603 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_clear_options.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      890 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      606 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      896 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1507 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_set.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1207 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_status.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      853 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_weapon_pickup.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/twnet_parser/messages7/system/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      580 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/con_ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/enter_game.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1201 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1349 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/input.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1024 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/input_timing.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1656 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/map_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      763 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      571 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ping.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ping_reply.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      834 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      587 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_off.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      585 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_on.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      807 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      819 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      814 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_line.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      573 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      593 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/request_map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      769 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/server_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1747 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      970 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap_empty.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1471 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap_single.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/msg7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/twnet_parser/msg_matcher/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/control7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/game7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/system7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      275 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/net_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.4.0/twnet_parser/packer.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7318 2023-04-09 14:18:13.000000 twnet_parser-0.4.0/twnet_parser/packet.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/pretty_print.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser.egg-info/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4557 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4286 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/SOURCES.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/dependency_links.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)       31 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/top_level.txt
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/venv/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/venv/bin/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2man.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.5.0/LICENSE.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6411 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5678 2023-04-30 11:10:43.000000 twnet_parser-0.5.0/README.md
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/examples/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/examples/print_pcap_files/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      680 2023-04-09 15:01:20.000000 twnet_parser-0.5.0/examples/print_pcap_files/print_pcap_files.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.5.0/pyproject.toml
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/scripts/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)    27976 2023-04-16 14:48:58.000000 twnet_parser-0.5.0/scripts/generate_messages.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/setup.cfg
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/tests/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.5.0/tests/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.5.0/tests/control_packets7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.5.0/tests/ctrl_packets_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.5.0/tests/int_packer_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.5.0/tests/invalid_packet_header7_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/tests/msg7/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.5.0/tests/msg7/sv_tune_params_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.5.0/tests/packet_header6_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9813 2023-04-16 09:39:23.000000 twnet_parser-0.5.0/tests/packet_header7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.5.0/tests/packet_invalid_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.5.0/tests/packet_with_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.5.0/tests/repack_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.5.0/tests/unpacker_state_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1714 2023-04-29 06:51:40.000000 twnet_parser-0.5.0/twnet_parser/chunk_header.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       25 2023-04-09 13:43:44.000000 twnet_parser-0.5.0/twnet_parser/constants.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      256 2023-04-30 10:39:09.000000 twnet_parser-0.5.0/twnet_parser/ctrl_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/enum7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/external/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/external/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/message_parser.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/twnet_parser/messages7/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/messages7/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      363 2023-04-30 10:43:30.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      879 2023-04-30 11:05:40.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-04-30 10:43:52.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      370 2023-04-30 10:44:02.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      754 2023-04-30 10:41:20.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/messages7/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1434 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1132 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_command.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      690 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      705 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_ready_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1314 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1804 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2251 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      918 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1337 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_leave.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      950 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1487 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      930 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_checkpoint.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_drop.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2916 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1327 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      978 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1177 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1004 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1643 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      697 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1390 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      940 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1606 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_race_finish.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      707 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1818 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_server_settings.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1961 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1477 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7615 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1005 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      719 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1669 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1322 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/messages7/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      692 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1464 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1139 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1833 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      877 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      684 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      949 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      700 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_off.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      698 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_on.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      922 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1224 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      934 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      929 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      686 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      706 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/server_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1861 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1084 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1585 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap_single.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/msg7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/msg_matcher/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/control7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/game7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/system7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      295 2023-04-16 13:57:22.000000 twnet_parser-0.5.0/twnet_parser/net_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.5.0/twnet_parser/packer.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9269 2023-04-30 11:05:42.000000 twnet_parser-0.5.0/twnet_parser/packet.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/pretty_print.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser.egg-info/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6411 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4354 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/top_level.txt
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/venv/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/venv/bin/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rstpep2html.py
```

### Comparing `twnet_parser-0.4.0/LICENSE.txt` & `twnet_parser-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/PKG-INFO` & `twnet_parser-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet_parser
-Version: 0.4.0
+Version: 0.5.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -46,19 +46,19 @@
 
 ## Features
 
 | Feature                        | Status             |
 | ------------------------------ | ------------------ |
 | Deserialize 0.7 packet headers | :heavy_check_mark: |
 | Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 80%                |
+| Deserialize 0.7 messages       | 85%                |
 | Deserialize 0.7 snapshots      |                    |
 | Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    |                    |
-| Serialize 0.7 messages         | 80%                |
+| Serialize 0.7 chunk headers    | :heavy_check_mark: |
+| Serialize 0.7 messages         | 85%                |
 | Deserialize 0.6 packet headers |                    |
 | Deserialize 0.6 chunk headers  |                    |
 | Deserialize 0.6 messages       |                    |
 | Deserialize 0.6 snapshots      |                    |
 | Serialize 0.6 packet headers   |                    |
 | Serialize 0.6 chunk headers    |                    |
 | Serialize 0.6 messages         |                    |
@@ -81,14 +81,75 @@
 If you want to build something with this library
 you do have to understand how the protocol works
 and when the client and server have to send what.
 
 This [protocol documentation](https://chillerdragon.github.io/teeworlds-protocol/index.html)
 should get you started to understand the basics.
 
+## Convenient defaults and fully customizable
+
+```python
+from twnet_parser.packet import TwPacket
+from twnet_parser.messages7.game.cl_call_vote import MsgClCallVote
+
+"""
+The call to packet.pack() generates
+a valid byte array that can be sent as an udp payload
+
+It uses default values for things like:
+ security token, acknowledge number, packet flags,
+ chunk header (flags, size, seq),
+ vote type, vote value, vote reason, vote force
+
+It computes a valid chunk header size field based
+on the payload length.
+
+It sets the correct num chunks field in the packet header
+based on the amount of messages you added (1 in this case)
+
+While this has all fields set that packet would be dropped by a vanilla
+implementation because the security token and sequence number is wrong.
+So you have to take care of those your self.
+"""
+packet = TwPacket()
+msg = MsgClCallVote()
+packet.messages.append(msg)
+packet.pack() # => b'\x00\x00\x01\xff\xff\xff\xff\x00\x00\x80\x01default\x00default\x00default\x00\x00'
+
+
+
+"""
+Here we also send a Call vote message.
+But this time we set a security token and a few other fields.
+
+Note that we set num_chunks to 6 which is wrong because
+we only send one message (MsgClCallVote).
+But this library allows you to do so.
+And it will not compute the correct amount.
+But use your explicitly set wrong one instead.
+
+This allows you to have full control and craft any kind of packet.
+May it be correct or not.
+"""
+packet = TwPacket()
+packet.header.token = b'\x48\x1f\x93\xd7'
+packet.header.num_chunks = 6
+packet.header.ack = 638
+packet.header.flags.control = False
+packet.header.flags.compression = False
+msg = MsgClCallVote()
+msg.header.seq = 10
+msg.type = 'option'
+msg.value = 'test'
+msg.reason = ''
+msg.force = False
+packet.messages.append(msg)
+packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
```

### Comparing `twnet_parser-0.4.0/README.md` & `twnet_parser-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 
 ## Features
 
 | Feature                        | Status             |
 | ------------------------------ | ------------------ |
 | Deserialize 0.7 packet headers | :heavy_check_mark: |
 | Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 80%                |
+| Deserialize 0.7 messages       | 85%                |
 | Deserialize 0.7 snapshots      |                    |
 | Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    |                    |
-| Serialize 0.7 messages         | 80%                |
+| Serialize 0.7 chunk headers    | :heavy_check_mark: |
+| Serialize 0.7 messages         | 85%                |
 | Deserialize 0.6 packet headers |                    |
 | Deserialize 0.6 chunk headers  |                    |
 | Deserialize 0.6 messages       |                    |
 | Deserialize 0.6 snapshots      |                    |
 | Serialize 0.6 packet headers   |                    |
 | Serialize 0.6 chunk headers    |                    |
 | Serialize 0.6 messages         |                    |
@@ -64,14 +64,75 @@
 If you want to build something with this library
 you do have to understand how the protocol works
 and when the client and server have to send what.
 
 This [protocol documentation](https://chillerdragon.github.io/teeworlds-protocol/index.html)
 should get you started to understand the basics.
 
+## Convenient defaults and fully customizable
+
+```python
+from twnet_parser.packet import TwPacket
+from twnet_parser.messages7.game.cl_call_vote import MsgClCallVote
+
+"""
+The call to packet.pack() generates
+a valid byte array that can be sent as an udp payload
+
+It uses default values for things like:
+ security token, acknowledge number, packet flags,
+ chunk header (flags, size, seq),
+ vote type, vote value, vote reason, vote force
+
+It computes a valid chunk header size field based
+on the payload length.
+
+It sets the correct num chunks field in the packet header
+based on the amount of messages you added (1 in this case)
+
+While this has all fields set that packet would be dropped by a vanilla
+implementation because the security token and sequence number is wrong.
+So you have to take care of those your self.
+"""
+packet = TwPacket()
+msg = MsgClCallVote()
+packet.messages.append(msg)
+packet.pack() # => b'\x00\x00\x01\xff\xff\xff\xff\x00\x00\x80\x01default\x00default\x00default\x00\x00'
+
+
+
+"""
+Here we also send a Call vote message.
+But this time we set a security token and a few other fields.
+
+Note that we set num_chunks to 6 which is wrong because
+we only send one message (MsgClCallVote).
+But this library allows you to do so.
+And it will not compute the correct amount.
+But use your explicitly set wrong one instead.
+
+This allows you to have full control and craft any kind of packet.
+May it be correct or not.
+"""
+packet = TwPacket()
+packet.header.token = b'\x48\x1f\x93\xd7'
+packet.header.num_chunks = 6
+packet.header.ack = 638
+packet.header.flags.control = False
+packet.header.flags.compression = False
+msg = MsgClCallVote()
+msg.header.seq = 10
+msg.type = 'option'
+msg.value = 'test'
+msg.reason = ''
+msg.force = False
+packet.messages.append(msg)
+packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
```

### Comparing `twnet_parser-0.4.0/scripts/generate_messages.py` & `twnet_parser-0.5.0/scripts/generate_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import os
 import json
 
-from typing import TypedDict, Literal, Optional, Dict, Union
+from typing import \
+    TypedDict, Literal, Optional, Dict, Union, TextIO
 
 KIND = Literal[ \
             'int32', \
             'tick', \
             'string', \
             'raw', \
             'sha256', \
@@ -17,39 +18,43 @@
             'boolean', \
             'tune_param', \
             'snapshot_object', \
             'array', \
             'flags', \
             'optional']
 
-class ConstantJson(TypedDict):
-    name: list[str]
-    type: str
+class GameEnumValueJson(TypedDict):
     value: int
+    name: list[str]
 
-class NetEnumValuesJson(TypedDict):
-    value: str
+class GameEnumJson(TypedDict):
     name: list[str]
+    values: list[GameEnumValueJson]
 
-class NetEnumJson(TypedDict):
+class ConstantJson(TypedDict):
     name: list[str]
-    values: list[NetEnumValuesJson]
+    type: str
+    value: int
 
 class InnerNetMessageMemberTypeJson(TypedDict):
     kind: KIND
     disallow_cc: bool
 
 class ArrayMemberTypeJson(TypedDict):
     kind: KIND
     # strings
     disallow_cc: bool
 
 class NetMessageMemberTypeJson(TypedDict):
     kind: KIND
     inner: InnerNetMessageMemberTypeJson
+
+    # enums
+    enum: list[str]
+
     # strings
     disallow_cc: bool
 
     # arrays
     count: int
     member_type: ArrayMemberTypeJson
 
@@ -64,15 +69,15 @@
     id: int
     name: list[str]
     members: list[NetMessageMemberJson]
     attributes: list[Literal['msg_encoding']]
 
 class SpecJson(TypedDict):
     constants: list[ConstantJson]
-    game_enumerations: list[NetEnumJson]
+    game_enumerations: list[GameEnumJson]
     game_messages: list[NetMessageJson]
     system_messages: list[NetMessageJson]
 
 def gen_match_file7(
         msg_type: Literal['system', 'game'],
         messages: list[NetMessageJson]
 ):
@@ -138,207 +143,38 @@
     name = ''.join([part.capitalize() for part in name_list])
     return fix_name_conflict(name)
 
 def name_to_snake(name_list: list[str]) -> str:
     name = '_'.join(name_list)
     return fix_name_conflict(name)
 
-def generate_msg(msg: NetMessageJson, game: Literal['game', 'system']) -> None:
-    name_snake = name_to_snake(msg['name'])
-    name_camel = name_to_camel(msg['name'])
-    dirname = os.path.dirname(__file__)
-    file_path= os.path.join(
-            dirname,
-            f'../twnet_parser/messages7/{game}/',
-            f'{name_snake}.py')
-    # if os.path.exists(file_path):
-    #     print(f"Warning: file already exists! {file_path}")
-    #     return
-    with open(file_path, 'w') as out_file:
-        print(f"Generating {file_path} ...")
-        out_file.write('# generated by scripts/generate_messages.py\n')
-        out_file.write('\n')
-        out_file.write('from twnet_parser.pretty_print import PrettyPrint\n')
-        if len(msg['members']) > 0:
-            out_file.write('from twnet_parser.packer import Unpacker\n')
-        out_file.write('from twnet_parser.chunk_header import ChunkHeader\n')
-        out_file.write(get_dependencies(msg))
-        out_file.write('\n')
-        out_file.write(f'class Msg{name_camel}(PrettyPrint):\n')
-        out_file.write('    def __init__(\n')
-        out_file.write('            self,\n')
-        args: list[str] = []
-        for member in msg['members']:
-            # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
-            ftype = 'int'
-            default = '-1'
-            if member['type']['kind'] == 'string':
-                ftype = 'str'
-                default = "'default'"
-            elif member['type']['kind'] in \
-                ('raw', 'sha256', 'rest'): # TODO: rest sha256 and raw
-                ftype = 'bytes'
-                default = "b'\\x00'"
-            elif member['type']['kind'] == 'data':
-                ftype = 'bytes'
-                default = "b'\\x00'"
-                if member['type']['size'] == 'specified_before':
-                    args.append('            data_size: Optional[int] = None')
-                else:
-                    raise ValueError(f"Error: unknown data size {member['type']}")
-            # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
-            elif member['type']['kind'] == 'enum':
-                ftype = 'int'
-                default = '0'
-                # TODO: use ENUM_NAME_SOME_VALUE as default here
-            elif member['type']['kind'] in ('int32', 'tick'):
-                ftype = 'int'
-                default = '0'
-            elif member['type']['kind'] == 'boolean':
-                ftype = 'bool'
-                default = 'False'
-            elif member['type']['kind'] == 'tune_param':
-                ftype = 'float'
-                default = '0.0'
-            elif member['type']['kind'] == 'snapshot_object':
-                # TODO: think about snapshot_object
-                ftype = 'int'
-                default = '0'
-            elif member['type']['kind'] == 'array':
-                size: int = member['type']['count']
-                if size is None:
-                    print("Error: size is none for the following message")
-                    print(msg)
-                    exit(1)
-                arr_member: ArrayMemberTypeJson = member['type']['member_type']
-                if arr_member['kind'] == 'string':
-                    ftype = f'Annotated[list[str], {size}]'
-                    default = '[' + ', '.join(["''"] * size) + ']'
-                elif arr_member['kind'] == 'boolean':
-                    ftype = f'Annotated[list[bool], {size}]'
-                    default = '[' + ', '.join(["False"] * size) + ']'
-                elif arr_member['kind'] in ('int32', 'tick', 'enum'):
-                    ftype = f'Annotated[list[int], {size}]'
-                    default = '[' + ', '.join(["0"] * size) + ']'
-                else:
-                    raise ValueError( \
-                        f"Error: unknown array member type {member['type']}")
-                # Initializing lists with defaults
-                # And type annotation can get quite long
-                # So split it in two lines
-                default = f'\\\n                {default}'
-            elif member['type']['kind'] == 'flags': # TODO: think about flags
-                ftype = 'int'
-                default = '0'
-            elif member['type']['kind'] == 'optional':
-                if member['type']['inner']['kind'] == 'string':
-                    ftype = 'str'
-                    default = "''"
-                elif member['type']['inner']['kind'] in ('int32', 'tick'):
-                    ftype = 'int'
-                    default = '0'
-                else:
-                    raise ValueError(f"Error: unknown optional type {member['type']}")
-            else:
-                raise ValueError(f"Error: unknown type {member['type']}")
-            name = name_to_snake(member["name"])
-            manual_default = get_default(f"{game}.{name_snake}.{name}")
-            if manual_default:
-                default = manual_default
-            args.append(f'            {name}: {ftype} = {default}')
-        out_file.write(',\n'.join(args) + '\n')
-        out_file.write('    ) -> None:\n')
-        out_file.write(f"        self.message_name = '{name_snake}'\n")
-        sys: str = 'True' if game == 'system' else 'False'
-        out_file.write(f"        self.system_message = {sys}\n")
-        out_file.write("        self.header: ChunkHeader\n")
-        out_file.write('\n')
-        for member in msg['members']:
-            # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
-            ftype = 'int'
-            if member['type']['kind'] == 'string':
-                ftype = 'str'
-            elif member['type']['kind'] in \
-                    ('raw', 'sha256', 'rest'): # TODO: sha256 and raw
-                ftype = 'bytes'
-            elif member['type']['kind'] == 'data':
-                ftype = 'bytes'
-                if member['type']['size'] == 'specified_before':
-                    out_file.write("        " \
-                        "self.data_size: int = data_size if data_size else len(data)\n")
-                else:
-                    raise ValueError(f"Error: unknown data size {member['type']}")
-            # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
-            elif member['type']['kind'] == 'enum':
-                ftype = 'int'
-            elif member['type']['kind'] in ('int32', 'tick'):
-                ftype = 'int'
-            elif member['type']['kind'] == 'boolean':
-                ftype = 'bool'
-            elif member['type']['kind'] == 'tune_param':
-                ftype = 'float'
-            elif member['type']['kind'] == 'snapshot_object':
-                # TODO: think about snapshot_object
-                ftype = 'int'
-            elif member['type']['kind'] == 'array':
-                # Array type annotations are so annoyingly long
-                # also there is a planned refactor
-                # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/4
-                # so inherit type from constructor arguments
-                ftype = ''
-            elif member['type']['kind'] == 'flags': # TODO: think about flags
-                ftype = 'int'
-            elif member['type']['kind'] == 'optional':
-                if member['type']['inner']['kind'] == 'string':
-                    ftype = 'str'
-                elif member['type']['inner']['kind'] in ('int32', 'tick'):
-                    ftype = 'int'
-                else:
-                    raise ValueError(f"Error: unknown optional type {member['type']}")
-            else:
-                raise ValueError(f"Error: unknown type {member['type']}")
-            name = name_to_snake(member["name"])
-            if ftype != '':
-                ftype = f': {ftype}'
-            out_file.write(f"        self.{name}{ftype} = {name}\n")
-        out_file.write('\n')
-        out_file.write('    # first byte of data\n')
-        out_file.write('    # has to be the first byte of the message payload\n')
-        out_file.write('    # NOT the chunk header and NOT the message id\n')
-        out_file.write('    def unpack(self, data: bytes) -> bool:\n')
-        if len(msg['members']) > 0:
-            out_file.write('        unpacker = Unpacker(data)\n')
-        out_file.write(gen_unpack_members(msg))
-        out_file.write('        return True\n')
-        out_file.write('\n')
-        out_file.write('    def pack(self) -> bytes:\n')
-        out_file.write(gen_pack_return(msg))
-
 def gen_unpack_members(msg: NetMessageJson) -> str:
     res: str = ''
     for member in msg['members']:
         # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
         unpacker = 'int()'
         if member['type']['kind'] == 'string':
             if member['type']['disallow_cc']:
                 unpacker = 'str(SANITIZE_CC)'
             else:
                 unpacker = 'str()'
-        elif member['type']['kind'] in \
-            ('raw', 'sha256', 'rest'): # TODO: do we need to fix size for sha256?
+        elif member['type']['kind'] == 'rest':
             unpacker = 'raw()'
+        elif member['type']['kind'] == 'sha256':
+            unpacker = 'raw(32)'
         elif member['type']['kind'] == 'data':
             if member['type']['size'] == 'specified_before':
                 res += '        self.data_size = unpacker.get_int()\n'
                 unpacker = 'raw(self.data_size)'
             else:
                 raise ValueError(f"Error: unknown data size {member['type']}")
         # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
         elif member['type']['kind'] == 'enum':
-            unpacker = 'int() # TODO: this is a enum'
+            enum_name: str = name_to_camel(member['type']['enum']).upper()
+            unpacker = f"int() # enum {enum_name}"
         elif member['type']['kind'] in ('int32', 'tick'):
             unpacker = 'int()'
         elif member['type']['kind'] == 'boolean':
             unpacker = 'int() == 1'
         elif member['type']['kind'] == 'tune_param':
             unpacker = 'int() / 100.0'
         elif member['type']['kind'] == 'snapshot_object':
@@ -353,15 +189,19 @@
             arr_member: ArrayMemberTypeJson = member['type']['member_type']
             if arr_member['kind'] == 'string':
                 if arr_member['disallow_cc']:
                     unpacker = 'str(SANITIZE_CC)'
                 else:
                     unpacker = 'str()'
             elif arr_member['kind'] == 'enum':
-                unpacker = 'int() # TODO: this is a enum'
+                # We intentionally do not do anything fancy here
+                # no enums for example because it comes with too many
+                # disadvantages see the related issue here
+                # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/7
+                unpacker = 'int()'
             elif arr_member['kind'] == 'boolean':
                 unpacker = 'int() == 1'
             elif arr_member['kind'] in ('int32', 'tick'):
                 unpacker = 'int()'
             else:
                 raise ValueError(f"Error: unknown array member type {member['type']}")
             name = name_to_snake(member["name"])
@@ -386,29 +226,32 @@
         name = name_to_snake(member["name"])
         res += f'        self.{name} = unpacker.get_{unpacker}\n'
     return res
 
 def get_dependencies(msg: NetMessageJson) -> str:
     packer_deps: list[str] = []
     typing_deps: list[str] = []
+    need_enums: bool = False
     for member in msg['members']:
         if member['type']['kind'] == 'string':
             packer_deps.append('pack_str')
             if member['type']['disallow_cc']:
                 packer_deps.append('SANITIZE_CC')
-        elif member['type']['kind'] in \
-            ('raw', 'sha256', 'rest'):
+        elif member['type']['kind'] == 'rest':
             pass
+        elif member['type']['kind'] == 'sha256':
+            typing_deps.append('Annotated')
         elif member['type']['kind'] == 'data':
             if member['type']['size'] == 'specified_before':
                 typing_deps.append('Optional')
             else:
                 raise ValueError(f"Error: unknown data size {member['type']}")
         # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
         elif member['type']['kind'] == 'enum':
+            need_enums = True
             packer_deps.append('pack_int')
         elif member['type']['kind'] in ('int32', 'tick'):
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'boolean':
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'tune_param':
             packer_deps.append('pack_int')
@@ -420,14 +263,15 @@
             typing_deps.append('Annotated')
             arr_member: ArrayMemberTypeJson = member['type']['member_type']
             if arr_member['kind'] == 'string':
                 packer_deps.append('pack_str')
                 if arr_member['disallow_cc']:
                     packer_deps.append('SANITIZE_CC')
             elif arr_member['kind'] == 'enum':
+                need_enums = True
                 packer_deps.append('pack_int')
             elif arr_member['kind'] == 'boolean':
                 packer_deps.append('pack_int')
             elif arr_member['kind'] in ('int32', 'tick'):
                 packer_deps.append('pack_int')
             else:
                 raise ValueError(f"Error: unknown array member type {member['type']}")
@@ -445,24 +289,25 @@
     res: str = ''
     if len(packer_deps) > 0:
         res += 'from twnet_parser.packer import ' + \
             ', '.join(sorted(set(packer_deps))) + '\n'
     if len(typing_deps) > 0:
         res += 'from typing import ' + \
             ', '.join(sorted(set(typing_deps))) + '\n'
+    if need_enums:
+        res += 'import twnet_parser.enum7 as enum7\n'
     return res
 
 def pack_field(member: NetMessageMemberJson) -> str:
     name: str = name_to_snake(member["name"])
     field: str = f'self.{name}'
     packer = 'int'
     if member['type']['kind'] == 'string':
         packer = 'str'
-    elif member['type']['kind'] in \
-        ('raw', 'sha256', 'rest'): # TODO: raw sha256 rest
+    elif member['type']['kind'] in ('sha256', 'rest'):
         return f'self.{name}'
     elif member['type']['kind'] == 'data':
         if member['type']['size'] == 'specified_before':
             return f'pack_int(self.data_size) + \\\n' \
                 f'            self.{name}'
         else:
             raise ValueError(f"Error: unknown data size {member['type']}")
@@ -548,35 +393,301 @@
         elif isinstance(default, str):
             return f"'{default}'"
         else:
             print(f"Error: invalid default type for field {field_path}")
             print(f"        please check {def_file} for errors")
             exit(1)
 
-def generate(spec: str) -> None:
-    print(f"generating classes from {spec} ...")
-    with open(spec) as spec_io:
-        spec_data: SpecJson = json.load(spec_io)
-        # for msg in [spec_data['game_messages'][1]]:
-        game_messages: list[NetMessageJson] = spec_data['game_messages']
-        system_messages: list[NetMessageJson] = spec_data['system_messages']
-        gen_match_file7('game', game_messages)
-        gen_match_file7('system', system_messages)
-        for msg in game_messages:
-            generate_msg(msg, 'game')
-        for msg in system_messages:
-            generate_msg(msg, 'system')
+class CodeGenerator():
+    def __init__(self) -> None:
+        self.game_enums: list[GameEnumJson] = []
+
+    def write_init_method_header(
+            self,
+            out_file: TextIO,
+            msg: NetMessageJson,
+            game: Literal['system', 'game'],
+            name_snake: str
+    ) -> None:
+        comma: str = ''
+        if len(msg['members']) > 0:
+            comma = ',\n'
+        out_file.write( \
+            '    def __init__(\n' \
+            '            self,\n' \
+            f'            chunk_header: ChunkHeader = ChunkHeader(){comma}')
+        args: list[str] = []
+        for member in msg['members']:
+            # {
+            #   'name': ['message'],
+            #   'type': {
+            #     'kind': 'string',
+            #     'disallow_cc': False
+            #   }
+            # }
+            ftype = 'int'
+            default = '-1'
+            if member['type']['kind'] == 'string':
+                ftype = 'str'
+                default = "'default'"
+            elif member['type']['kind'] == 'rest':
+                ftype = 'bytes'
+                default = "b'\\x00'"
+            elif member['type']['kind'] == 'sha256':
+                ftype = 'Annotated[bytes, 32]'
+                default = "bytes(32)"
+            elif member['type']['kind'] == 'data':
+                ftype = 'bytes'
+                default = "b'\\x00'"
+                if member['type']['size'] == 'specified_before':
+                    args.append('            data_size: Optional[int] = None')
+                else:
+                    raise ValueError(f"Error: unknown data size {member['type']}")
+            # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
+            elif member['type']['kind'] == 'enum':
+                enum_name: str = name_to_camel(member['type']['enum'])
+                ftype = 'int'
+                default = self.get_default_enum7(enum_name)
+                default = f"enum7.{default}.value"
+            elif member['type']['kind'] in ('int32', 'tick'):
+                ftype = 'int'
+                default = '0'
+            elif member['type']['kind'] == 'boolean':
+                ftype = 'bool'
+                default = 'False'
+            elif member['type']['kind'] == 'tune_param':
+                ftype = 'float'
+                default = '0.0'
+            elif member['type']['kind'] == 'snapshot_object':
+                # TODO: think about snapshot_object
+                ftype = 'int'
+                default = '0'
+            elif member['type']['kind'] == 'array':
+                size: int = member['type']['count']
+                if size is None:
+                    print("Error: size is none for the following message")
+                    print(msg)
+                    exit(1)
+                arr_member: ArrayMemberTypeJson = member['type']['member_type']
+                if arr_member['kind'] == 'string':
+                    ftype = f'Annotated[list[str], {size}]'
+                    default = '[' + ', '.join(["''"] * size) + ']'
+                elif arr_member['kind'] == 'boolean':
+                    ftype = f'Annotated[list[bool], {size}]'
+                    default = '[' + ', '.join(["False"] * size) + ']'
+                elif arr_member['kind'] in ('int32', 'tick', 'enum'):
+                    ftype = f'Annotated[list[int], {size}]'
+                    default = '[' + ', '.join(["0"] * size) + ']'
+                else:
+                    raise ValueError( \
+                        f"Error: unknown array member type {member['type']}")
+                # Initializing lists with defaults
+                # And type annotation can get quite long
+                # So split it in two lines
+                default = f'\\\n                {default}'
+            elif member['type']['kind'] == 'flags': # TODO: think about flags
+                ftype = 'int'
+                default = '0'
+            elif member['type']['kind'] == 'optional':
+                if member['type']['inner']['kind'] == 'string':
+                    ftype = 'str'
+                    default = "''"
+                elif member['type']['inner']['kind'] in ('int32', 'tick'):
+                    ftype = 'int'
+                    default = '0'
+                else:
+                    raise \
+                        ValueError( \
+                        f"Error: unknown optional type {member['type']}")
+            else:
+                raise ValueError(f"Error: unknown type {member['type']}")
+            name = name_to_snake(member["name"])
+            manual_default = get_default(f"{game}.{name_snake}.{name}")
+            if manual_default:
+                default = manual_default
+            args.append(f'            {name}: {ftype} = {default}')
+        out_file.write(',\n'.join(args) + '\n')
+        out_file.write('    ) -> None:\n')
+
+    def generate_msg(
+            self,
+            msg: NetMessageJson,
+            game: Literal['game', 'system']
+    ) -> None:
+        name_snake = name_to_snake(msg['name'])
+        name_camel = name_to_camel(msg['name'])
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                f'../twnet_parser/messages7/{game}/',
+                f'{name_snake}.py')
+        # if os.path.exists(file_path):
+        #     print(f"Warning: file already exists! {file_path}")
+        #     return
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write('# generated by scripts/generate_messages.py\n')
+            out_file.write('\n')
+            out_file.write('from twnet_parser.pretty_print import PrettyPrint\n')
+            if len(msg['members']) > 0:
+                out_file.write('from twnet_parser.packer import Unpacker\n')
+            out_file.write('from twnet_parser.chunk_header import ChunkHeader\n')
+            out_file.write(get_dependencies(msg))
+            out_file.write('\n')
+            out_file.write(f'class Msg{name_camel}(PrettyPrint):\n')
+            self.write_init_method_header(out_file, msg, game, name_snake)
+            out_file.write(f"        self.message_name: str = '{name_snake}'\n")
+            sys: str = 'True' if game == 'system' else 'False'
+            out_file.write(f"        self.system_message: bool = {sys}\n")
+            out_file.write(f"        self.message_id: int = {msg['id']}\n")
+            out_file.write("        self.header: ChunkHeader = chunk_header\n")
+            out_file.write('\n')
+            for member in msg['members']:
+                # {
+                #   'name': ['message'],
+                #   'type': {
+                #     'kind': 'string',
+                #     'disallow_cc': False
+                #   }
+                # } 
+                ftype = 'int'
+                if member['type']['kind'] == 'string':
+                    ftype = 'str'
+                elif member['type']['kind'] == 'rest':
+                    ftype = 'bytes'
+                elif member['type']['kind'] == 'sha256':
+                    ftype = 'Annotated[bytes, 32]'
+                elif member['type']['kind'] == 'data':
+                    ftype = 'bytes'
+                    if member['type']['size'] == 'specified_before':
+                        out_file.write("        " \
+                            "self.data_size: int =" \
+                            " data_size if data_size else len(data)\n")
+                    else:
+                        raise ValueError(f"Error: unknown data size {member['type']}")
+                # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
+                elif member['type']['kind'] == 'enum':
+                    ftype = 'int'
+                elif member['type']['kind'] in ('int32', 'tick'):
+                    ftype = 'int'
+                elif member['type']['kind'] == 'boolean':
+                    ftype = 'bool'
+                elif member['type']['kind'] == 'tune_param':
+                    ftype = 'float'
+                elif member['type']['kind'] == 'snapshot_object':
+                    # TODO: think about snapshot_object
+                    ftype = 'int'
+                elif member['type']['kind'] == 'array':
+                    # Array type annotations are so annoyingly long
+                    # also there is a planned refactor
+                    # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/4
+                    # so inherit type from constructor arguments
+                    ftype = ''
+                elif member['type']['kind'] == 'flags': # TODO: think about flags
+                    ftype = 'int'
+                elif member['type']['kind'] == 'optional':
+                    if member['type']['inner']['kind'] == 'string':
+                        ftype = 'str'
+                    elif member['type']['inner']['kind'] in ('int32', 'tick'):
+                        ftype = 'int'
+                    else:
+                        raise \
+                            ValueError( \
+                            f"Error: unknown optional type {member['type']}")
+                else:
+                    raise ValueError(f"Error: unknown type {member['type']}")
+                name = name_to_snake(member["name"])
+                if ftype != '':
+                    ftype = f': {ftype}'
+                if member['type']['kind'] == 'enum':
+                    out_file.write(f"        self.{name}{ftype} = {name}\n")
+                else:
+                    out_file.write(f"        self.{name}{ftype} = {name}\n")
+            out_file.write('\n')
+            out_file.write('    # first byte of data\n')
+            out_file.write('    # has to be the first byte of the message payload\n')
+            out_file.write('    # NOT the chunk header and NOT the message id\n')
+            out_file.write('    def unpack(self, data: bytes) -> bool:\n')
+            if len(msg['members']) > 0:
+                out_file.write('        unpacker = Unpacker(data)\n')
+            out_file.write(gen_unpack_members(msg))
+            out_file.write('        return True\n')
+            out_file.write('\n')
+            out_file.write('    def pack(self) -> bytes:\n')
+            out_file.write(gen_pack_return(msg))
+
+    def get_default_enum7(self, enum_name: str) -> str:
+        """
+        enum_name has to be camel case
+
+        If for example enum_name 'chat' is given
+        it returns 'CHAT_NONE'
+        """
+        enum: GameEnumJson
+        for enum in self.game_enums:
+            base: str = name_to_camel(enum['name'])
+            if base != enum_name:
+                continue
+            val: GameEnumValueJson
+            for val in enum['values']:
+                sub: str = name_to_snake(val['name']).upper()
+                return f"{base}.{sub}"
+        raise ValueError(f"Enum not found '{enum_name}'")
+
+    def gen_enum_file7(self) -> None:
+        enum_code: str = 'from enum import Enum\n\n'
+        enum: GameEnumJson
+        for enum in self.game_enums:
+            base: str = name_to_camel(enum['name'])
+            enum_code += f'class {base}(Enum):\n'
+            val: GameEnumValueJson
+            for val in enum['values']:
+                sub: str = name_to_snake(val['name']).upper()
+                enum_code += \
+                    '    ' \
+                    f"{sub}: int = {val['value']}\n"
+            enum_code += "\n"
+        # cut off last doubled newline
+        # because we do not split a section anymore
+        enum_code = enum_code[:-1]
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                '../twnet_parser/enum7.py')
+        # if os.path.exists(file_path):
+        #     print(f"Warning: file already exists! {file_path}")
+        #     return
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write(enum_code)
+
+    def generate(self, spec: str) -> None:
+        print(f"generating classes from {spec} ...")
+        with open(spec) as spec_io:
+            spec_data: SpecJson = json.load(spec_io)
+            # for msg in [spec_data['game_messages'][1]]:
+            self.game_enums = spec_data['game_enumerations']
+            game_messages: list[NetMessageJson] = spec_data['game_messages']
+            system_messages: list[NetMessageJson] = spec_data['system_messages']
+            self.gen_enum_file7()
+            gen_match_file7('game', game_messages)
+            gen_match_file7('system', system_messages)
+            for msg in game_messages:
+                self.generate_msg(msg, 'game')
+            for msg in system_messages:
+                self.generate_msg(msg, 'system')
 
 def main() -> None:
     dirname = os.path.dirname(__file__)
     spec_07 = os.path.join(
             dirname,
             '../../libtw2/gamenet/generate/spec/teeworlds-0.7.5.json')
     if os.path.exists(spec_07):
-        generate(spec_07)
+        generator = CodeGenerator()
+        generator.generate(spec_07)
     else:
         print(f"Error: file not found {spec_07}")
         print("        try running these commands")
         print("")
         print("        git clone git@github.com:heinrich5991/libtw2 ..")
 
 if __name__ == '__main__':
```

### Comparing `twnet_parser-0.4.0/setup.cfg` & `twnet_parser-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twnet_parser
-version = 0.4.0
+version = 0.5.0
 author = ChillerDragon
 author_email = chillerdragon@gmail.com
 description = A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/teeworlds-network/twnet_parser
 license = BSD-2.0
```

### Comparing `twnet_parser-0.4.0/tests/control_packets7_test.py` & `twnet_parser-0.5.0/tests/control_packets7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/int_packer_test.py` & `twnet_parser-0.5.0/tests/int_packer_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/msg7/sv_tune_params_test.py` & `twnet_parser-0.5.0/tests/msg7/sv_tune_params_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/packet_header6_test.py` & `twnet_parser-0.5.0/tests/packet_header6_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/packet_header7_test.py` & `twnet_parser-0.5.0/tests/packet_header7_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-from twnet_parser.packet import parse7, PacketHeaderParser7, PacketHeader
+from twnet_parser.packet import \
+    parse7, PacketHeaderParser7, PacketHeader, TwPacket
 
-def test_packet_header_unpack():
+def test_packet_header_unpack() -> None:
     # TODO: change api to
     #       PacketHeader.pack()
     #       PacketHeader.unpack(bytes)
 
     parser = PacketHeaderParser7()
-    header = parser.parse_header(b'\x04\x0a\x00\xcf\x2e\xde\x1d')
+    header: PacketHeader = parser.parse_header(b'\x04\x0a\x00\xcf\x2e\xde\x1d')
 
     assert header.ack == 10
     assert header.token == b'\xcf.\xde\x1d'
     assert header.num_chunks == 0
 
     assert header.flags.control is True
     assert header.flags.resend is False
     assert header.flags.compression is False
     assert header.flags.connless is False
 
-def test_packet_header_pack_flags():
-    header = PacketHeader()
+def test_packet_header_pack_flags() -> None:
+    header: PacketHeader = PacketHeader()
     header.ack = 0
 
     header.flags.control = True
     header.flags.resend = False
     header.flags.compression = False
     header.flags.connless = False
     assert header.pack()[0:1] == b'\x04'
 
     header.flags.control = False
     header.flags.resend = False
     header.flags.compression = True
     header.flags.connless = False
     assert header.pack()[0:1] == b'\x10'
 
-def test_packet_header_pack_ack():
-    header = PacketHeader()
+def test_packet_header_pack_ack() -> None:
+    header: PacketHeader = PacketHeader()
     header.flags.control = False
     header.flags.resend = False
     header.flags.compression = False
     header.flags.connless = False
 
     header.ack = 8
     assert header.pack()[1:2] == b'\x08'
     header.ack = 9
     assert header.pack()[1:2] == b'\x09'
     header.ack = 10
     assert header.pack()[1:2] == b'\x0a'
     header.ack = 11
     assert header.pack()[1:2] == b'\x0b'
 
-def test_packet_header_repack_overflowing_ack():
-    header = PacketHeader()
+def test_packet_header_repack_overflowing_ack() -> None:
+    header: PacketHeader = PacketHeader()
     header.flags.control = False
     header.flags.resend = False
     header.flags.compression = False
     header.flags.connless = False
 
     header.ack = 1024
     parser = PacketHeaderParser7()
@@ -67,16 +68,16 @@
     assert header.ack == 1
 
     header.ack = 2000
     parser = PacketHeaderParser7()
     header = parser.parse_header(header.pack())
     assert header.ack == 976
 
-def test_packet_header_repack_ack_overlapping_into_flags_byte():
-    header = PacketHeader()
+def test_packet_header_repack_ack_overlapping_into_flags_byte() -> None:
+    header: PacketHeader = PacketHeader()
     header.flags.control = False
     header.flags.resend = False
     header.flags.compression = False
     header.flags.connless = False
 
     parser = PacketHeaderParser7()
 
@@ -127,27 +128,27 @@
     # which is 00000101 in binary
     #          |____/|/
     #          |     |
     #       flags   higher bits of ack
     header = parser.parse_header(b'\x05\xff\x00\xcf\x2e\xde\x1d')
     assert header.ack == 511
 
-def test_packet_header_pack_num_chunks():
+def test_packet_header_pack_num_chunks() -> None:
     header = PacketHeader()
 
     header.num_chunks = 0
     assert header.pack()[2:3] == b'\x00'
 
     header.num_chunks = 1
     assert header.pack()[2:3] == b'\x01'
 
     header.num_chunks = 6
     assert header.pack()[2:3] == b'\x06'
 
-def test_packet_header_pack_token():
+def test_packet_header_pack_token() -> None:
     header = PacketHeader()
     header.token = b'\x11\x22\x33\xff'
     assert header.pack()[3:] == b'\x11\x22\x33\xff'
 
     header.token = b'\x22\xff\xaa\xff'
     assert header.pack()[3:] == b'\x22\xff\xaa\xff'
 
@@ -156,30 +157,30 @@
 
     header.token = b'helo'
     assert header.pack()[3:] == b'helo'
 
     header.token = b'tekn'
     assert header.pack()[3:] == b'tekn'
 
-def test_packet_header_pack_full():
-    header = PacketHeader()
+def test_packet_header_pack_full() -> None:
+    header: PacketHeader = PacketHeader()
 
     header.ack = 10
     header.token = b'\xcf.\xde\x1d'
     header.num_chunks = 0
 
     header.flags.control = True
     header.flags.resend = False
     header.flags.compression = False
     header.flags.connless = False
 
     assert header.pack() == b'\x04\x0a\x00\xcf\x2e\xde\x1d'
 
-def test_packet_header_repack_all_set():
-    header = PacketHeader()
+def test_packet_header_repack_all_set() -> None:
+    header: PacketHeader = PacketHeader()
 
     header.ack = 1023
     header.token = b'\xff\xff\xff\xff'
     header.num_chunks = 255
 
     header.flags.control = True
     header.flags.resend = True
@@ -229,16 +230,16 @@
     assert header.num_chunks == 255
 
     assert header.flags.control is True
     assert header.flags.resend is True
     assert header.flags.compression is True
     assert header.flags.connless is True
 
-def test_packet_header_repack_none_set():
-    header = PacketHeader()
+def test_packet_header_repack_none_set() -> None:
+    header: PacketHeader = PacketHeader()
 
     header.ack = 0
     header.token = b'\x00\x00\x00\x00'
     header.num_chunks = 0
 
     header.flags.control = False
     header.flags.resend = False
@@ -255,16 +256,16 @@
     assert header.num_chunks == 0
 
     assert header.flags.control is False
     assert header.flags.resend is False
     assert header.flags.compression is False
     assert header.flags.connless is False
 
-def test_parse_7_close():
-    packet = parse7(b'\x04\x0a\x00\xcf\x2e\xde\x1d\04') # 0.7 close
+def test_parse_7_close() -> None:
+    packet: TwPacket = parse7(b'\x04\x0a\x00\xcf\x2e\xde\x1d\04') # 0.7 close
 
     assert packet.version == '0.7'
 
     assert packet.header.ack == 10
     assert packet.header.token == b'\xcf.\xde\x1d'
     assert packet.header.num_chunks == 0
 
@@ -272,16 +273,16 @@
     assert packet.header.flags.resend is False
     assert packet.header.flags.compression is False
     assert packet.header.flags.connless is False
 
     assert packet.messages[0].message_name == 'close'
     assert len(packet.messages) == 1
 
-def test_parse_7_close_fake_resend():
-    packet = parse7(b'\x0c\x0a\x00\xaa\xbb\xcc\xdd\04') # 0.7 close
+def test_parse_7_close_fake_resend() -> None:
+    packet: TwPacket = parse7(b'\x0c\x0a\x00\xaa\xbb\xcc\xdd\04') # 0.7 close
     #                   ^
     #                resending ctrl close
     #                probably never happens
 
     assert packet.version == '0.7'
 
     assert packet.header.ack == 10
@@ -292,16 +293,16 @@
     assert packet.header.flags.resend is True
     assert packet.header.flags.compression is False
     assert packet.header.flags.connless is False
 
     assert packet.messages[0].message_name == 'close'
     assert len(packet.messages) == 1
 
-def test_parse_7_close_fake_num_chunks():
-    packet = parse7(b'\x04\x0a\x01\xcf\xee\xde\x2d\04') # 0.7 close
+def test_parse_7_close_fake_num_chunks() -> None:
+    packet: TwPacket = parse7(b'\x04\x0a\x01\xcf\xee\xde\x2d\04') # 0.7 close
     #                          ^
     #                       1 chunk makes no sense
     #                       because control messages should
     #                       always have 0 chunks
 
     assert packet.version == '0.7'
```

### Comparing `twnet_parser-0.4.0/tests/packet_invalid_test.py` & `twnet_parser-0.5.0/tests/packet_invalid_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/packet_with_chunks7_test.py` & `twnet_parser-0.5.0/tests/packet_with_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/repack_chunks7_test.py` & `twnet_parser-0.5.0/tests/repack_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/tests/unpacker_state_test.py` & `twnet_parser-0.5.0/tests/unpacker_state_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/external/huffman.py` & `twnet_parser-0.5.0/twnet_parser/external/huffman.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/message_parser.py` & `twnet_parser-0.5.0/twnet_parser/message_parser.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/control/close.py` & `twnet_parser-0.5.0/twnet_parser/messages7/control/close.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from twnet_parser.packer import pack_str
 
 class CtrlClose(PrettyPrint):
     def __init__(
             self,
             reason: Optional[str] = None
     ) -> None:
-        self.message_name = 'close'
+        self.message_name: str = 'close'
+        self.message_id: int = 4
+
         self.reason: Optional[str] = reason
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
-    def unpack(self, data: bytes, we_are_a_client: bool = False) -> bool:
+    def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         unpacker = Unpacker(data)
         self.reason = unpacker.get_str() # TODO: this is an optional field
         return True
 
-    def pack(self) -> bytes:
+    def pack(self, we_are_a_client: bool = True) -> bytes:
         if self.reason:
             return pack_str(self.reason)
         return b''
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/control/connect.py` & `twnet_parser-0.5.0/twnet_parser/messages7/control/connect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from twnet_parser.pretty_print import PrettyPrint
 
 class CtrlConnect(PrettyPrint):
     def __init__(
             self,
             response_token: bytes = b'\xff\xff\xff\xff'
     ) -> None:
-        self.message_name = 'connect'
+        self.message_name: str = 'connect'
+        self.message_id: int = 1
+
         self.response_token: bytes = response_token
 
-    def unpack(self, data: bytes, we_are_a_client: bool = False) -> bool:
+    def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         # anti reflection attack
         if len(data) < 512:
             return False
         self.response_token = data[0:4]
         return True
 
-    def pack(self) -> bytes:
+    def pack(self, we_are_a_client: bool = True) -> bytes:
         return self.response_token + bytes(508)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/control/token.py` & `twnet_parser-0.5.0/twnet_parser/messages7/control/token.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from twnet_parser.pretty_print import PrettyPrint
 
 class CtrlToken(PrettyPrint):
     def __init__(
             self,
             response_token: bytes = b'\xff\xff\xff\xff'
     ) -> None:
-        self.message_name = 'token'
+        self.message_name: str = 'token'
+        self.message_id: int = 5
+
         self.response_token: bytes = response_token
 
-    def unpack(self, data: bytes, we_are_a_client: bool = False) -> bool:
+    def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         if not we_are_a_client:
             # anti reflection attack
             if len(data) < 512:
                 return False
         self.response_token = data[0:4]
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_call_vote.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_call_vote.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
 class MsgClCallVote(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             type: str = 'default',
             value: str = 'default',
             reason: str = 'default',
             force: bool = False
     ) -> None:
-        self.message_name = 'cl_call_vote'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_call_vote'
+        self.system_message: bool = False
+        self.message_id: int = 32
+        self.header: ChunkHeader = chunk_header
 
         self.type: str = type
         self.value: str = value
         self.reason: str = reason
         self.force: bool = force
 
     # first byte of data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_command.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_vote.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
+from twnet_parser.packer import pack_int
 
-class MsgClCommand(PrettyPrint):
+class MsgClVote(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
-            arguments: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            vote: int = 0
     ) -> None:
-        self.message_name = 'cl_command'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_vote'
+        self.system_message: bool = False
+        self.message_id: int = 31
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
-        self.arguments: str = arguments
+        self.vote: int = vote
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str(SANITIZE_CC)
-        self.arguments = unpacker.get_str(SANITIZE_CC)
+        self.vote = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_str(self.arguments)
+        return pack_int(self.vote)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_emoticon.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_emoticon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
 class MsgClEmoticon(PrettyPrint):
     def __init__(
             self,
-            emoticon: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            emoticon: int = enum7.Emoticon.OOP.value
     ) -> None:
-        self.message_name = 'cl_emoticon'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_emoticon'
+        self.system_message: bool = False
+        self.message_id: int = 30
+        self.header: ChunkHeader = chunk_header
 
         self.emoticon: int = emoticon
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.emoticon = unpacker.get_int() # TODO: this is a enum
+        self.emoticon = unpacker.get_int() # enum EMOTICON
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.emoticon)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_kill.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_ready_to_enter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgClKill(PrettyPrint):
+class MsgSvReadyToEnter(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'cl_kill'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_ready_to_enter'
+        self.system_message: bool = False
+        self.message_id: int = 8
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_ready_change.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_clear_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgClReadyChange(PrettyPrint):
+class MsgSvVoteClearOptions(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'cl_ready_change'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_clear_options'
+        self.system_message: bool = False
+        self.message_id: int = 11
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_say.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_extra_projectile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from twnet_parser.packer import pack_int
 
-class MsgClSay(PrettyPrint):
+class MsgSvExtraProjectile(PrettyPrint):
     def __init__(
             self,
-            mode: int = 0,
-            target: int = 0,
-            message: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            projectile: int = 0
     ) -> None:
-        self.message_name = 'cl_say'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_extra_projectile'
+        self.system_message: bool = False
+        self.message_id: int = 7
+        self.header: ChunkHeader = chunk_header
 
-        self.mode: int = mode
-        self.target: int = target
-        self.message: str = message
+        self.projectile: int = projectile
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.mode = unpacker.get_int() # TODO: this is a enum
-        self.target = unpacker.get_int()
-        self.message = unpacker.get_str(SANITIZE_CC)
+        self.projectile = unpacker.get_int() # TODO: this is a snapshot object
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.mode) + \
-            pack_int(self.target) + \
-            pack_str(self.message)
+        return pack_int(self.projectile)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_spectator_mode.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_spectator_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
 class MsgClSetSpectatorMode(PrettyPrint):
     def __init__(
             self,
-            spec_mode: int = 0,
+            chunk_header: ChunkHeader = ChunkHeader(),
+            spec_mode: int = enum7.Spec.FREEVIEW.value,
             spectator_id: int = 0
     ) -> None:
-        self.message_name = 'cl_set_spectator_mode'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_set_spectator_mode'
+        self.system_message: bool = False
+        self.message_id: int = 26
+        self.header: ChunkHeader = chunk_header
 
         self.spec_mode: int = spec_mode
         self.spectator_id: int = spectator_id
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.spec_mode = unpacker.get_int() # TODO: this is a enum
+        self.spec_mode = unpacker.get_int() # enum SPEC
         self.spectator_id = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.spec_mode) + \
             pack_int(self.spectator_id)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_team.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_checkpoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
-class MsgClSetTeam(PrettyPrint):
+class MsgSvCheckpoint(PrettyPrint):
     def __init__(
             self,
-            team: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            diff: int = 0
     ) -> None:
-        self.message_name = 'cl_set_team'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_checkpoint'
+        self.system_message: bool = False
+        self.message_id: int = 36
+        self.header: ChunkHeader = chunk_header
 
-        self.team: int = team
+        self.diff: int = diff
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.team = unpacker.get_int() # TODO: this is a enum
+        self.diff = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.team)
+        return pack_int(self.diff)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_skin_change.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_skin_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 from typing import Annotated
 
 class MsgClSkinChange(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
-        self.message_name = 'cl_skin_change'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_skin_change'
+        self.system_message: bool = False
+        self.message_id: int = 34
+        self.header: ChunkHeader = chunk_header
 
         self.skin_part_names = skin_part_names
         self.use_custom_colors = use_custom_colors
         self.skin_part_colors = skin_part_colors
 
     # first byte of data
     # has to be the first byte of the message payload
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_start_info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_start_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 from typing import Annotated
 
 class MsgClStartInfo(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             clan: str = 'default',
             country: int = 0,
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
-        self.message_name = 'cl_start_info'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_start_info'
+        self.system_message: bool = False
+        self.message_id: int = 27
+        self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.clan: str = clan
         self.country: int = country
         self.skin_part_names = skin_part_names
         self.use_custom_colors = use_custom_colors
         self.skin_part_colors = skin_part_colors
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_vote.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_team.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
-class MsgClVote(PrettyPrint):
+class MsgClSetTeam(PrettyPrint):
     def __init__(
             self,
-            vote: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            team: int = enum7.Team.SPECTATORS.value
     ) -> None:
-        self.message_name = 'cl_vote'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_set_team'
+        self.system_message: bool = False
+        self.message_id: int = 25
+        self.header: ChunkHeader = chunk_header
 
-        self.vote: int = vote
+        self.team: int = team
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.vote = unpacker.get_int()
+        self.team = unpacker.get_int() # enum TEAM
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.vote)
+        return pack_int(self.team)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_enter.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_enter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+import twnet_parser.enum7 as enum7
 
 class MsgDeClientEnter(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             client_id: int = 0,
-            team: int = 0
+            team: int = enum7.Team.SPECTATORS.value
     ) -> None:
-        self.message_name = 'de_client_enter'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'de_client_enter'
+        self.system_message: bool = False
+        self.message_id: int = 22
+        self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.client_id: int = client_id
         self.team: int = team
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.name = unpacker.get_str(SANITIZE_CC)
         self.client_id = unpacker.get_int()
-        self.team = unpacker.get_int() # TODO: this is a enum
+        self.team = unpacker.get_int() # enum TEAM
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
             pack_int(self.client_id) + \
             pack_int(self.team)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_leave.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_rem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from twnet_parser.packer import pack_str
 
-class MsgDeClientLeave(PrettyPrint):
+class MsgRconCmdRem(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
-            client_id: int = 0,
-            reason: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default'
     ) -> None:
-        self.message_name = 'de_client_leave'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'rcon_cmd_rem'
+        self.system_message: bool = True
+        self.message_id: int = 15
+        self.header: ChunkHeader = chunk_header
 
         self.name: str = name
-        self.client_id: int = client_id
-        self.reason: str = reason
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str(SANITIZE_CC)
-        self.client_id = unpacker.get_int()
-        self.reason = unpacker.get_str(SANITIZE_CC)
+        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_int(self.client_id) + \
-            pack_str(self.reason)
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_broadcast.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_broadcast.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
 class MsgSvBroadcast(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             message: str = 'default'
     ) -> None:
-        self.message_name = 'sv_broadcast'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_broadcast'
+        self.system_message: bool = False
+        self.message_id: int = 2
+        self.header: ChunkHeader = chunk_header
 
         self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_chat.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+import twnet_parser.enum7 as enum7
 
 class MsgSvChat(PrettyPrint):
     def __init__(
             self,
-            mode: int = 0,
+            chunk_header: ChunkHeader = ChunkHeader(),
+            mode: int = enum7.Chat.NONE.value,
             client_id: int = 0,
             target_id: int = 0,
             message: str = 'default'
     ) -> None:
-        self.message_name = 'sv_chat'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_chat'
+        self.system_message: bool = False
+        self.message_id: int = 3
+        self.header: ChunkHeader = chunk_header
 
         self.mode: int = mode
         self.client_id: int = client_id
         self.target_id: int = target_id
         self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.mode = unpacker.get_int() # TODO: this is a enum
+        self.mode = unpacker.get_int() # enum CHAT
         self.client_id = unpacker.get_int()
         self.target_id = unpacker.get_int()
         self.message = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.mode) + \
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_checkpoint.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_remove.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
-class MsgSvCheckpoint(PrettyPrint):
+class MsgSvVoteOptionRemove(PrettyPrint):
     def __init__(
             self,
-            diff: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            description: str = 'default'
     ) -> None:
-        self.message_name = 'sv_checkpoint'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_option_remove'
+        self.system_message: bool = False
+        self.message_id: int = 14
+        self.header: ChunkHeader = chunk_header
 
-        self.diff: int = diff
+        self.description: str = description
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.diff = unpacker.get_int()
+        self.description = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.diff)
+        return pack_str(self.description)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_drop.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_set.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+import twnet_parser.enum7 as enum7
 
-class MsgSvClientDrop(PrettyPrint):
+class MsgSvVoteSet(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            reason: str = 'default',
-            silent: bool = False
+            type: int = enum7.Vote.UNKNOWN.value,
+            timeout: int = 0,
+            description: str = 'default',
+            reason: str = 'default'
     ) -> None:
-        self.message_name = 'sv_client_drop'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_set'
+        self.system_message: bool = False
+        self.message_id: int = 15
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
+        self.type: int = type
+        self.timeout: int = timeout
+        self.description: str = description
         self.reason: str = reason
-        self.silent: bool = silent
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
+        self.type = unpacker.get_int() # enum VOTE
+        self.timeout = unpacker.get_int()
+        self.description = unpacker.get_str(SANITIZE_CC)
         self.reason = unpacker.get_str(SANITIZE_CC)
-        self.silent = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
-            pack_str(self.reason) + \
-            pack_int(self.silent)
+            pack_int(self.type) + \
+            pack_int(self.timeout) + \
+            pack_str(self.description) + \
+            pack_str(self.reason)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 from typing import Annotated
+import twnet_parser.enum7 as enum7
 
 class MsgSvClientInfo(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
             local: bool = False,
-            team: int = 0,
+            team: int = enum7.Team.SPECTATORS.value,
             name: str = 'default',
             clan: str = 'default',
             country: int = 0,
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0],
             silent: bool = False
     ) -> None:
-        self.message_name = 'sv_client_info'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_client_info'
+        self.system_message: bool = False
+        self.message_id: int = 18
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.local: bool = local
         self.team: int = team
         self.name: str = name
         self.clan: str = clan
         self.country: int = country
@@ -41,15 +44,15 @@
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
         self.local = unpacker.get_int() == 1
-        self.team = unpacker.get_int() # TODO: this is a enum
+        self.team = unpacker.get_int() # enum TEAM
         self.name = unpacker.get_str(SANITIZE_CC)
         self.clan = unpacker.get_str(SANITIZE_CC)
         self.country = unpacker.get_int()
         for i in range(0, 6):
             self.skin_part_names[i] = unpacker.get_str(SANITIZE_CC)
         for i in range(0, 6):
             self.use_custom_colors[i] = unpacker.get_int() == 1
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_str
 
 class MsgSvCommandInfo(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             args_format: str = 'default',
             help_text: str = 'default'
     ) -> None:
-        self.message_name = 'sv_command_info'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_command_info'
+        self.system_message: bool = False
+        self.message_id: int = 37
+        self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.args_format: str = args_format
         self.help_text: str = help_text
 
     # first byte of data
     # has to be the first byte of the message payload
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info_remove.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/map_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
 
-class MsgSvCommandInfoRemove(PrettyPrint):
+class MsgMapData(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'sv_command_info_remove'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'map_data'
+        self.system_message: bool = True
+        self.message_id: int = 3
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str(SANITIZE_CC)
+        self.data = unpacker.get_raw()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return self.data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_emoticon.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_emoticon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
 class MsgSvEmoticon(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            emoticon: int = 0
+            emoticon: int = enum7.Emoticon.OOP.value
     ) -> None:
-        self.message_name = 'sv_emoticon'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_emoticon'
+        self.system_message: bool = False
+        self.message_id: int = 10
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.emoticon: int = emoticon
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.emoticon = unpacker.get_int() # TODO: this is a enum
+        self.emoticon = unpacker.get_int() # enum EMOTICON
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
             pack_int(self.emoticon)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_extra_projectile.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/snap_empty.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
-class MsgSvExtraProjectile(PrettyPrint):
+class MsgSnapEmpty(PrettyPrint):
     def __init__(
             self,
-            projectile: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            tick: int = 0,
+            delta_tick: int = 0
     ) -> None:
-        self.message_name = 'sv_extra_projectile'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'snap_empty'
+        self.system_message: bool = True
+        self.message_id: int = 7
+        self.header: ChunkHeader = chunk_header
 
-        self.projectile: int = projectile
+        self.tick: int = tick
+        self.delta_tick: int = delta_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.projectile = unpacker.get_int() # TODO: this is a snapshot object
+        self.tick = unpacker.get_int()
+        self.delta_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.projectile)
+        return pack_int(self.tick) + \
+            pack_int(self.delta_tick)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvGameInfo(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             game_flags: int = 0,
             score_limit: int = 0,
             time_limit: int = 0,
             match_num: int = 0,
             match_current: int = 0
     ) -> None:
-        self.message_name = 'sv_game_info'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_game_info'
+        self.system_message: bool = False
+        self.message_id: int = 19
+        self.header: ChunkHeader = chunk_header
 
         self.game_flags: int = game_flags
         self.score_limit: int = score_limit
         self.time_limit: int = time_limit
         self.match_num: int = match_num
         self.match_current: int = match_current
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_msg.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_msg.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
 class MsgSvGameMsg(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'sv_game_msg'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_game_msg'
+        self.system_message: bool = False
+        self.message_id: int = 21
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_kill_msg.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_kill_msg.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvKillMsg(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             killer: int = 0,
             victim: int = 0,
             weapon: int = 0,
             mode_special: int = 0
     ) -> None:
-        self.message_name = 'sv_kill_msg'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_kill_msg'
+        self.system_message: bool = False
+        self.message_id: int = 5
+        self.header: ChunkHeader = chunk_header
 
         self.killer: int = killer
         self.victim: int = victim
         self.weapon: int = weapon
         self.mode_special: int = mode_special
 
     # first byte of data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_motd.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgSvMotd(PrettyPrint):
+class MsgRconCmd(PrettyPrint):
     def __init__(
             self,
-            message: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            cmd: str = 'default'
     ) -> None:
-        self.message_name = 'sv_motd'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'rcon_cmd'
+        self.system_message: bool = True
+        self.message_id: int = 21
+        self.header: ChunkHeader = chunk_header
 
-        self.message: str = message
+        self.cmd: str = cmd
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.message = unpacker.get_str()
+        self.cmd = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.message)
+        return pack_str(self.cmd)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_race_finish.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_race_finish.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvRaceFinish(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
             time: int = 0,
             diff: int = 0,
             record_personal: bool = False,
             record_server: bool = False
     ) -> None:
-        self.message_name = 'sv_race_finish'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_race_finish'
+        self.system_message: bool = False
+        self.message_id: int = 35
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.time: int = time
         self.diff: int = diff
         self.record_personal: bool = record_personal
         self.record_server: bool = record_server
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_ready_to_enter.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/request_map_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgSvReadyToEnter(PrettyPrint):
+class MsgRequestMapData(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'sv_ready_to_enter'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'request_map_data'
+        self.system_message: bool = True
+        self.message_id: int = 23
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_server_settings.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_server_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvServerSettings(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             kick_vote: bool = False,
             kick_min: int = 0,
             spec_vote: bool = False,
             team_lock: bool = False,
             team_balance: bool = False,
             player_slots: int = 0
     ) -> None:
-        self.message_name = 'sv_server_settings'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_server_settings'
+        self.system_message: bool = False
+        self.message_id: int = 17
+        self.header: ChunkHeader = chunk_header
 
         self.kick_vote: bool = kick_vote
         self.kick_min: int = kick_min
         self.spec_vote: bool = spec_vote
         self.team_lock: bool = team_lock
         self.team_balance: bool = team_balance
         self.player_slots: int = player_slots
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_skin_change.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_skin_change.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 from typing import Annotated
 
 class MsgSvSkinChange(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
-        self.message_name = 'sv_skin_change'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_skin_change'
+        self.system_message: bool = False
+        self.message_id: int = 33
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.skin_part_names = skin_part_names
         self.use_custom_colors = use_custom_colors
         self.skin_part_colors = skin_part_colors
 
     # first byte of data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_team.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_team.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
 class MsgSvTeam(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            team: int = 0,
+            team: int = enum7.Team.SPECTATORS.value,
             silent: bool = False,
             cooldown_tick: int = 0
     ) -> None:
-        self.message_name = 'sv_team'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_team'
+        self.system_message: bool = False
+        self.message_id: int = 4
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.team: int = team
         self.silent: bool = silent
         self.cooldown_tick: int = cooldown_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.team = unpacker.get_int() # TODO: this is a enum
+        self.team = unpacker.get_int() # enum TEAM
         self.silent = unpacker.get_int() == 1
         self.cooldown_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
             pack_int(self.team) + \
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_tune_params.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_tune_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvTuneParams(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             ground_control_speed: float = 10,
             ground_control_accel: float = 2,
             ground_friction: float = 0.5,
             ground_jump_impulse: float = 13.2,
             air_jump_impulse: float = 12,
             air_control_speed: float = 5,
             air_control_accel: float = 1.5,
@@ -37,17 +38,18 @@
             laser_reach: float = 800,
             laser_bounce_delay: float = 150,
             laser_bounce_num: float = 1,
             laser_bounce_cost: float = 0,
             player_collision: float = 1,
             player_hooking: float = 1
     ) -> None:
-        self.message_name = 'sv_tune_params'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_tune_params'
+        self.system_message: bool = False
+        self.message_id: int = 6
+        self.header: ChunkHeader = chunk_header
 
         self.ground_control_speed: float = ground_control_speed
         self.ground_control_accel: float = ground_control_accel
         self.ground_friction: float = ground_friction
         self.ground_jump_impulse: float = ground_jump_impulse
         self.air_jump_impulse: float = air_jump_impulse
         self.air_control_speed: float = air_control_speed
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_clear_options.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_kill.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgSvVoteClearOptions(PrettyPrint):
+class MsgClKill(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'sv_vote_clear_options'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_kill'
+        self.system_message: bool = False
+        self.message_id: int = 28
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_add.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_add.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_str
 
 class MsgSvVoteOptionAdd(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             description: str = 'default'
     ) -> None:
-        self.message_name = 'sv_vote_option_add'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_option_add'
+        self.system_message: bool = False
+        self.message_id: int = 13
+        self.header: ChunkHeader = chunk_header
 
         self.description: str = description
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_list_add.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/con_ready.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgSvVoteOptionListAdd(PrettyPrint):
+class MsgConReady(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'sv_vote_option_list_add'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'con_ready'
+        self.system_message: bool = True
+        self.message_id: int = 5
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_remove.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_add.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
+from twnet_parser.packer import pack_str
 
-class MsgSvVoteOptionRemove(PrettyPrint):
+class MsgRconCmdAdd(PrettyPrint):
     def __init__(
             self,
-            description: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default',
+            help: str = 'default',
+            params: str = 'default'
     ) -> None:
-        self.message_name = 'sv_vote_option_remove'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'rcon_cmd_add'
+        self.system_message: bool = True
+        self.message_id: int = 14
+        self.header: ChunkHeader = chunk_header
 
-        self.description: str = description
+        self.name: str = name
+        self.help: str = help
+        self.params: str = params
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.description = unpacker.get_str(SANITIZE_CC)
+        self.name = unpacker.get_str()
+        self.help = unpacker.get_str()
+        self.params = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.description)
+        return pack_str(self.name) + \
+            pack_str(self.help) + \
+            pack_str(self.params)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_set.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_drop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
-class MsgSvVoteSet(PrettyPrint):
+class MsgSvClientDrop(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            type: int = 0,
-            timeout: int = 0,
-            description: str = 'default',
-            reason: str = 'default'
+            reason: str = 'default',
+            silent: bool = False
     ) -> None:
-        self.message_name = 'sv_vote_set'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_client_drop'
+        self.system_message: bool = False
+        self.message_id: int = 20
+        self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
-        self.type: int = type
-        self.timeout: int = timeout
-        self.description: str = description
         self.reason: str = reason
+        self.silent: bool = silent
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.type = unpacker.get_int() # TODO: this is a enum
-        self.timeout = unpacker.get_int()
-        self.description = unpacker.get_str(SANITIZE_CC)
         self.reason = unpacker.get_str(SANITIZE_CC)
+        self.silent = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
-            pack_int(self.type) + \
-            pack_int(self.timeout) + \
-            pack_str(self.description) + \
-            pack_str(self.reason)
+            pack_str(self.reason) + \
+            pack_int(self.silent)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_status.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgSvVoteStatus(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             yes: int = 0,
             no: int = 0,
             pass_: int = 0,
             total: int = 0
     ) -> None:
-        self.message_name = 'sv_vote_status'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_status'
+        self.system_message: bool = False
+        self.message_id: int = 16
+        self.header: ChunkHeader = chunk_header
 
         self.yes: int = yes
         self.no: int = no
         self.pass_: int = pass_
         self.total: int = total
 
     # first byte of data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_weapon_pickup.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/server_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
 
-class MsgSvWeaponPickup(PrettyPrint):
+class MsgServerInfo(PrettyPrint):
     def __init__(
             self,
-            weapon: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'sv_weapon_pickup'
-        self.system_message = False
-        self.header: ChunkHeader
+        self.message_name: str = 'server_info'
+        self.system_message: bool = True
+        self.message_id: int = 4
+        self.header: ChunkHeader = chunk_header
 
-        self.weapon: int = weapon
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.weapon = unpacker.get_int() # TODO: this is a enum
+        self.data = unpacker.get_raw()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.weapon)
+        return self.data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/con_ready.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/enter_game.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgConReady(PrettyPrint):
+class MsgEnterGame(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'con_ready'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'enter_game'
+        self.system_message: bool = True
+        self.message_id: int = 19
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import pack_str
 
-class MsgInfo(PrettyPrint):
+class MsgRconAuth(PrettyPrint):
     def __init__(
             self,
-            version: str = 'default',
-            password: str = '',
-            client_version: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            password: str = 'default'
     ) -> None:
-        self.message_name = 'info'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'rcon_auth'
+        self.system_message: bool = True
+        self.message_id: int = 22
+        self.header: ChunkHeader = chunk_header
 
-        self.version: str = version
         self.password: str = password
-        self.client_version: int = client_version
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.version = unpacker.get_str()
-        self.password = unpacker.get_str() # TODO: optionals
-        self.client_version = unpacker.get_int() # TODO: optionals
+        self.password = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.version) + \
-            pack_str(self.password) + \
-            pack_int(self.client_version)
+        return pack_str(self.password)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/input.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/input.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgInput(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             ack_snapshot: int = 0,
             intended_tick: int = 0,
             input_size: int = 0,
             input: int = 0
     ) -> None:
-        self.message_name = 'input'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'input'
+        self.system_message: bool = True
+        self.message_id: int = 20
+        self.header: ChunkHeader = chunk_header
 
         self.ack_snapshot: int = ack_snapshot
         self.intended_tick: int = intended_tick
         self.input_size: int = input_size
         self.input: int = input
 
     # first byte of data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/input_timing.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/input_timing.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
 class MsgInputTiming(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             input_pred_tick: int = 0,
             time_left: int = 0
     ) -> None:
-        self.message_name = 'input_timing'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'input_timing'
+        self.system_message: bool = True
+        self.message_id: int = 10
+        self.header: ChunkHeader = chunk_header
 
         self.input_pred_tick: int = input_pred_tick
         self.time_left: int = time_left
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/map_change.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/map_change.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int, pack_str
+from typing import Annotated
 
 class MsgMapChange(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             crc: int = 0,
             size: int = 0,
             num_response_chunks_per_request: int = 0,
             chunk_size: int = 0,
-            sha256: bytes = b'\x00'
+            sha256: Annotated[bytes, 32] = bytes(32)
     ) -> None:
-        self.message_name = 'map_change'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'map_change'
+        self.system_message: bool = True
+        self.message_id: int = 2
+        self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.crc: int = crc
         self.size: int = size
         self.num_response_chunks_per_request: int = num_response_chunks_per_request
         self.chunk_size: int = chunk_size
-        self.sha256: bytes = sha256
+        self.sha256: Annotated[bytes, 32] = sha256
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.name = unpacker.get_str()
         self.crc = unpacker.get_int()
         self.size = unpacker.get_int()
         self.num_response_chunks_per_request = unpacker.get_int()
         self.chunk_size = unpacker.get_int()
-        self.sha256 = unpacker.get_raw()
+        self.sha256 = unpacker.get_raw(32)
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
             pack_int(self.crc) + \
             pack_int(self.size) + \
             pack_int(self.num_response_chunks_per_request) + \
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/map_data.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_add.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import pack_str
 
-class MsgMapData(PrettyPrint):
+class MsgMaplistEntryAdd(PrettyPrint):
     def __init__(
             self,
-            data: bytes = b'\x00'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default'
     ) -> None:
-        self.message_name = 'map_data'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'maplist_entry_add'
+        self.system_message: bool = True
+        self.message_id: int = 29
+        self.header: ChunkHeader = chunk_header
 
-        self.data: bytes = data
+        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.data = unpacker.get_raw()
+        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return self.data
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_add.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_ready_change.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
-from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
 
-class MsgMaplistEntryAdd(PrettyPrint):
+class MsgClReadyChange(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'maplist_entry_add'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_ready_change'
+        self.system_message: bool = False
+        self.message_id: int = 29
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
-        unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return b''
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_rem.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_list_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
-from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
 
-class MsgMaplistEntryRem(PrettyPrint):
+class MsgSvVoteOptionListAdd(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'maplist_entry_rem'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_vote_option_list_add'
+        self.system_message: bool = False
+        self.message_id: int = 12
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
-        unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return b''
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/ping.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/ping_reply.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgPing(PrettyPrint):
+class MsgPingReply(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'ping'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'ping_reply'
+        self.system_message: bool = True
+        self.message_id: int = 27
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/ping_reply.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/ready.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgPingReply(PrettyPrint):
+class MsgReady(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'ping_reply'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'ready'
+        self.system_message: bool = True
+        self.message_id: int = 18
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_line.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgRconAuth(PrettyPrint):
+class MsgRconLine(PrettyPrint):
     def __init__(
             self,
-            password: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            line: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_auth'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'rcon_line'
+        self.system_message: bool = True
+        self.message_id: int = 13
+        self.header: ChunkHeader = chunk_header
 
-        self.password: str = password
+        self.line: str = line
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.password = unpacker.get_str()
+        self.line = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.password)
+        return pack_str(self.line)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_off.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/ping.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgRconAuthOff(PrettyPrint):
+class MsgPing(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name = 'rcon_auth_off'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'ping'
+        self.system_message: bool = True
+        self.message_id: int = 26
+        self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_on.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info_remove.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
+from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
-class MsgRconAuthOn(PrettyPrint):
+class MsgSvCommandInfoRemove(PrettyPrint):
     def __init__(
             self,
-
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_auth_on'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_command_info_remove'
+        self.system_message: bool = False
+        self.message_id: int = 38
+        self.header: ChunkHeader = chunk_header
 
+        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
+        unpacker = Unpacker(data)
+        self.name = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return b''
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_weapon_pickup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import pack_int
+import twnet_parser.enum7 as enum7
 
-class MsgRconCmd(PrettyPrint):
+class MsgSvWeaponPickup(PrettyPrint):
     def __init__(
             self,
-            cmd: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            weapon: int = enum7.Weapon.HAMMER.value
     ) -> None:
-        self.message_name = 'rcon_cmd'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_weapon_pickup'
+        self.system_message: bool = False
+        self.message_id: int = 9
+        self.header: ChunkHeader = chunk_header
 
-        self.cmd: str = cmd
+        self.weapon: int = weapon
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.cmd = unpacker.get_str()
+        self.weapon = unpacker.get_int() # enum WEAPON
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.cmd)
+        return pack_int(self.weapon)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_add.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_say.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+import twnet_parser.enum7 as enum7
 
-class MsgRconCmdAdd(PrettyPrint):
+class MsgClSay(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
-            help: str = 'default',
-            params: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            mode: int = enum7.Chat.NONE.value,
+            target: int = 0,
+            message: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_cmd_add'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_say'
+        self.system_message: bool = False
+        self.message_id: int = 24
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
-        self.help: str = help
-        self.params: str = params
+        self.mode: int = mode
+        self.target: int = target
+        self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
-        self.help = unpacker.get_str()
-        self.params = unpacker.get_str()
+        self.mode = unpacker.get_int() # enum CHAT
+        self.target = unpacker.get_int()
+        self.message = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_str(self.help) + \
-            pack_str(self.params)
+        return pack_int(self.mode) + \
+            pack_int(self.target) + \
+            pack_str(self.message)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_rem.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_motd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgRconCmdRem(PrettyPrint):
+class MsgSvMotd(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            message: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_cmd_rem'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'sv_motd'
+        self.system_message: bool = False
+        self.message_id: int = 1
+        self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
+        self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.message = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return pack_str(self.message)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_line.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
-class MsgRconLine(PrettyPrint):
+class MsgClCommand(PrettyPrint):
     def __init__(
             self,
-            line: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default',
+            arguments: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_line'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'cl_command'
+        self.system_message: bool = False
+        self.message_id: int = 39
+        self.header: ChunkHeader = chunk_header
 
-        self.line: str = line
+        self.name: str = name
+        self.arguments: str = arguments
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.line = unpacker.get_str()
+        self.name = unpacker.get_str(SANITIZE_CC)
+        self.arguments = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.line)
+        return pack_str(self.name) + \
+            pack_str(self.arguments)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/server_info.py` & `twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_leave.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
-class MsgServerInfo(PrettyPrint):
+class MsgDeClientLeave(PrettyPrint):
     def __init__(
             self,
-            data: bytes = b'\x00'
+            chunk_header: ChunkHeader = ChunkHeader(),
+            name: str = 'default',
+            client_id: int = 0,
+            reason: str = 'default'
     ) -> None:
-        self.message_name = 'server_info'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'de_client_leave'
+        self.system_message: bool = False
+        self.message_id: int = 23
+        self.header: ChunkHeader = chunk_header
 
-        self.data: bytes = data
+        self.name: str = name
+        self.client_id: int = client_id
+        self.reason: str = reason
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.data = unpacker.get_raw()
+        self.name = unpacker.get_str(SANITIZE_CC)
+        self.client_id = unpacker.get_int()
+        self.reason = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return self.data
+        return pack_str(self.name) + \
+            pack_int(self.client_id) + \
+            pack_str(self.reason)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/snap.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/snap.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 from typing import Optional
 
 class MsgSnap(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             tick: int = 0,
             delta_tick: int = 0,
             num_parts: int = 0,
             part: int = 0,
             crc: int = 0,
             data_size: Optional[int] = None,
             data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'snap'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'snap'
+        self.system_message: bool = True
+        self.message_id: int = 6
+        self.header: ChunkHeader = chunk_header
 
         self.tick: int = tick
         self.delta_tick: int = delta_tick
         self.num_parts: int = num_parts
         self.part: int = part
         self.crc: int = crc
         self.data_size: int = data_size if data_size else len(data)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/snap_empty.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import pack_int, pack_str
 
-class MsgSnapEmpty(PrettyPrint):
+class MsgInfo(PrettyPrint):
     def __init__(
             self,
-            tick: int = 0,
-            delta_tick: int = 0
+            chunk_header: ChunkHeader = ChunkHeader(),
+            version: str = 'default',
+            password: str = '',
+            client_version: int = 0
     ) -> None:
-        self.message_name = 'snap_empty'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'info'
+        self.system_message: bool = True
+        self.message_id: int = 1
+        self.header: ChunkHeader = chunk_header
 
-        self.tick: int = tick
-        self.delta_tick: int = delta_tick
+        self.version: str = version
+        self.password: str = password
+        self.client_version: int = client_version
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.tick = unpacker.get_int()
-        self.delta_tick = unpacker.get_int()
+        self.version = unpacker.get_str()
+        self.password = unpacker.get_str() # TODO: optionals
+        self.client_version = unpacker.get_int() # TODO: optionals
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.tick) + \
-            pack_int(self.delta_tick)
+        return pack_str(self.version) + \
+            pack_str(self.password) + \
+            pack_int(self.client_version)
```

### Comparing `twnet_parser-0.4.0/twnet_parser/messages7/system/snap_single.py` & `twnet_parser-0.5.0/twnet_parser/messages7/system/snap_single.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 from typing import Optional
 
 class MsgSnapSingle(PrettyPrint):
     def __init__(
             self,
+            chunk_header: ChunkHeader = ChunkHeader(),
             tick: int = 0,
             delta_tick: int = 0,
             crc: int = 0,
             data_size: Optional[int] = None,
             data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'snap_single'
-        self.system_message = True
-        self.header: ChunkHeader
+        self.message_name: str = 'snap_single'
+        self.system_message: bool = True
+        self.message_id: int = 8
+        self.header: ChunkHeader = chunk_header
 
         self.tick: int = tick
         self.delta_tick: int = delta_tick
         self.crc: int = crc
         self.data_size: int = data_size if data_size else len(data)
         self.data: bytes = data
```

### Comparing `twnet_parser-0.4.0/twnet_parser/msg7.py` & `twnet_parser-0.5.0/twnet_parser/msg7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/msg_matcher/control7.py` & `twnet_parser-0.5.0/twnet_parser/msg_matcher/control7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/msg_matcher/game7.py` & `twnet_parser-0.5.0/twnet_parser/msg_matcher/game7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/msg_matcher/system7.py` & `twnet_parser-0.5.0/twnet_parser/msg_matcher/system7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/packer.py` & `twnet_parser-0.5.0/twnet_parser/packer.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/twnet_parser/packet.py` & `twnet_parser-0.5.0/twnet_parser/packet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 
-from typing import Union
-from typing import cast
+from typing import Union, cast, Optional
 
-from twnet_parser.packer import Unpacker
+from twnet_parser.packer import Unpacker, pack_int
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.message_parser import MessageParser
 from twnet_parser.net_message import NetMessage
 from twnet_parser.ctrl_message import CtrlMessage
 from twnet_parser.chunk_header import ChunkHeader, ChunkFlags
 from twnet_parser.msg_matcher.control7 import match_control7
 from twnet_parser.constants import NET_MAX_SEQUENCE
@@ -23,40 +22,45 @@
 
 CHUNKFLAG7_VITAL = 1
 CHUNKFLAG7_RESEND = 2
 
 PACKET_HEADER7_SIZE = 7
 
 class PacketFlags7(PrettyPrint):
-    def __init__(self):
-        self.control = False
-        self.resend = False
-        self.compression = False
-        self.connless = False
+    def __init__(self) -> None:
+        self.control: Optional[bool] = None
+        self.resend: Optional[bool] = None
+        self.compression: Optional[bool] = None
+        self.connless: Optional[bool] = None
 
 class PacketFlags6(PrettyPrint):
-    def __init__(self):
-        self.token = False
-        self.control = False
-        self.resend = False
-        self.compression = False
-        self.connless = False
+    def __init__(self) -> None:
+        self.token: Optional[bool] = None
+        self.control: Optional[bool] = None
+        self.resend: Optional[bool] = None
+        self.compression: Optional[bool] = None
+        self.connless: Optional[bool] = None
 
 class PacketHeader(PrettyPrint):
     def __init__(
             self,
             flags: PacketFlags7 = PacketFlags7(),
             ack: int = 0,
             token: bytes = b'\xff\xff\xff\xff',
-            num_chunks: int = 0
+            num_chunks: Optional[int] = None
     ) -> None:
+        """
+        If num_chunks is not set it will count
+        the messages it was given when
+        the pack() method is called
+        """
         self.flags: PacketFlags7 = flags
         self.ack: int = ack % NET_MAX_SEQUENCE
         self.token: bytes = token
-        self.num_chunks: int = num_chunks
+        self.num_chunks: Optional[int] = num_chunks
 
     def pack(self) -> bytes:
         """
         Generate 7 byte teeworlds 0.7 packet header
         based on the current instance variable
         values.
 
@@ -79,28 +83,63 @@
             flags |= PACKETFLAG7_CONTROL
         if self.flags.resend:
             flags |= PACKETFLAG7_RESEND
         if self.flags.compression:
             flags |= PACKETFLAG7_COMPRESSION
         if self.flags.connless:
             flags |= PACKETFLAG7_CONNLESS
+        if self.num_chunks is None:
+            self.num_chunks = 0
         return bytes([ \
             ((flags << 2)&0xfc) | ((self.ack>>8)&0x03), \
             self.ack&0xff, \
             self.num_chunks \
         ]) + self.token
 
 class TwPacket(PrettyPrint):
     def __init__(self) -> None:
         self.version: str = 'unknown'
         self.payload_raw: bytes = b''
         self.payload_decompressed: bytes = b''
         self.header: PacketHeader = PacketHeader()
         self.messages: list[Union[CtrlMessage, NetMessage]] = []
 
+    def pack(self, we_are_a_client = True) -> bytes:
+        payload: bytes = b''
+        msg: Union[CtrlMessage, NetMessage]
+        is_control: bool = False
+        for msg in self.messages:
+            # TODO: this is super ugly
+            # revist https://gitlab.com/teeworlds-network/twnet_parser/-/issues/1
+            # we can not check isinstance() not sure why
+            # maybe because CtrlMessage and NetMessage are no actual classes
+            # but just ducktyping helpers
+            if not hasattr(msg, 'system_message'):
+                is_control = True
+                msg = cast(CtrlMessage, msg)
+                payload += pack_int(msg.message_id)
+                payload += msg.pack(we_are_a_client)
+            else:
+                msg = cast(NetMessage, msg)
+                msg_payload: bytes = pack_int((msg.message_id<<1)|(int)(msg.system_message))
+                msg_payload += msg.pack()
+                if msg.header.size is None:
+                    msg.header.size = len(msg_payload)
+                payload += msg.header.pack()
+                payload += msg_payload
+        if self.header.num_chunks is None:
+            if is_control:
+                self.header.num_chunks = 0
+            else:
+                self.header.num_chunks = len(self.messages)
+        if is_control:
+            if self.header.flags.control is None:
+                self.header.flags.control = True
+        return self.header.pack() + payload
+
 class PacketHeaderParser7():
     def parse_flags7(self, data: bytes) -> PacketFlags7:
         # FFFF FFaa
         flag_bits = (data[0] & 0xfc) >> 2
         flags = PacketFlags7()
         flags.control = (flag_bits & PACKETFLAG7_CONTROL) != 0
         flags.resend = (flag_bits & PACKETFLAG7_RESEND) != 0
@@ -157,14 +196,16 @@
     # first byte of a message chunk
     # NOT the whole packet with packet header
     def get_messages(self, data: bytes) -> list[NetMessage]:
         messages: list[NetMessage] = []
         i = 0
         while i < len(data):
             msg = self.get_message(data[i:])
+            if msg.header.size is None:
+                raise ValueError('header size is not set')
             i += msg.header.size + 2 # header + msg id = 3
             if msg.header.flags.vital:
                 i += 1
             messages.append(msg)
         return messages
 
     # the first byte of data has to be the
@@ -209,9 +250,9 @@
                 list[Union[CtrlMessage, NetMessage]],
                 self.get_messages(pck.payload_decompressed))
         return pck
 
 def parse6(data: bytes) -> TwPacket:
     raise NotImplementedError()
 
-def parse7(data: bytes, we_are_a_client: bool = False) -> TwPacket:
+def parse7(data: bytes, we_are_a_client: bool = True) -> TwPacket:
     return PacketParser().parse7(data, we_are_a_client)
```

### Comparing `twnet_parser-0.4.0/twnet_parser.egg-info/PKG-INFO` & `twnet_parser-0.5.0/twnet_parser.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet-parser
-Version: 0.4.0
+Version: 0.5.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -46,19 +46,19 @@
 
 ## Features
 
 | Feature                        | Status             |
 | ------------------------------ | ------------------ |
 | Deserialize 0.7 packet headers | :heavy_check_mark: |
 | Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 80%                |
+| Deserialize 0.7 messages       | 85%                |
 | Deserialize 0.7 snapshots      |                    |
 | Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    |                    |
-| Serialize 0.7 messages         | 80%                |
+| Serialize 0.7 chunk headers    | :heavy_check_mark: |
+| Serialize 0.7 messages         | 85%                |
 | Deserialize 0.6 packet headers |                    |
 | Deserialize 0.6 chunk headers  |                    |
 | Deserialize 0.6 messages       |                    |
 | Deserialize 0.6 snapshots      |                    |
 | Serialize 0.6 packet headers   |                    |
 | Serialize 0.6 chunk headers    |                    |
 | Serialize 0.6 messages         |                    |
@@ -81,14 +81,75 @@
 If you want to build something with this library
 you do have to understand how the protocol works
 and when the client and server have to send what.
 
 This [protocol documentation](https://chillerdragon.github.io/teeworlds-protocol/index.html)
 should get you started to understand the basics.
 
+## Convenient defaults and fully customizable
+
+```python
+from twnet_parser.packet import TwPacket
+from twnet_parser.messages7.game.cl_call_vote import MsgClCallVote
+
+"""
+The call to packet.pack() generates
+a valid byte array that can be sent as an udp payload
+
+It uses default values for things like:
+ security token, acknowledge number, packet flags,
+ chunk header (flags, size, seq),
+ vote type, vote value, vote reason, vote force
+
+It computes a valid chunk header size field based
+on the payload length.
+
+It sets the correct num chunks field in the packet header
+based on the amount of messages you added (1 in this case)
+
+While this has all fields set that packet would be dropped by a vanilla
+implementation because the security token and sequence number is wrong.
+So you have to take care of those your self.
+"""
+packet = TwPacket()
+msg = MsgClCallVote()
+packet.messages.append(msg)
+packet.pack() # => b'\x00\x00\x01\xff\xff\xff\xff\x00\x00\x80\x01default\x00default\x00default\x00\x00'
+
+
+
+"""
+Here we also send a Call vote message.
+But this time we set a security token and a few other fields.
+
+Note that we set num_chunks to 6 which is wrong because
+we only send one message (MsgClCallVote).
+But this library allows you to do so.
+And it will not compute the correct amount.
+But use your explicitly set wrong one instead.
+
+This allows you to have full control and craft any kind of packet.
+May it be correct or not.
+"""
+packet = TwPacket()
+packet.header.token = b'\x48\x1f\x93\xd7'
+packet.header.num_chunks = 6
+packet.header.ack = 638
+packet.header.flags.control = False
+packet.header.flags.compression = False
+msg = MsgClCallVote()
+msg.header.seq = 10
+msg.type = 'option'
+msg.value = 'test'
+msg.reason = ''
+msg.force = False
+packet.messages.append(msg)
+packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
```

### Comparing `twnet_parser-0.4.0/twnet_parser.egg-info/SOURCES.txt` & `twnet_parser-0.5.0/twnet_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+examples/print_pcap_files/print_pcap_files.py
 scripts/generate_messages.py
 tests/__init__.py
 tests/control_packets7_test.py
 tests/ctrl_packets_test.py
 tests/int_packer_test.py
 tests/invalid_packet_header7_test.py
 tests/packet_header6_test.py
@@ -15,14 +16,15 @@
 tests/repack_chunks7_test.py
 tests/unpacker_state_test.py
 tests/msg7/sv_tune_params_test.py
 twnet_parser/__init__.py
 twnet_parser/chunk_header.py
 twnet_parser/constants.py
 twnet_parser/ctrl_message.py
+twnet_parser/enum7.py
 twnet_parser/message_parser.py
 twnet_parser/msg7.py
 twnet_parser/net_message.py
 twnet_parser/packer.py
 twnet_parser/packet.py
 twnet_parser/pretty_print.py
 twnet_parser.egg-info/PKG-INFO
```

### Comparing `twnet_parser-0.4.0/venv/bin/rst2html.py` & `twnet_parser-0.5.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2html4.py` & `twnet_parser-0.5.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2html5.py` & `twnet_parser-0.5.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2latex.py` & `twnet_parser-0.5.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2man.py` & `twnet_parser-0.5.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2odt.py` & `twnet_parser-0.5.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2odt_prepstyles.py` & `twnet_parser-0.5.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2pseudoxml.py` & `twnet_parser-0.5.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2s5.py` & `twnet_parser-0.5.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2xetex.py` & `twnet_parser-0.5.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rst2xml.py` & `twnet_parser-0.5.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.4.0/venv/bin/rstpep2html.py` & `twnet_parser-0.5.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

