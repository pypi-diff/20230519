# Comparing `tmp/twnet_parser-0.6.0.tar.gz` & `tmp/twnet_parser-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twnet_parser-0.6.0.tar", last modified: Mon May  8 07:52:24 2023, max compression
+gzip compressed data, was "twnet_parser-0.7.0.tar", last modified: Fri May 19 07:47:26 2023, max compression
```

## Comparing `twnet_parser-0.6.0.tar` & `twnet_parser-0.7.0.tar`

### file list

```diff
@@ -1,136 +1,152 @@
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.6.0/LICENSE.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6172 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5439 2023-05-07 13:09:43.000000 twnet_parser-0.6.0/README.md
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.196052 twnet_parser-0.6.0/examples/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.199385 twnet_parser-0.6.0/examples/download_map/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1693 2023-05-08 07:48:02.000000 twnet_parser-0.6.0/examples/download_map/download_map.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.199385 twnet_parser-0.6.0/examples/print_pcap_files/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      680 2023-04-09 15:01:20.000000 twnet_parser-0.6.0/examples/print_pcap_files/print_pcap_files.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.6.0/pyproject.toml
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.199385 twnet_parser-0.6.0/scripts/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)    27976 2023-04-16 14:48:58.000000 twnet_parser-0.6.0/scripts/generate_messages.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/setup.cfg
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.202718 twnet_parser-0.6.0/tests/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.6.0/tests/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.6.0/tests/control_packets7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.6.0/tests/ctrl_packets_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.6.0/tests/int_packer_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.6.0/tests/invalid_packet_header7_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.202718 twnet_parser-0.6.0/tests/msg7/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.6.0/tests/msg7/sv_tune_params_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.6.0/tests/packet_header6_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9813 2023-04-16 09:39:23.000000 twnet_parser-0.6.0/tests/packet_header7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.6.0/tests/packet_invalid_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.6.0/tests/packet_with_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.6.0/tests/repack_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.6.0/tests/unpacker_state_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.202718 twnet_parser-0.6.0/twnet_parser/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1717 2023-05-07 12:05:43.000000 twnet_parser-0.6.0/twnet_parser/chunk_header.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       51 2023-05-07 11:03:40.000000 twnet_parser-0.6.0/twnet_parser/constants.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      256 2023-04-30 10:39:09.000000 twnet_parser-0.6.0/twnet_parser/ctrl_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/enum7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.202718 twnet_parser-0.6.0/twnet_parser/external/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/external/huffman.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/message_parser.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.199385 twnet_parser-0.6.0/twnet_parser/messages7/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.206051 twnet_parser-0.6.0/twnet_parser/messages7/control/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      363 2023-04-30 10:43:30.000000 twnet_parser-0.6.0/twnet_parser/messages7/control/accept.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      879 2023-04-30 11:05:40.000000 twnet_parser-0.6.0/twnet_parser/messages7/control/close.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-04-30 10:43:52.000000 twnet_parser-0.6.0/twnet_parser/messages7/control/connect.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      370 2023-04-30 10:44:02.000000 twnet_parser-0.6.0/twnet_parser/messages7/control/keep_alive.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      754 2023-04-30 10:41:20.000000 twnet_parser-0.6.0/twnet_parser/messages7/control/token.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.209385 twnet_parser-0.6.0/twnet_parser/messages7/game/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1434 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_call_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1132 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_command.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      690 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_kill.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      705 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_ready_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1314 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_say.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_set_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1804 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2251 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_start_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      918 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/cl_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1337 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/de_client_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/de_client_leave.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      950 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_broadcast.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1487 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_chat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      930 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_checkpoint.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_client_drop.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2916 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_client_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1327 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_command_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      978 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_command_info_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1177 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1004 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_extra_projectile.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1643 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_game_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      697 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_game_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1390 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_kill_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      940 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_motd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1606 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_race_finish.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      707 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_ready_to_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1818 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_server_settings.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1961 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1477 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7615 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_tune_params.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_clear_options.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1005 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      719 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1669 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_set.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1322 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_status.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/game/sv_weapon_pickup.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/twnet_parser/messages7/system/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      692 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/con_ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/enter_game.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1331 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1464 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/input.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1139 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/input_timing.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1833 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/map_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      877 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/maplist_entry_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/maplist_entry_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      684 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/ping.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/ping_reply.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      949 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      700 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth_off.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      698 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth_on.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      922 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1224 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      934 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      929 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_line.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      686 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      706 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/request_map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/server_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1861 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/snap.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1084 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/snap_empty.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1585 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/messages7/system/snap_single.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/msg7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/twnet_parser/msg_matcher/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/msg_matcher/control7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/msg_matcher/game7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-05-08 06:58:07.000000 twnet_parser-0.6.0/twnet_parser/msg_matcher/system7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      295 2023-04-16 13:57:22.000000 twnet_parser-0.6.0/twnet_parser/net_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.6.0/twnet_parser/packer.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9326 2023-05-08 07:50:38.000000 twnet_parser-0.6.0/twnet_parser/packet.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.6.0/twnet_parser/pretty_print.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.202718 twnet_parser-0.6.0/twnet_parser.egg-info/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6172 2023-05-08 07:52:24.000000 twnet_parser-0.6.0/twnet_parser.egg-info/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4392 2023-05-08 07:52:24.000000 twnet_parser-0.6.0/twnet_parser.egg-info/SOURCES.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-05-08 07:52:24.000000 twnet_parser-0.6.0/twnet_parser.egg-info/dependency_links.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-05-08 07:52:24.000000 twnet_parser-0.6.0/twnet_parser.egg-info/top_level.txt
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.199385 twnet_parser-0.6.0/venv/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:52:24.212718 twnet_parser-0.6.0/venv/bin/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2html.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2man.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-05-07 10:41:18.000000 twnet_parser-0.6.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.7.0/LICENSE.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6415 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5682 2023-05-13 14:22:02.000000 twnet_parser-0.7.0/README.md
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/download_map/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     4656 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/examples/download_map/download_map.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/print_pcap_files/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      681 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/examples/print_pcap_files/print_pcap_files.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.7.0/pyproject.toml
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/scripts/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)    46929 2023-05-19 07:45:51.000000 twnet_parser-0.7.0/scripts/generate_messages.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/setup.cfg
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/tests/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.7.0/tests/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.7.0/tests/control_packets7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.7.0/tests/ctrl_packets_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-05-09 13:53:12.000000 twnet_parser-0.7.0/tests/int_packer_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.7.0/tests/invalid_packet_header7_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/tests/msg7/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.7.0/tests/msg7/sv_tune_params_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.7.0/tests/packet_header6_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9816 2023-05-09 18:37:49.000000 twnet_parser-0.7.0/tests/packet_header7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.7.0/tests/packet_invalid_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.7.0/tests/packet_with_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.7.0/tests/repack_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7972 2023-05-10 09:03:48.000000 twnet_parser-0.7.0/tests/unpacker_state_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1717 2023-05-07 12:05:43.000000 twnet_parser-0.7.0/twnet_parser/chunk_header.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      278 2023-05-09 10:04:55.000000 twnet_parser-0.7.0/twnet_parser/connless_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       98 2023-05-09 15:59:50.000000 twnet_parser-0.7.0/twnet_parser/constants.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      302 2023-05-09 09:32:18.000000 twnet_parser-0.7.0/twnet_parser/ctrl_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/enum7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser/external/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/external/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      322 2023-05-10 09:59:05.000000 twnet_parser-0.7.0/twnet_parser/master_server.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/message_parser.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/twnet_parser/messages7/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.119950 twnet_parser-0.7.0/twnet_parser/messages7/connless/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      882 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_check.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_error.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      641 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_ok.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      651 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_response.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      903 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/heartbeat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2810 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      997 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/list.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      644 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_list.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.119950 twnet_parser-0.7.0/twnet_parser/messages7/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      448 2023-05-09 09:39:14.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      946 2023-05-09 09:39:20.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      732 2023-05-09 09:39:30.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      455 2023-05-09 09:39:40.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      839 2023-05-09 09:39:50.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/messages7/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1523 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1221 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_command.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      779 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      794 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_ready_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1403 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1301 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1087 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1875 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2322 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1007 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1426 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_leave.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1039 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1576 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1019 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_checkpoint.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_drop.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2987 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1416 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1067 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1266 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1093 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1732 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1479 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1029 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1695 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_race_finish.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      796 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1907 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_server_settings.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2032 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1566 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7704 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      805 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1094 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      808 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1100 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1758 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1411 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1106 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/messages7/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      783 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1422 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1555 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1230 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1906 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      968 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      775 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1040 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      791 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_off.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      789 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_on.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1013 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1025 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      777 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      797 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      974 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/server_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2021 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1175 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1658 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap_single.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2304 2023-05-12 15:10:15.000000 twnet_parser-0.7.0/twnet_parser/msg7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/msg_matcher/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2525 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/connless7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-05-19 07:45:11.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/control7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/game7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/system7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      348 2023-05-09 09:36:25.000000 twnet_parser-0.7.0/twnet_parser/net_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6333 2023-05-10 10:14:10.000000 twnet_parser-0.7.0/twnet_parser/packer.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    10665 2023-05-10 10:30:42.000000 twnet_parser-0.7.0/twnet_parser/packet.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/pretty_print.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      742 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/twnet_parser/snapshot7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser.egg-info/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6415 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5026 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/top_level.txt
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/venv/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/venv/bin/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rstpep2html.py
```

### Comparing `twnet_parser-0.6.0/LICENSE.txt` & `twnet_parser-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/PKG-INFO` & `twnet_parser-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet_parser
-Version: 0.6.0
+Version: 0.7.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -42,23 +42,26 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                    | 0.7                | 0.6                |
-| -------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers | :heavy_check_mark: |                    |
-| Deserialize chunk headers  | :heavy_check_mark: |                    |
-| Deserialize messages       | 85%                |                    |
-| Deserialize snapshots      |                    |                    |
-| Serialize packet headers   | :heavy_check_mark: |                    |
-| Serialize chunk headers    | :heavy_check_mark: |                    |
-| Serialize messages         | 85%                |                    |
+| Feature                      | 0.7                | 0.6                |
+| ---------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers   | :heavy_check_mark: |                    |
+| Deserialize chunk headers    | :heavy_check_mark: |                    |
+| Deserialize messages         | 85%                |                    |
+| Deserialize snapshots        |                    |                    |
+| Deserialize connless packets | :heavy_check_mark: |                    |
+| Serialize packet headers     | :heavy_check_mark: |                    |
+| Serialize chunk headers      | :heavy_check_mark: |                    |
+| Serialize messages           | 85%                |                    |
+| Serialize snapshots          |                    |                    |
+| Serialize connless packets   | :heavy_check_mark: |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.6.0/README.md` & `twnet_parser-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,26 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                    | 0.7                | 0.6                |
-| -------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers | :heavy_check_mark: |                    |
-| Deserialize chunk headers  | :heavy_check_mark: |                    |
-| Deserialize messages       | 85%                |                    |
-| Deserialize snapshots      |                    |                    |
-| Serialize packet headers   | :heavy_check_mark: |                    |
-| Serialize chunk headers    | :heavy_check_mark: |                    |
-| Serialize messages         | 85%                |                    |
+| Feature                      | 0.7                | 0.6                |
+| ---------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers   | :heavy_check_mark: |                    |
+| Deserialize chunk headers    | :heavy_check_mark: |                    |
+| Deserialize messages         | 85%                |                    |
+| Deserialize snapshots        |                    |                    |
+| Deserialize connless packets | :heavy_check_mark: |                    |
+| Serialize packet headers     | :heavy_check_mark: |                    |
+| Serialize chunk headers      | :heavy_check_mark: |                    |
+| Serialize messages           | 85%                |                    |
+| Serialize snapshots          |                    |                    |
+| Serialize connless packets   | :heavy_check_mark: |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.6.0/examples/print_pcap_files/print_pcap_files.py` & `twnet_parser-0.7.0/examples/print_pcap_files/print_pcap_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import sys
 
 import dpkt
 import twnet_parser.packet
 
 def print_tw_packets(pcap):
```

### Comparing `twnet_parser-0.6.0/scripts/generate_messages.py` & `twnet_parser-0.7.0/scripts/generate_messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python3
 
 import os
 import json
 
 from typing import \
-    TypedDict, Literal, Optional, Dict, Union, TextIO
+    TypedDict, Literal, Optional, Dict, Union, TextIO, Annotated
+
+KINDCONLESS = Literal[ \
+            'packed_addresses', \
+            'be_uint16', \
+            'uint8']
 
 KIND = Literal[ \
             'int32', \
             'tick', \
             'string', \
             'raw', \
             'sha256', \
@@ -40,14 +45,23 @@
     disallow_cc: bool
 
 class ArrayMemberTypeJson(TypedDict):
     kind: KIND
     # strings
     disallow_cc: bool
 
+    # array in array only for de client info
+    # type forward declaration or self reference is not supported
+    # so hack it with a string
+    member_type: 'ArrayMemberTypeJson'
+    count: int
+
+class NetConnlessMemberTypeJson(TypedDict):
+    kind: KINDCONLESS
+
 class NetMessageMemberTypeJson(TypedDict):
     kind: KIND
     inner: InnerNetMessageMemberTypeJson
 
     # enums
     enum: list[str]
 
@@ -67,90 +81,69 @@
 
 class NetMessageJson(TypedDict):
     id: int
     name: list[str]
     members: list[NetMessageMemberJson]
     attributes: list[Literal['msg_encoding']]
 
+class NetConnlessJson(TypedDict):
+    id: Annotated[list[int], 8]
+    name: list[str]
+    members: list[NetMessageMemberJson]
+
 class SpecJson(TypedDict):
     constants: list[ConstantJson]
     game_enumerations: list[GameEnumJson]
     game_messages: list[NetMessageJson]
     system_messages: list[NetMessageJson]
-
-def gen_match_file7(
-        msg_type: Literal['system', 'game'],
-        messages: list[NetMessageJson]
-):
-    match_code: str = """# generated by scripts/generate_messages.py
-from typing import Optional
-
-import twnet_parser.msg7
-from twnet_parser.net_message import NetMessage
-
-"""
-
-    msg: NetMessageJson
-    for msg in messages:
-        name_snake = name_to_snake(msg['name'])
-        match_code += f"import twnet_parser.messages7.{msg_type}" \
-                f".{name_snake}" \
-                " as \\\n" \
-                f"       {msg_type}7_{name_snake}\n"
-
-    match_code += f"""
-def match_{msg_type}7(msg_id: int, data: bytes) -> NetMessage:
-    msg: Optional[NetMessage] = None
-"""
-
-    if_ = 'if'
-    for msg in messages:
-        name_snake = name_to_snake(msg['name'])
-        name_camel = name_to_camel(msg['name'])
-        match_code += \
-f"""
-    {if_} msg_id == twnet_parser.msg7.{name_snake.upper()}:
-        msg = {msg_type}7_{name_snake}.Msg{name_camel}()"""
-        if_ = 'elif'
-
-    match_code += '\n\n    if msg is None:\n'
-    match_code += '        '
-    match_code += 'raise ValueError('
-    match_code += 'f"Error: unknown ' \
-            + msg_type + \
-            ' message id={msg_id} data={data[0]}")\n'
-    match_code += '\n'
-    match_code += '    msg.unpack(data)\n'
-    match_code += '    return msg\n'
-
-    dirname = os.path.dirname(__file__)
-    file_path= os.path.join(
-            dirname,
-            f'../twnet_parser/msg_matcher/{msg_type}7.py')
-    # if os.path.exists(file_path):
-    #     print(f"Warning: file already exists! {file_path}")
-    #     return
-    with open(file_path, 'w') as out_file:
-        print(f"Generating {file_path} ...")
-        out_file.write(match_code)
+    connless_messages: list[NetConnlessJson]
+    snapshot_objects: list[NetMessageJson]
 
 def fix_name_conflict(name: str) -> str:
     # https://peps.python.org/pep-0008/#descriptive-naming-styles
-    if name == 'pass':
-        return 'pass_'
+    if name in ('pass', 'self'):
+        return f'{name}_'
     return name
 
 def name_to_camel(name_list: list[str]) -> str:
     name = ''.join([part.capitalize() for part in name_list])
     return fix_name_conflict(name)
 
 def name_to_snake(name_list: list[str]) -> str:
     name = '_'.join(name_list)
     return fix_name_conflict(name)
 
+def gen_unpack_members_connless7(msg: NetConnlessJson) -> str:
+    res: str = ''
+    for member in msg['members']:
+        unpacker = 'int()'
+        name = name_to_snake(member["name"])
+        if member['type']['kind'] == 'be_uint16':
+            unpacker = 'be_uint16()'
+        elif member['type']['kind'] == 'uint8':
+            unpacker = 'uint8()'
+        elif member['type']['kind'] == 'int32':
+            unpacker = 'int()'
+        elif member['type']['kind'] == 'int32_string':
+            res += f'        self.{name} = int(unpacker.get_str())\n'
+            continue
+        elif member['type']['kind'] == 'string':
+            if member['type']['disallow_cc']:
+                unpacker = 'str(SANITIZE_CC)'
+            else:
+                unpacker = 'str()'
+        elif member['type']['kind'] == 'serverinfo_client': # TODO: serverinfo_client
+            unpacker = 'raw()'
+        elif member['type']['kind'] == 'packed_addresses':
+            unpacker = 'packed_addresses()'
+        else:
+            raise ValueError(f"Error: unknown type {member['type']}")
+        res += f'        self.{name} = unpacker.get_{unpacker}\n'
+    return res
+
 def gen_unpack_members(msg: NetMessageJson) -> str:
     res: str = ''
     for member in msg['members']:
         # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
         unpacker = 'int()'
         if member['type']['kind'] == 'string':
             if member['type']['disallow_cc']:
@@ -198,14 +191,30 @@
                 # disadvantages see the related issue here
                 # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/7
                 unpacker = 'int()'
             elif arr_member['kind'] == 'boolean':
                 unpacker = 'int() == 1'
             elif arr_member['kind'] in ('int32', 'tick'):
                 unpacker = 'int()'
+            elif arr_member['kind'] == 'array':
+                sub_size: int = arr_member['count']
+                sub_arr_member = arr_member['member_type']
+                unpacker = 'int()'
+                if sub_arr_member['kind'] == 'int32':
+                    name = name_to_snake(member["name"])
+                    res += f'        for i in range(0, {size}):\n'
+                    res +=  '            sub: list[int] = []\n'
+                    res += f'            for k in range(0, {sub_size}):\n'
+                    res += f'                sub[k] = unpacker.get_{unpacker}\n'
+                    res += f'            self.{name}[i] = sub\n'
+                    continue
+                else:
+                    raise ValueError(
+                            f"Error: unknown sub array member type {member['type']}"
+                    )
             else:
                 raise ValueError(f"Error: unknown array member type {member['type']}")
             name = name_to_snake(member["name"])
             res += f'        for i in range(0, {size}):\n'
             res += f'            self.{name}[i] = unpacker.get_{unpacker}\n'
             continue
         elif member['type']['kind'] == 'flags': # TODO: think about flags
@@ -223,84 +232,14 @@
                 unpacker = 'int() # TODO: optionals'
         else:
             raise ValueError(f"Error: unknown type {member['type']}")
         name = name_to_snake(member["name"])
         res += f'        self.{name} = unpacker.get_{unpacker}\n'
     return res
 
-def get_dependencies(msg: NetMessageJson) -> str:
-    packer_deps: list[str] = []
-    typing_deps: list[str] = []
-    need_enums: bool = False
-    for member in msg['members']:
-        if member['type']['kind'] == 'string':
-            packer_deps.append('pack_str')
-            if member['type']['disallow_cc']:
-                packer_deps.append('SANITIZE_CC')
-        elif member['type']['kind'] == 'rest':
-            pass
-        elif member['type']['kind'] == 'sha256':
-            typing_deps.append('Annotated')
-        elif member['type']['kind'] == 'data':
-            if member['type']['size'] == 'specified_before':
-                typing_deps.append('Optional')
-            else:
-                raise ValueError(f"Error: unknown data size {member['type']}")
-        # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
-        elif member['type']['kind'] == 'enum':
-            need_enums = True
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] in ('int32', 'tick'):
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'boolean':
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'tune_param':
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'snapshot_object':
-            # TODO: think about snapshot_object
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'array':
-            packer_deps.append('pack_int')
-            typing_deps.append('Annotated')
-            arr_member: ArrayMemberTypeJson = member['type']['member_type']
-            if arr_member['kind'] == 'string':
-                packer_deps.append('pack_str')
-                if arr_member['disallow_cc']:
-                    packer_deps.append('SANITIZE_CC')
-            elif arr_member['kind'] == 'enum':
-                need_enums = True
-                packer_deps.append('pack_int')
-            elif arr_member['kind'] == 'boolean':
-                packer_deps.append('pack_int')
-            elif arr_member['kind'] in ('int32', 'tick'):
-                packer_deps.append('pack_int')
-            else:
-                raise ValueError(f"Error: unknown array member type {member['type']}")
-        elif member['type']['kind'] == 'flags': # TODO: think about flags
-            packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'optional':
-            if member['type']['inner']['kind'] == 'string':
-                packer_deps.append('pack_str')
-                if member['type']['inner']['disallow_cc']:
-                    packer_deps.append('SANITIZE_CC')
-            elif member['type']['inner']['kind'] in ('int32', 'tick'):
-                packer_deps.append('pack_int')
-        else:
-            raise ValueError(f"Error: unknown type {member['type']}")
-    res: str = ''
-    if len(packer_deps) > 0:
-        res += 'from twnet_parser.packer import ' + \
-            ', '.join(sorted(set(packer_deps))) + '\n'
-    if len(typing_deps) > 0:
-        res += 'from typing import ' + \
-            ', '.join(sorted(set(typing_deps))) + '\n'
-    if need_enums:
-        res += 'import twnet_parser.enum7 as enum7\n'
-    return res
-
 def pack_field(member: NetMessageMemberJson) -> str:
     name: str = name_to_snake(member["name"])
     field: str = f'self.{name}'
     packer = 'int'
     if member['type']['kind'] == 'string':
         packer = 'str'
     elif member['type']['kind'] in ('sha256', 'rest'):
@@ -330,14 +269,20 @@
            packer = 'str'
         elif arr_member['kind'] == 'enum':
            packer = 'int'
         elif arr_member['kind'] == 'boolean':
            packer = 'int'
         elif arr_member['kind'] in ('int32', 'tick'):
            packer = 'int'
+        elif arr_member['kind'] == 'array':
+            sub_arr_member = arr_member['member_type']
+            if sub_arr_member['kind'] == 'int32':
+                return f"b''.join([b''.join([pack_{packer}(x) for x in sub]) for sub in {field}])"
+            else:
+               raise ValueError(f"Error: unknown sub array member type {member['type']}")
         else:
            raise ValueError(f"Error: unknown array member type {member['type']}")
         return f"b''.join([pack_{packer}(x) for x in {field}])"
     elif member['type']['kind'] == 'flags': # TODO: think about flags
         packer = 'int'
     elif member['type']['kind'] == 'optional':
         packer = 'int'
@@ -358,14 +303,47 @@
     if len(members) == 1:
         return f'        return {pack_field(members[0])}'
     mem_strs: list[str] = [
             f'            {pack_field(member)}' for member in members[1:]]
     return f"        return {pack_field(members[0])} + \\\n" + \
             ' + \\\n'.join(mem_strs)
 
+def pack_field_connless7(member: NetMessageMemberJson) -> str:
+    name: str = name_to_snake(member["name"])
+    field: str = f'self.{name}'
+    packer = 'int'
+    if member['type']['kind'] == 'packed_addresses':
+        packer = 'packed_addresses'
+    elif member['type']['kind'] == 'be_uint16':
+        packer = 'be_uint16'
+    elif member['type']['kind'] == 'uint8':
+        packer = 'uint8'
+    elif member['type']['kind'] == 'string':
+        packer = 'str'
+    elif member['type']['kind'] == 'int32':
+        packer = 'int'
+    elif member['type']['kind'] == 'int32_string':
+        return f'pack_str(str({field}))'
+    elif member['type']['kind'] == 'serverinfo_client': # TODO: serverinfo_client
+        return f'self.{name}'
+    else:
+        raise ValueError(f"Error: unknown type {member['type']}")
+    return f'pack_{packer}({field})'
+
+def gen_pack_return_connless7(msg: NetConnlessJson) -> str:
+    members: list[NetMessageMemberJson] = msg['members']
+    if len(members) == 0:
+        return "        return b''"
+    if len(members) == 1:
+        return f'        return {pack_field_connless7(members[0])}'
+    mem_strs: list[str] = [
+            f'            {pack_field_connless7(member)}' for member in members[1:]]
+    return f"        return {pack_field_connless7(members[0])} + \\\n" + \
+            ' + \\\n'.join(mem_strs)
+
 def get_default(field_path: str) -> Optional[str]:
     """
     field_path has the following format:
 
         game.msg_name.field_name
 
     example:
@@ -394,17 +372,404 @@
             return f"'{default}'"
         else:
             print(f"Error: invalid default type for field {field_path}")
             print(f"        please check {def_file} for errors")
             exit(1)
 
 class CodeGenerator():
-    def __init__(self) -> None:
+    def __init__(self, protocol_version: str) -> None:
+        self.protocol_version = protocol_version
         self.game_enums: list[GameEnumJson] = []
 
+    def get_dependencies_connless(self, msg: NetConnlessJson) -> str:
+        packer_deps: list[str] = []
+        typing_deps: list[str] = ['Literal']
+        res: str = ''
+        for member in msg['members']:
+            if member['type']['kind'] == 'packed_addresses':
+                packer_deps.append('pack_packed_addresses')
+                res += 'from twnet_parser.master_server import MastersrvAddr\n'
+            elif member['type']['kind'] == 'uint8':
+                packer_deps.append('pack_uint8')
+            elif member['type']['kind'] == 'be_uint16':
+                packer_deps.append('pack_be_uint16')
+            elif member['type']['kind'] == 'int32':
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'int32_string':
+                packer_deps.append('pack_str')
+            elif member['type']['kind'] == 'serverinfo_client': # TODO: serverinfo_client
+                pass # use pack raw
+            elif member['type']['kind'] == 'string':
+                packer_deps.append('pack_str')
+                if member['type']['disallow_cc']:
+                    packer_deps.append('SANITIZE_CC')
+            else:
+                raise ValueError(f"Error: unknown type {member['type']}")
+        if len(packer_deps) > 0:
+            res += 'from twnet_parser.packer import ' + \
+                ', '.join(sorted(set(packer_deps))) + '\n'
+        if len(typing_deps) > 0:
+            res += 'from typing import ' + \
+                ', '.join(sorted(set(typing_deps))) + '\n'
+        return res
+
+    def get_dependencies(
+            self,
+            msg: NetMessageJson,
+            typing_dep: Optional[str] = 'Literal'
+    ) -> str:
+        packer_deps: list[str] = []
+        typing_deps: list[str] = []
+        if typing_dep:
+            typing_deps.append(typing_dep)
+        need_enums: bool = False
+        for member in msg['members']:
+            if member['type']['kind'] == 'string':
+                packer_deps.append('pack_str')
+                if member['type']['disallow_cc']:
+                    packer_deps.append('SANITIZE_CC')
+            elif member['type']['kind'] == 'rest':
+                pass
+            elif member['type']['kind'] == 'sha256':
+                typing_deps.append('Annotated')
+            elif member['type']['kind'] == 'data':
+                if member['type']['size'] == 'specified_before':
+                    typing_deps.append('Optional')
+                else:
+                    raise ValueError(f"Error: unknown data size {member['type']}")
+            # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
+            elif member['type']['kind'] == 'enum':
+                need_enums = True
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] in ('int32', 'tick'):
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'boolean':
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'tune_param':
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'snapshot_object':
+                # TODO: think about snapshot_object
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'array':
+                packer_deps.append('pack_int')
+                typing_deps.append('Annotated')
+                arr_member: ArrayMemberTypeJson = member['type']['member_type']
+                if arr_member['kind'] == 'string':
+                    packer_deps.append('pack_str')
+                    if arr_member['disallow_cc']:
+                        packer_deps.append('SANITIZE_CC')
+                elif arr_member['kind'] == 'enum':
+                    need_enums = True
+                    packer_deps.append('pack_int')
+                elif arr_member['kind'] == 'boolean':
+                    packer_deps.append('pack_int')
+                elif arr_member['kind'] in ('int32', 'tick'):
+                    packer_deps.append('pack_int')
+                elif arr_member['kind'] == 'array':
+                    if arr_member['member_type']['kind'] == 'int32':
+                        packer_deps.append('pack_int')
+                    else:
+                        raise ValueError(
+                                f"Error: unknown sub array member type {member['type']}"
+                        )
+                else:
+                    raise ValueError(f"Error: unknown array member type {member['type']}")
+            elif member['type']['kind'] == 'flags': # TODO: think about flags
+                packer_deps.append('pack_int')
+            elif member['type']['kind'] == 'optional':
+                if member['type']['inner']['kind'] == 'string':
+                    packer_deps.append('pack_str')
+                    if member['type']['inner']['disallow_cc']:
+                        packer_deps.append('SANITIZE_CC')
+                elif member['type']['inner']['kind'] in ('int32', 'tick'):
+                    packer_deps.append('pack_int')
+            else:
+                raise ValueError(f"Error: unknown type {member['type']}")
+        res: str = ''
+        if len(packer_deps) > 0:
+            res += 'from twnet_parser.packer import ' + \
+                ', '.join(sorted(set(packer_deps))) + '\n'
+        if len(typing_deps) > 0:
+            res += 'from typing import ' + \
+                ', '.join(sorted(set(typing_deps))) + '\n'
+        if need_enums:
+            res += f'import twnet_parser.enum{self.protocol_version} as enum{self.protocol_version}\n'
+        return res
+
+    def gen_match_file(
+            self,
+            msg_type: Literal['system', 'game'],
+            messages: list[NetMessageJson]
+    ):
+        match_code: str = f"""# generated by scripts/generate_messages.py
+from typing import Optional
+
+import twnet_parser.msg{self.protocol_version}
+from twnet_parser.net_message import NetMessage
+
+"""
+
+        msg: NetMessageJson
+        for msg in messages:
+            name_snake = name_to_snake(msg['name'])
+            match_code += f"import twnet_parser.messages{self.protocol_version}.{msg_type}" \
+                    f".{name_snake}" \
+                    " as \\\n" \
+                    f"       {msg_type}{self.protocol_version}_{name_snake}\n"
+
+        match_code += f"""
+def match_{msg_type}{self.protocol_version}(msg_id: int, data: bytes) -> NetMessage:
+    msg: Optional[NetMessage] = None
+"""
+
+        if_ = 'if'
+        for msg in messages:
+            name_snake = name_to_snake(msg['name'])
+            name_camel = name_to_camel(msg['name'])
+            match_code += f"""
+    {if_} msg_id == twnet_parser.msg{self.protocol_version}.{name_snake.upper()}:
+        msg = {msg_type}{self.protocol_version}_{name_snake}.Msg{name_camel}()"""
+            if_ = 'elif'
+
+        match_code += '\n\n    if msg is None:\n'
+        match_code += '        '
+        match_code += 'raise ValueError('
+        match_code += 'f"Error: unknown ' \
+                + msg_type + \
+                ' message id={msg_id} data={data[0]}")\n'
+        match_code += '\n'
+        match_code += '    msg.unpack(data)\n'
+        match_code += '    return msg\n'
+
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                f'../twnet_parser/msg_matcher/{msg_type}{self.protocol_version}.py')
+        # if os.path.exists(file_path):
+        #     print(f"Warning: file already exists! {file_path}")
+        #     return
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write(match_code)
+
+    def gen_match_file_connless(
+            self,
+            messages: list[NetConnlessJson]
+    ):
+        match_code: str = f"""# generated by scripts/generate_messages.py
+from typing import Optional
+
+import twnet_parser.msg{self.protocol_version}
+from twnet_parser.connless_message import ConnlessMessage
+
+"""
+
+        msg: NetConnlessJson
+        for msg in messages:
+            name_snake = name_to_snake(msg['name'])
+            match_code += f"import twnet_parser.messages{self.protocol_version}.connless" \
+                    f".{name_snake}" \
+                    " as \\\n" \
+                    f"       connless_{name_snake}\n"
+
+        match_code += f"""
+def match_connless{self.protocol_version}(msg_id: bytes, data: bytes) -> ConnlessMessage:
+    msg: Optional[ConnlessMessage] = None
+"""
+
+        if_ = 'if'
+        for msg in messages:
+            name_snake = name_to_snake(msg['name'])
+            name_camel = name_to_camel(msg['name'])
+            match_code += \
+    f"""
+    {if_} msg_id == twnet_parser.msg{self.protocol_version}.CONNLESS_{name_snake.upper()}:
+        msg = connless_{name_snake}.Msg{name_camel}()"""
+            if_ = 'elif'
+
+        match_code += '\n\n    if msg is None:\n'
+        match_code += '        '
+        match_code += 'raise ValueError(\n'
+        match_code += '            '
+        match_code += 'f"Error: unknown conless ' \
+                ' message id={msg_id!r} data={data[0]}"\n'
+        match_code += '        )\n'
+        match_code += '\n'
+        match_code += '    msg.unpack(data)\n'
+        match_code += '    return msg\n'
+
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                f'../twnet_parser/msg_matcher/connless{self.protocol_version}.py')
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write(match_code)
+
+    def gen_init_member_header_def(
+            self,
+            member: NetMessageMemberJson,
+            name_snake: str,
+            message_type: Literal['game', 'system', 'connless', 'snap']
+    ) -> list[str]:
+        """
+        get_init_member_header_def
+
+        given a member field it returns an array of strings
+        that represent the python code for the content in the
+        init method parameter list
+
+            def __init__(self, [THIS IS GENERATED]) -> None:
+
+        it might return two fields for members like data
+        that also introduce a size field
+
+        the returned assignements do not include indentation
+        """
+        args: list[str] = []
+        # {
+        #   'name': ['message'],
+        #   'type': {
+        #     'kind': 'string',
+        #     'disallow_cc': False
+        #   }
+        # }
+        ftype = 'int'
+        default = '-1'
+        if member['type']['kind'] == 'string':
+            ftype = 'str'
+            default = "'default'"
+        elif member['type']['kind'] == 'packed_addresses': # TODO: packed_addreses default value
+            ftype = 'list[MastersrvAddr]'
+            default = '[]'
+        elif member['type']['kind'] == 'serverinfo_client': # TODO: serverinfo_client
+            ftype = 'bytes'
+            default = "b''"
+        elif member['type']['kind'] == 'be_uint16':
+            ftype = 'int'
+            default = '0'
+        elif member['type']['kind'] == 'uint8':
+            ftype = 'int'
+            default = '0'
+        elif member['type']['kind'] == 'rest':
+            ftype = 'bytes'
+            default = "b'\\x00'"
+        elif member['type']['kind'] == 'sha256':
+            ftype = 'Annotated[bytes, 32]'
+            default = "bytes(32)"
+        elif member['type']['kind'] == 'data':
+            ftype = 'bytes'
+            default = "b'\\x00'"
+            if member['type']['size'] == 'specified_before':
+                args.append('data_size: Optional[int] = None')
+            else:
+                raise ValueError(f"Error: unknown data size {member['type']}")
+        # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
+        elif member['type']['kind'] == 'enum':
+            enum_name: str = name_to_camel(member['type']['enum'])
+            ftype = 'int'
+            default = self.get_default_enum(enum_name)
+            default = f"enum{self.protocol_version}.{default}.value"
+        elif member['type']['kind'] in ('int32', 'tick', 'int32_string'):
+            ftype = 'int'
+            default = '0'
+        elif member['type']['kind'] == 'boolean':
+            ftype = 'bool'
+            default = 'False'
+        elif member['type']['kind'] == 'tune_param':
+            ftype = 'float'
+            default = '0.0'
+        elif member['type']['kind'] == 'snapshot_object':
+            # TODO: think about snapshot_object
+            ftype = 'int'
+            default = '0'
+        elif member['type']['kind'] == 'array':
+            size: int = member['type']['count']
+            if size is None:
+                print("Error: size is none for the following member")
+                print(member)
+                exit(1)
+            arr_member: ArrayMemberTypeJson = member['type']['member_type']
+            if arr_member['kind'] == 'string':
+                ftype = f'Annotated[list[str], {size}]'
+                default = '[' + ', '.join(["''"] * size) + ']'
+            elif arr_member['kind'] == 'boolean':
+                ftype = f'Annotated[list[bool], {size}]'
+                default = '[' + ', '.join(["False"] * size) + ']'
+            elif arr_member['kind'] in ('int32', 'tick', 'enum'):
+                ftype = f'Annotated[list[int], {size}]'
+                default = '[' + ', '.join(["0"] * size) + ']'
+            elif arr_member['kind'] == 'array': # snap de client info has an array of int32 arrays as field
+                # should probably do some kind of recursion here
+                # but it breaks my brain
+                sub_size: int = arr_member['count']
+                if sub_size is None:
+                    print("Error: size is none for the following sub member")
+                    print(arr_member)
+                    exit(1)
+                sub_arr_member: ArrayMemberTypeJson = arr_member['member_type']
+                if sub_arr_member['kind'] == 'int32':
+                    ftype = f'Annotated[list[list[int]], ({size},{sub_size})]'
+                    inner_default = '[' + ', '.join(["0"] * sub_size) + ']'
+                    default = '[' + ',\n                 '.join([inner_default] * size) + ']'
+                else:
+                    raise ValueError( \
+                        f"Error: msg {name_to_snake(member['name'])} " \
+                        f"has unknown array sub member type {member['type']}")
+            else:
+                raise ValueError( \
+                    f"Error: msg {name_to_snake(member['name'])} " \
+                    f"has unknown array member type {member['type']}")
+            # Initializing lists with defaults
+            # And type annotation can get quite long
+            # So split it in two lines
+            default = f'\\\n                {default}'
+        elif member['type']['kind'] == 'flags': # TODO: think about flags
+            ftype = 'int'
+            default = '0'
+        elif member['type']['kind'] == 'optional':
+            if member['type']['inner']['kind'] == 'string':
+                ftype = 'str'
+                default = "''"
+            elif member['type']['inner']['kind'] in ('int32', 'tick'):
+                ftype = 'int'
+                default = '0'
+            else:
+                raise \
+                    ValueError( \
+                    f"Error: unknown optional type {member['type']}")
+        else:
+            raise ValueError(f"Error: unknown type {member['type']}")
+        name = name_to_snake(member["name"])
+        manual_default = get_default(f"{message_type}.{name_snake}.{name}")
+        if manual_default:
+            default = manual_default
+        args.append(f'{name}: {ftype} = {default}')
+        return args
+
+    def write_init_method_header_connless(
+            self,
+            out_file: TextIO,
+            msg: NetConnlessJson,
+            name_snake: str
+    ) -> None:
+        comma: str = ''
+        if len(msg['members']) > 0:
+            comma = ',\n'
+        out_file.write( \
+            '    def __init__(\n' \
+            f'            self{comma}')
+        args: list[str] = []
+        for member in msg['members']:
+            mem_defs: list[str] = self.gen_init_member_header_def(member, name_snake, 'connless')
+            for mem_def in mem_defs:
+                args.append(f'            {mem_def}')
+        out_file.write(',\n'.join(args) + '\n')
+        out_file.write('    ) -> None:\n')
+
     def write_init_method_header(
             self,
             out_file: TextIO,
             msg: NetMessageJson,
             game: Literal['system', 'game'],
             name_snake: str
     ) -> None:
@@ -413,213 +778,247 @@
             comma = ',\n'
         out_file.write( \
             '    def __init__(\n' \
             '            self,\n' \
             f'            chunk_header: ChunkHeader = ChunkHeader(){comma}')
         args: list[str] = []
         for member in msg['members']:
+            mem_defs: list[str] = self.gen_init_member_header_def(member, name_snake, game)
+            for mem_def in mem_defs:
+                args.append(f'            {mem_def}')
+        out_file.write(',\n'.join(args) + '\n')
+        out_file.write('    ) -> None:\n')
+
+    def generate_snap_obj7(self, obj: NetMessageJson) -> None:
+        name_snake = name_to_snake(obj['name'])
+        name_camel = name_to_camel(obj['name'])
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                f'../twnet_parser/snap/0{self.protocol_version}/',
+                f'{name_snake}.py')
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write('# generated by scripts/generate_messages.py\n')
+            out_file.write('\n')
+            out_file.write('from twnet_parser.pretty_print import PrettyPrint\n')
+            if len(obj['members']) > 0:
+                out_file.write('from twnet_parser.packer import Unpacker\n')
+            out_file.write(self.get_dependencies(obj, None))
+            out_file.write('\n')
+            out_file.write(f'class Obj{name_camel}(PrettyPrint):\n')
+            comma: str = ''
+            if len(obj['members']) > 0:
+                comma = ',\n'
+            out_file.write( \
+                '    def __init__(\n' \
+                f'            self{comma}')
+            args: list[str] = []
+            for member in obj['members']:
+                mem_defs: list[str] = self.gen_init_member_header_def(member, name_snake, 'snap')
+                for mem_def in mem_defs:
+                    args.append(f'            {mem_def}')
+            out_file.write(',\n'.join(args) + '\n')
+            out_file.write('    ) -> None:\n')
+            out_file.write(f"        self.item_name: str = 'connless.{name_snake}'\n")
+            out_file.write(f"        self.type_id: int = {obj['id']}\n")
+            out_file.write( "        self.id: int = 0\n")
+            out_file.write('\n')
+            self.generate_field_assignments_in_initialize(obj, out_file)
+            out_file.write('\n')
+            out_file.write('    # first byte of data\n')
+            out_file.write('    # has to be the first byte of the message payload\n')
+            out_file.write('    # NOT the chunk header and NOT the message id\n')
+            out_file.write('    def unpack(self, data: bytes) -> bool:\n')
+            if len(obj['members']) > 0:
+                out_file.write('        unpacker = Unpacker(data)\n')
+            out_file.write(gen_unpack_members(obj))
+            out_file.write('        return True\n')
+            out_file.write('\n')
+            out_file.write('    def pack(self) -> bytes:\n')
+            out_file.write(gen_pack_return(obj))
+
+    def generate_msg_connless(
+            self,
+            msg: NetConnlessJson
+    ) -> None:
+        name_snake = name_to_snake(msg['name'])
+        name_camel = name_to_camel(msg['name'])
+        dirname = os.path.dirname(__file__)
+        file_path= os.path.join(
+                dirname,
+                f'../twnet_parser/messages{self.protocol_version}/connless/',
+                f'{name_snake}.py')
+        with open(file_path, 'w') as out_file:
+            print(f"Generating {file_path} ...")
+            out_file.write('# generated by scripts/generate_messages.py\n')
+            out_file.write('\n')
+            out_file.write('from twnet_parser.pretty_print import PrettyPrint\n')
+            if len(msg['members']) > 0:
+                out_file.write('from twnet_parser.packer import Unpacker\n')
+            out_file.write(self.get_dependencies_connless(msg))
+            out_file.write('\n')
+            out_file.write(f'class Msg{name_camel}(PrettyPrint):\n')
+            self.write_init_method_header_connless(out_file, msg, name_snake)
+            out_file.write(f"        self.message_type: Literal['connless'] = 'connless'\n")
+            out_file.write(f"        self.message_name: str = 'connless.{name_snake}'\n")
+            out_file.write(f"        self.message_id: list[int] = {msg['id']}\n")
+            out_file.write('\n')
+            for member in msg['members']:
+                ftype = 'int'
+                if member['type']['kind'] == 'packed_addresses': # TODO: packed_addreses default value
+                    ftype = 'list[MastersrvAddr]'
+                elif member['type']['kind'] == 'be_uint16': # TODO: be_uint16
+                    ftype = 'int'
+                elif member['type']['kind'] == 'uint8': # TODO: uint8
+                    ftype = 'int'
+                elif member['type']['kind'] in ('int32', 'int32_string'):
+                    ftype = 'int'
+                elif member['type']['kind'] == 'string':
+                    ftype = 'str'
+                elif member['type']['kind'] == 'serverinfo_client': # TODO: serverinfo_client
+                    ftype = 'bytes'
+                else:
+                    raise ValueError(f"Error: unknown connless type {member['type']}")
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
+            out_file.write(gen_unpack_members_connless7(msg))
+            out_file.write('        return True\n')
+            out_file.write('\n')
+            out_file.write('    def pack(self) -> bytes:\n')
+            out_file.write(gen_pack_return_connless7(msg))
+
+    def generate_field_assignments_in_initialize(
+            self,
+            msg: NetMessageJson,
+            out_file
+    ) -> None:
+        for member in msg['members']:
             # {
             #   'name': ['message'],
             #   'type': {
             #     'kind': 'string',
             #     'disallow_cc': False
             #   }
             # }
             ftype = 'int'
-            default = '-1'
             if member['type']['kind'] == 'string':
                 ftype = 'str'
-                default = "'default'"
             elif member['type']['kind'] == 'rest':
                 ftype = 'bytes'
-                default = "b'\\x00'"
             elif member['type']['kind'] == 'sha256':
                 ftype = 'Annotated[bytes, 32]'
-                default = "bytes(32)"
             elif member['type']['kind'] == 'data':
                 ftype = 'bytes'
-                default = "b'\\x00'"
                 if member['type']['size'] == 'specified_before':
-                    args.append('            data_size: Optional[int] = None')
+                    out_file.write("        " \
+                        "self.data_size: int =" \
+                        " data_size if data_size else len(data)\n")
                 else:
                     raise ValueError(f"Error: unknown data size {member['type']}")
             # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
             elif member['type']['kind'] == 'enum':
-                enum_name: str = name_to_camel(member['type']['enum'])
                 ftype = 'int'
-                default = self.get_default_enum7(enum_name)
-                default = f"enum7.{default}.value"
             elif member['type']['kind'] in ('int32', 'tick'):
                 ftype = 'int'
-                default = '0'
             elif member['type']['kind'] == 'boolean':
                 ftype = 'bool'
-                default = 'False'
             elif member['type']['kind'] == 'tune_param':
                 ftype = 'float'
-                default = '0.0'
             elif member['type']['kind'] == 'snapshot_object':
                 # TODO: think about snapshot_object
                 ftype = 'int'
-                default = '0'
             elif member['type']['kind'] == 'array':
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
+                # Array type annotations are so annoyingly long
+                # also there is a planned refactor
+                # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/4
+                # so inherit type from constructor arguments
+                ftype = ''
             elif member['type']['kind'] == 'flags': # TODO: think about flags
                 ftype = 'int'
-                default = '0'
             elif member['type']['kind'] == 'optional':
                 if member['type']['inner']['kind'] == 'string':
                     ftype = 'str'
-                    default = "''"
                 elif member['type']['inner']['kind'] in ('int32', 'tick'):
                     ftype = 'int'
-                    default = '0'
                 else:
                     raise \
                         ValueError( \
                         f"Error: unknown optional type {member['type']}")
             else:
                 raise ValueError(f"Error: unknown type {member['type']}")
             name = name_to_snake(member["name"])
-            manual_default = get_default(f"{game}.{name_snake}.{name}")
-            if manual_default:
-                default = manual_default
-            args.append(f'            {name}: {ftype} = {default}')
-        out_file.write(',\n'.join(args) + '\n')
-        out_file.write('    ) -> None:\n')
+            if ftype != '':
+                ftype = f': {ftype}'
+            if member['type']['kind'] == 'enum':
+                out_file.write(f"        self.{name}{ftype} = {name}\n")
+            else:
+                out_file.write(f"        self.{name}{ftype} = {name}\n")
 
     def generate_msg(
             self,
             msg: NetMessageJson,
-            game: Literal['game', 'system']
+            game: Literal['system', 'game']
     ) -> None:
         name_snake = name_to_snake(msg['name'])
         name_camel = name_to_camel(msg['name'])
         dirname = os.path.dirname(__file__)
         file_path= os.path.join(
                 dirname,
-                f'../twnet_parser/messages7/{game}/',
+                f'../twnet_parser/messages{self.protocol_version}/{game}/',
                 f'{name_snake}.py')
         # if os.path.exists(file_path):
         #     print(f"Warning: file already exists! {file_path}")
         #     return
         with open(file_path, 'w') as out_file:
             print(f"Generating {file_path} ...")
             out_file.write('# generated by scripts/generate_messages.py\n')
             out_file.write('\n')
             out_file.write('from twnet_parser.pretty_print import PrettyPrint\n')
             if len(msg['members']) > 0:
                 out_file.write('from twnet_parser.packer import Unpacker\n')
             out_file.write('from twnet_parser.chunk_header import ChunkHeader\n')
-            out_file.write(get_dependencies(msg))
+            out_file.write(self.get_dependencies(msg))
             out_file.write('\n')
             out_file.write(f'class Msg{name_camel}(PrettyPrint):\n')
             self.write_init_method_header(out_file, msg, game, name_snake)
+            out_file.write(f"        self.message_type: Literal['system', 'game'] = '{game}'\n")
             out_file.write(f"        self.message_name: str = '{name_snake}'\n")
             sys: str = 'True' if game == 'system' else 'False'
             out_file.write(f"        self.system_message: bool = {sys}\n")
             out_file.write(f"        self.message_id: int = {msg['id']}\n")
             out_file.write("        self.header: ChunkHeader = chunk_header\n")
             out_file.write('\n')
-            for member in msg['members']:
-                # {
-                #   'name': ['message'],
-                #   'type': {
-                #     'kind': 'string',
-                #     'disallow_cc': False
-                #   }
-                # } 
-                ftype = 'int'
-                if member['type']['kind'] == 'string':
-                    ftype = 'str'
-                elif member['type']['kind'] == 'rest':
-                    ftype = 'bytes'
-                elif member['type']['kind'] == 'sha256':
-                    ftype = 'Annotated[bytes, 32]'
-                elif member['type']['kind'] == 'data':
-                    ftype = 'bytes'
-                    if member['type']['size'] == 'specified_before':
-                        out_file.write("        " \
-                            "self.data_size: int =" \
-                            " data_size if data_size else len(data)\n")
-                    else:
-                        raise ValueError(f"Error: unknown data size {member['type']}")
-                # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
-                elif member['type']['kind'] == 'enum':
-                    ftype = 'int'
-                elif member['type']['kind'] in ('int32', 'tick'):
-                    ftype = 'int'
-                elif member['type']['kind'] == 'boolean':
-                    ftype = 'bool'
-                elif member['type']['kind'] == 'tune_param':
-                    ftype = 'float'
-                elif member['type']['kind'] == 'snapshot_object':
-                    # TODO: think about snapshot_object
-                    ftype = 'int'
-                elif member['type']['kind'] == 'array':
-                    # Array type annotations are so annoyingly long
-                    # also there is a planned refactor
-                    # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/4
-                    # so inherit type from constructor arguments
-                    ftype = ''
-                elif member['type']['kind'] == 'flags': # TODO: think about flags
-                    ftype = 'int'
-                elif member['type']['kind'] == 'optional':
-                    if member['type']['inner']['kind'] == 'string':
-                        ftype = 'str'
-                    elif member['type']['inner']['kind'] in ('int32', 'tick'):
-                        ftype = 'int'
-                    else:
-                        raise \
-                            ValueError( \
-                            f"Error: unknown optional type {member['type']}")
-                else:
-                    raise ValueError(f"Error: unknown type {member['type']}")
-                name = name_to_snake(member["name"])
-                if ftype != '':
-                    ftype = f': {ftype}'
-                if member['type']['kind'] == 'enum':
-                    out_file.write(f"        self.{name}{ftype} = {name}\n")
-                else:
-                    out_file.write(f"        self.{name}{ftype} = {name}\n")
+            self.generate_field_assignments_in_initialize(msg, out_file)
             out_file.write('\n')
             out_file.write('    # first byte of data\n')
             out_file.write('    # has to be the first byte of the message payload\n')
             out_file.write('    # NOT the chunk header and NOT the message id\n')
             out_file.write('    def unpack(self, data: bytes) -> bool:\n')
             if len(msg['members']) > 0:
                 out_file.write('        unpacker = Unpacker(data)\n')
             out_file.write(gen_unpack_members(msg))
             out_file.write('        return True\n')
             out_file.write('\n')
             out_file.write('    def pack(self) -> bytes:\n')
             out_file.write(gen_pack_return(msg))
 
-    def get_default_enum7(self, enum_name: str) -> str:
+    def get_default_enum(self, enum_name: str) -> str:
         """
         enum_name has to be camel case
 
         If for example enum_name 'chat' is given
         it returns 'CHAT_NONE'
         """
         enum: GameEnumJson
@@ -629,15 +1028,15 @@
                 continue
             val: GameEnumValueJson
             for val in enum['values']:
                 sub: str = name_to_snake(val['name']).upper()
                 return f"{base}.{sub}"
         raise ValueError(f"Enum not found '{enum_name}'")
 
-    def gen_enum_file7(self) -> None:
+    def gen_enum_file(self) -> None:
         enum_code: str = 'from enum import Enum\n\n'
         enum: GameEnumJson
         for enum in self.game_enums:
             base: str = name_to_camel(enum['name'])
             enum_code += f'class {base}(Enum):\n'
             val: GameEnumValueJson
             for val in enum['values']:
@@ -648,15 +1047,15 @@
             enum_code += "\n"
         # cut off last doubled newline
         # because we do not split a section anymore
         enum_code = enum_code[:-1]
         dirname = os.path.dirname(__file__)
         file_path= os.path.join(
                 dirname,
-                '../twnet_parser/enum7.py')
+                f'../twnet_parser/enum{self.protocol_version}.py')
         # if os.path.exists(file_path):
         #     print(f"Warning: file already exists! {file_path}")
         #     return
         with open(file_path, 'w') as out_file:
             print(f"Generating {file_path} ...")
             out_file.write(enum_code)
 
@@ -664,32 +1063,62 @@
         print(f"generating classes from {spec} ...")
         with open(spec) as spec_io:
             spec_data: SpecJson = json.load(spec_io)
             # for msg in [spec_data['game_messages'][1]]:
             self.game_enums = spec_data['game_enumerations']
             game_messages: list[NetMessageJson] = spec_data['game_messages']
             system_messages: list[NetMessageJson] = spec_data['system_messages']
-            self.gen_enum_file7()
-            gen_match_file7('game', game_messages)
-            gen_match_file7('system', system_messages)
+            connless_messages: list[NetConnlessJson] = spec_data['connless_messages']
+            snapshot_objects: list[NetMessageJson] = spec_data['snapshot_objects']
+            self.gen_enum_file()
+            self.gen_match_file('game', game_messages)
+            self.gen_match_file('system', system_messages)
+            self.gen_match_file_connless(connless_messages)
             for msg in game_messages:
                 self.generate_msg(msg, 'game')
             for msg in system_messages:
+                if msg['name'] == ['snap']:
+                    continue
                 self.generate_msg(msg, 'system')
+            for connless_msg in connless_messages:
+                self.generate_msg_connless(connless_msg)
+            # for obj in snapshot_objects:
+            #     self.generate_snap_obj7(obj)
+
+class SpecInfo:
+    def __init__(
+            self,
+            json_path: str,
+            version_name: str
+    ) -> None:
+        self.json_path = json_path
+        self.version_name = version_name
 
 def main() -> None:
     dirname = os.path.dirname(__file__)
-    spec_07 = os.path.join(
-            dirname,
-            '../../libtw2/gamenet/generate/spec/teeworlds-0.7.5.json')
-    if os.path.exists(spec_07):
-        generator = CodeGenerator()
-        generator.generate(spec_07)
-    else:
-        print(f"Error: file not found {spec_07}")
-        print("        try running these commands")
-        print("")
-        print("        git clone git@github.com:heinrich5991/libtw2 ..")
+    spec_infos: list[SpecInfo] = [
+            SpecInfo(
+                '../../libtw2/gamenet/generate/spec/teeworlds-0.7.5.json',
+                '7'
+            ),
+    ]
+    #         SpecInfo(
+    #             '../../libtw2/gamenet/generate/spec/teeworlds-0.6.json',
+    #             '6'
+    #         )
+    # ]
+    for spec_info in spec_infos:
+        spec_file = os.path.join(
+                dirname,
+                spec_info.json_path)
+        if os.path.exists(spec_file):
+            generator = CodeGenerator(spec_info.version_name)
+            generator.generate(spec_file)
+        else:
+            print(f"Error: file not found {spec_file}")
+            print("        try running these commands")
+            print("")
+            print("        git clone git@github.com:heinrich5991/libtw2 ..")
 
 if __name__ == '__main__':
     main()
```

### Comparing `twnet_parser-0.6.0/setup.cfg` & `twnet_parser-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twnet_parser
-version = 0.6.0
+version = 0.7.0
 author = ChillerDragon
 author_email = chillerdragon@gmail.com
 description = A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/teeworlds-network/twnet_parser
 license = BSD-2.0
```

### Comparing `twnet_parser-0.6.0/tests/control_packets7_test.py` & `twnet_parser-0.7.0/tests/control_packets7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/ctrl_packets_test.py` & `twnet_parser-0.7.0/tests/ctrl_packets_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/int_packer_test.py` & `twnet_parser-0.7.0/tests/int_packer_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/msg7/sv_tune_params_test.py` & `twnet_parser-0.7.0/tests/msg7/sv_tune_params_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/packet_header6_test.py` & `twnet_parser-0.7.0/tests/packet_header6_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/packet_header7_test.py` & `twnet_parser-0.7.0/tests/packet_header7_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,62 +181,62 @@
     header.ack = 1023
     header.token = b'\xff\xff\xff\xff'
     header.num_chunks = 255
 
     header.flags.control = True
     header.flags.resend = True
     header.flags.compression = True
-    header.flags.connless = True
+    header.flags.connless = False
 
     # Note that even if we set everything
     # we still end up with two leading zeros
     # because those bits are unused
     # and we init the flags with 0
     assert header.pack() == bytes([ \
-            0b00111111, \
+            0b00011111, \
             0b11111111, \
             0b11111111, \
             0b11111111, \
             0b11111111, \
             0b11111111, \
             0b11111111
     ])
 
     parser = PacketHeaderParser7()
-    header = parser.parse_header(b'\xff\xff\xff\xff\xff\xff\xff')
+    header = parser.parse_header(b'\x1f\xff\xff\xff\xff\xff\xff')
 
     assert header.ack == 1023
     assert header.token == b'\xff\xff\xff\xff'
     assert header.num_chunks == 255
 
     assert header.flags.control is True
     assert header.flags.resend is True
     assert header.flags.compression is True
-    assert header.flags.connless is True
+    assert header.flags.connless is False
 
     # Note that is doesn matter wether we parse
     #
-    # b'\xff\xff\xff\xff\xff\xff\xff'
+    # b'\x1f\xff\xff\xff\xff\xff\xff'
     #
     #    or
     #
-    # b'\x3f\xff\xff\xff\xff\xff\xff'
+    # b'\xdf\xff\xff\xff\xff\xff\xff'
     #
     # because the first two bytes are ignored anyways
     parser = PacketHeaderParser7()
-    header = parser.parse_header(b'\x3f\xff\xff\xff\xff\xff\xff')
+    header = parser.parse_header(b'\xdf\xff\xff\xff\xff\xff\xff')
 
     assert header.ack == 1023
     assert header.token == b'\xff\xff\xff\xff'
     assert header.num_chunks == 255
 
     assert header.flags.control is True
     assert header.flags.resend is True
     assert header.flags.compression is True
-    assert header.flags.connless is True
+    assert header.flags.connless is False
 
 def test_packet_header_repack_none_set() -> None:
     header: PacketHeader = PacketHeader()
 
     header.ack = 0
     header.token = b'\x00\x00\x00\x00'
     header.num_chunks = 0
```

### Comparing `twnet_parser-0.6.0/tests/packet_invalid_test.py` & `twnet_parser-0.7.0/tests/packet_invalid_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/packet_with_chunks7_test.py` & `twnet_parser-0.7.0/tests/packet_with_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/repack_chunks7_test.py` & `twnet_parser-0.7.0/tests/repack_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/tests/unpacker_state_test.py` & `twnet_parser-0.7.0/tests/unpacker_state_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,53 @@
-from twnet_parser.packer import Unpacker, pack_int, pack_str
+from twnet_parser.packer import \
+        Unpacker, pack_int, pack_str, pack_uint8, pack_be_uint16
 from twnet_parser.packer import \
         NO_SANITIZE, SANITIZE, SANITIZE_CC, SKIP_START_WHITESPACES
 
+def test_pack_uint8():
+    assert pack_uint8(1) == b'\x01'
+    assert pack_uint8(2) == b'\x02'
+    assert pack_uint8(3) == b'\x03'
+
+def test_pack_be_uint16():
+    assert pack_be_uint16(1) == b'\x00\x01'
+    assert pack_be_uint16(2) == b'\x00\x02'
+    assert pack_be_uint16(3) == b'\x00\x03'
+    assert pack_be_uint16(256) == b'\x01\x00'
+
+def test_unpack_uint8():
+    u = Unpacker(b'\x01')
+    assert u.get_uint8() == 1
+    u = Unpacker(b'\x02')
+    assert u.get_uint8() == 2
+
+def test_unpack_multiple_uint8():
+    u = Unpacker(b'\x01\x02')
+    assert u.get_uint8() == 1
+    assert u.get_uint8() == 2
+
+def test_unpack_be_uint16():
+    u = Unpacker(b'\x00\x01')
+    assert u.get_be_uint16() == 1
+    u = Unpacker(b'\x00\x02')
+    assert u.get_be_uint16() == 2
+    u = Unpacker(b'\x00\x33')
+    assert u.get_be_uint16() == 51
+    u = Unpacker(b'\x01\x00')
+    assert u.get_be_uint16() == 256
+    # this is needed for the connless lis2
+    # packed_addresses field
+    u = Unpacker(b'\x20\x6F')
+    assert u.get_be_uint16() == 8303
+
+def test_unpack_multiple_be_uint16():
+    u = Unpacker(b'\x00\x01\x00\x02')
+    assert u.get_be_uint16() == 1
+    assert u.get_be_uint16() == 2
+
 def test_unpack_ints_and_strings() -> None:
     u = Unpacker(b'\x01\x02\x03\x01foo\x00bar\x00')
     assert u.get_int() == 1
     assert u.get_int() == 2
     assert u.get_int() == 3
     assert u.get_int() == 1
     assert u.get_str() == 'foo'
```

### Comparing `twnet_parser-0.6.0/twnet_parser/chunk_header.py` & `twnet_parser-0.7.0/twnet_parser/chunk_header.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/enum7.py` & `twnet_parser-0.7.0/twnet_parser/enum7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/external/huffman.py` & `twnet_parser-0.7.0/twnet_parser/external/huffman.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/message_parser.py` & `twnet_parser-0.7.0/twnet_parser/message_parser.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/control/close.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_checkpoint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from typing import Optional
+# generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
-from twnet_parser.packer import pack_str
+from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import pack_int
+from typing import Literal
 
-class CtrlClose(PrettyPrint):
+class MsgSvCheckpoint(PrettyPrint):
     def __init__(
             self,
-            reason: Optional[str] = None
+            chunk_header: ChunkHeader = ChunkHeader(),
+            diff: int = 0
     ) -> None:
-        self.message_name: str = 'close'
-        self.message_id: int = 4
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_checkpoint'
+        self.system_message: bool = False
+        self.message_id: int = 36
+        self.header: ChunkHeader = chunk_header
 
-        self.reason: Optional[str] = reason
+        self.diff: int = diff
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
-    def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
+    def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.reason = unpacker.get_str() # TODO: this is an optional field
+        self.diff = unpacker.get_int()
         return True
 
-    def pack(self, we_are_a_client: bool = True) -> bytes:
-        if self.reason:
-            return pack_str(self.reason)
-        return b''
+    def pack(self) -> bytes:
+        return pack_int(self.diff)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/control/connect.py` & `twnet_parser-0.7.0/twnet_parser/messages7/control/connect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Literal
 from twnet_parser.pretty_print import PrettyPrint
 
 class CtrlConnect(PrettyPrint):
     def __init__(
             self,
             response_token: bytes = b'\xff\xff\xff\xff'
     ) -> None:
+        self.message_type: Literal['control'] = 'control'
         self.message_name: str = 'connect'
         self.message_id: int = 1
 
         self.response_token: bytes = response_token
 
     def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         # anti reflection attack
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/control/token.py` & `twnet_parser-0.7.0/twnet_parser/messages7/control/token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Literal
 from twnet_parser.pretty_print import PrettyPrint
 
 class CtrlToken(PrettyPrint):
     def __init__(
             self,
             response_token: bytes = b'\xff\xff\xff\xff'
     ) -> None:
+        self.message_type: Literal['control'] = 'control'
         self.message_name: str = 'token'
         self.message_id: int = 5
 
         self.response_token: bytes = response_token
 
     def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         if not we_are_a_client:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_call_vote.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_call_vote.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 
 class MsgClCallVote(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             type: str = 'default',
             value: str = 'default',
             reason: str = 'default',
             force: bool = False
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_call_vote'
         self.system_message: bool = False
         self.message_id: int = 32
         self.header: ChunkHeader = chunk_header
 
         self.type: str = type
         self.value: str = value
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_command.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_str
+from typing import Literal
 
 class MsgClCommand(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             arguments: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_command'
         self.system_message: bool = False
         self.message_id: int = 39
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.arguments: str = arguments
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_emoticon.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_rem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
-import twnet_parser.enum7 as enum7
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgClEmoticon(PrettyPrint):
+class MsgMaplistEntryRem(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            emoticon: int = enum7.Emoticon.OOP.value
+            name: str = 'default'
     ) -> None:
-        self.message_name: str = 'cl_emoticon'
-        self.system_message: bool = False
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'maplist_entry_rem'
+        self.system_message: bool = True
         self.message_id: int = 30
         self.header: ChunkHeader = chunk_header
 
-        self.emoticon: int = emoticon
+        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.emoticon = unpacker.get_int() # enum EMOTICON
+        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.emoticon)
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_kill.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_off.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgClKill(PrettyPrint):
+class MsgRconAuthOff(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'cl_kill'
-        self.system_message: bool = False
-        self.message_id: int = 28
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_auth_off'
+        self.system_message: bool = True
+        self.message_id: int = 12
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_ready_change.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_ready_change.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
 class MsgClReadyChange(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_ready_change'
         self.system_message: bool = False
         self.message_id: int = 29
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_say.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_say.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgClSay(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             mode: int = enum7.Chat.NONE.value,
             target: int = 0,
             message: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_say'
         self.system_message: bool = False
         self.message_id: int = 24
         self.header: ChunkHeader = chunk_header
 
         self.mode: int = mode
         self.target: int = target
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_set_spectator_mode.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_spectator_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgClSetSpectatorMode(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             spec_mode: int = enum7.Spec.FREEVIEW.value,
             spectator_id: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_set_spectator_mode'
         self.system_message: bool = False
         self.message_id: int = 26
         self.header: ChunkHeader = chunk_header
 
         self.spec_mode: int = spec_mode
         self.spectator_id: int = spectator_id
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_set_team.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_team.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgClSetTeam(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             team: int = enum7.Team.SPECTATORS.value
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_set_team'
         self.system_message: bool = False
         self.message_id: int = 25
         self.header: ChunkHeader = chunk_header
 
         self.team: int = team
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_skin_change.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_skin_change.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
-from typing import Annotated
+from typing import Annotated, Literal
 
 class MsgClSkinChange(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_skin_change'
         self.system_message: bool = False
         self.message_id: int = 34
         self.header: ChunkHeader = chunk_header
 
         self.skin_part_names = skin_part_names
         self.use_custom_colors = use_custom_colors
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_start_info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_start_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
-from typing import Annotated
+from typing import Annotated, Literal
 
 class MsgClStartInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             clan: str = 'default',
@@ -16,14 +16,15 @@
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'cl_start_info'
         self.system_message: bool = False
         self.message_id: int = 27
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.clan: str = clan
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/cl_vote.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_extra_projectile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
-class MsgClVote(PrettyPrint):
+class MsgSvExtraProjectile(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            vote: int = 0
+            projectile: int = 0
     ) -> None:
-        self.message_name: str = 'cl_vote'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_extra_projectile'
         self.system_message: bool = False
-        self.message_id: int = 31
+        self.message_id: int = 7
         self.header: ChunkHeader = chunk_header
 
-        self.vote: int = vote
+        self.projectile: int = projectile
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.vote = unpacker.get_int()
+        self.projectile = unpacker.get_int() # TODO: this is a snapshot object
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.vote)
+        return pack_int(self.projectile)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/de_client_enter.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_enter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgDeClientEnter(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             client_id: int = 0,
             team: int = enum7.Team.SPECTATORS.value
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'de_client_enter'
         self.system_message: bool = False
         self.message_id: int = 22
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.client_id: int = client_id
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/de_client_leave.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_leave.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 
 class MsgDeClientLeave(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             client_id: int = 0,
             reason: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'de_client_leave'
         self.system_message: bool = False
         self.message_id: int = 23
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.client_id: int = client_id
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_broadcast.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_broadcast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
+from typing import Literal
 
 class MsgSvBroadcast(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             message: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_broadcast'
         self.system_message: bool = False
         self.message_id: int = 2
         self.header: ChunkHeader = chunk_header
 
         self.message: str = message
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_chat.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgSvChat(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             mode: int = enum7.Chat.NONE.value,
             client_id: int = 0,
             target_id: int = 0,
             message: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_chat'
         self.system_message: bool = False
         self.message_id: int = 3
         self.header: ChunkHeader = chunk_header
 
         self.mode: int = mode
         self.client_id: int = client_id
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_checkpoint.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_line.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgSvCheckpoint(PrettyPrint):
+class MsgRconLine(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            diff: int = 0
+            line: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_checkpoint'
-        self.system_message: bool = False
-        self.message_id: int = 36
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_line'
+        self.system_message: bool = True
+        self.message_id: int = 13
         self.header: ChunkHeader = chunk_header
 
-        self.diff: int = diff
+        self.line: str = line
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.diff = unpacker.get_int()
+        self.line = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.diff)
+        return pack_str(self.line)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_client_drop.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_team.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from twnet_parser.packer import pack_int
+from typing import Literal
+import twnet_parser.enum7 as enum7
 
-class MsgSvClientDrop(PrettyPrint):
+class MsgSvTeam(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            reason: str = 'default',
-            silent: bool = False
+            team: int = enum7.Team.SPECTATORS.value,
+            silent: bool = False,
+            cooldown_tick: int = 0
     ) -> None:
-        self.message_name: str = 'sv_client_drop'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_team'
         self.system_message: bool = False
-        self.message_id: int = 20
+        self.message_id: int = 4
         self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
-        self.reason: str = reason
+        self.team: int = team
         self.silent: bool = silent
+        self.cooldown_tick: int = cooldown_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.reason = unpacker.get_str(SANITIZE_CC)
+        self.team = unpacker.get_int() # enum TEAM
         self.silent = unpacker.get_int() == 1
+        self.cooldown_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
-            pack_str(self.reason) + \
-            pack_int(self.silent)
+            pack_int(self.team) + \
+            pack_int(self.silent) + \
+            pack_int(self.cooldown_tick)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_client_info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
-from typing import Annotated
+from typing import Annotated, Literal
 import twnet_parser.enum7 as enum7
 
 class MsgSvClientInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
@@ -21,14 +21,15 @@
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0],
             silent: bool = False
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_client_info'
         self.system_message: bool = False
         self.message_id: int = 18
         self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.local: bool = local
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_command_info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgSvCommandInfo(PrettyPrint):
+class MsgRconCmdAdd(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
-            args_format: str = 'default',
-            help_text: str = 'default'
+            help: str = 'default',
+            params: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_command_info'
-        self.system_message: bool = False
-        self.message_id: int = 37
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_cmd_add'
+        self.system_message: bool = True
+        self.message_id: int = 14
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
-        self.args_format: str = args_format
-        self.help_text: str = help_text
+        self.help: str = help
+        self.params: str = params
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str(SANITIZE_CC)
-        self.args_format = unpacker.get_str(SANITIZE_CC)
-        self.help_text = unpacker.get_str(SANITIZE_CC)
+        self.name = unpacker.get_str()
+        self.help = unpacker.get_str()
+        self.params = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
-            pack_str(self.args_format) + \
-            pack_str(self.help_text)
+            pack_str(self.help) + \
+            pack_str(self.params)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_command_info_remove.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_rem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgSvCommandInfoRemove(PrettyPrint):
+class MsgRconCmdRem(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_command_info_remove'
-        self.system_message: bool = False
-        self.message_id: int = 38
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_cmd_rem'
+        self.system_message: bool = True
+        self.message_id: int = 15
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str(SANITIZE_CC)
+        self.name = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_emoticon.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_emoticon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgSvEmoticon(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
             emoticon: int = enum7.Emoticon.OOP.value
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_emoticon'
         self.system_message: bool = False
         self.message_id: int = 10
         self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.emoticon: int = emoticon
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_extra_projectile.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgSvExtraProjectile(PrettyPrint):
+class MsgRconAuth(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            projectile: int = 0
+            password: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_extra_projectile'
-        self.system_message: bool = False
-        self.message_id: int = 7
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_auth'
+        self.system_message: bool = True
+        self.message_id: int = 22
         self.header: ChunkHeader = chunk_header
 
-        self.projectile: int = projectile
+        self.password: str = password
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.projectile = unpacker.get_int() # TODO: this is a snapshot object
+        self.password = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.projectile)
+        return pack_str(self.password)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_game_info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgSvGameInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             game_flags: int = 0,
             score_limit: int = 0,
             time_limit: int = 0,
             match_num: int = 0,
             match_current: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_game_info'
         self.system_message: bool = False
         self.message_id: int = 19
         self.header: ChunkHeader = chunk_header
 
         self.game_flags: int = game_flags
         self.score_limit: int = score_limit
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_game_msg.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_kill.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgSvGameMsg(PrettyPrint):
+class MsgClKill(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'sv_game_msg'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'cl_kill'
         self.system_message: bool = False
-        self.message_id: int = 21
+        self.message_id: int = 28
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_kill_msg.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_kill_msg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgSvKillMsg(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             killer: int = 0,
             victim: int = 0,
             weapon: int = 0,
             mode_special: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_kill_msg'
         self.system_message: bool = False
         self.message_id: int = 5
         self.header: ChunkHeader = chunk_header
 
         self.killer: int = killer
         self.victim: int = victim
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_motd.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info_remove.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
+from typing import Literal
 
-class MsgSvMotd(PrettyPrint):
+class MsgSvCommandInfoRemove(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            message: str = 'default'
+            name: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_motd'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_command_info_remove'
         self.system_message: bool = False
-        self.message_id: int = 1
+        self.message_id: int = 38
         self.header: ChunkHeader = chunk_header
 
-        self.message: str = message
+        self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.message = unpacker.get_str()
+        self.name = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.message)
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_race_finish.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
+import twnet_parser.enum7 as enum7
 
-class MsgSvRaceFinish(PrettyPrint):
+class MsgSvVoteSet(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
-            time: int = 0,
-            diff: int = 0,
-            record_personal: bool = False,
-            record_server: bool = False
+            type: int = enum7.Vote.UNKNOWN.value,
+            timeout: int = 0,
+            description: str = 'default',
+            reason: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_race_finish'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_vote_set'
         self.system_message: bool = False
-        self.message_id: int = 35
+        self.message_id: int = 15
         self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
-        self.time: int = time
-        self.diff: int = diff
-        self.record_personal: bool = record_personal
-        self.record_server: bool = record_server
+        self.type: int = type
+        self.timeout: int = timeout
+        self.description: str = description
+        self.reason: str = reason
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.time = unpacker.get_int()
-        self.diff = unpacker.get_int()
-        self.record_personal = unpacker.get_int() == 1
-        self.record_server = unpacker.get_int() == 1
+        self.type = unpacker.get_int() # enum VOTE
+        self.timeout = unpacker.get_int()
+        self.description = unpacker.get_str(SANITIZE_CC)
+        self.reason = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
-            pack_int(self.time) + \
-            pack_int(self.diff) + \
-            pack_int(self.record_personal) + \
-            pack_int(self.record_server)
+            pack_int(self.type) + \
+            pack_int(self.timeout) + \
+            pack_str(self.description) + \
+            pack_str(self.reason)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_ready_to_enter.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/ready.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgSvReadyToEnter(PrettyPrint):
+class MsgReady(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'sv_ready_to_enter'
-        self.system_message: bool = False
-        self.message_id: int = 8
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'ready'
+        self.system_message: bool = True
+        self.message_id: int = 18
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_server_settings.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_server_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgSvServerSettings(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             kick_vote: bool = False,
             kick_min: int = 0,
             spec_vote: bool = False,
             team_lock: bool = False,
             team_balance: bool = False,
             player_slots: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_server_settings'
         self.system_message: bool = False
         self.message_id: int = 17
         self.header: ChunkHeader = chunk_header
 
         self.kick_vote: bool = kick_vote
         self.kick_min: int = kick_min
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_skin_change.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_skin_change.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
-from typing import Annotated
+from typing import Annotated, Literal
 
 class MsgSvSkinChange(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             client_id: int = 0,
             skin_part_names: Annotated[list[str], 6] = \
                 ['', '', '', '', '', ''],
             use_custom_colors: Annotated[list[bool], 6] = \
                 [False, False, False, False, False, False],
             skin_part_colors: Annotated[list[int], 6] = \
                 [0, 0, 0, 0, 0, 0]
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_skin_change'
         self.system_message: bool = False
         self.message_id: int = 33
         self.header: ChunkHeader = chunk_header
 
         self.client_id: int = client_id
         self.skin_part_names = skin_part_names
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_team.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
-import twnet_parser.enum7 as enum7
+from twnet_parser.packer import pack_int, pack_str
+from typing import Literal
 
-class MsgSvTeam(PrettyPrint):
+class MsgInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            client_id: int = 0,
-            team: int = enum7.Team.SPECTATORS.value,
-            silent: bool = False,
-            cooldown_tick: int = 0
+            version: str = '0.7 802f1be60a05665f',
+            password: str = '',
+            client_version: int = 1797
     ) -> None:
-        self.message_name: str = 'sv_team'
-        self.system_message: bool = False
-        self.message_id: int = 4
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'info'
+        self.system_message: bool = True
+        self.message_id: int = 1
         self.header: ChunkHeader = chunk_header
 
-        self.client_id: int = client_id
-        self.team: int = team
-        self.silent: bool = silent
-        self.cooldown_tick: int = cooldown_tick
+        self.version: str = version
+        self.password: str = password
+        self.client_version: int = client_version
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.client_id = unpacker.get_int()
-        self.team = unpacker.get_int() # enum TEAM
-        self.silent = unpacker.get_int() == 1
-        self.cooldown_tick = unpacker.get_int()
+        self.version = unpacker.get_str()
+        self.password = unpacker.get_str() # TODO: optionals
+        self.client_version = unpacker.get_int() # TODO: optionals
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.client_id) + \
-            pack_int(self.team) + \
-            pack_int(self.silent) + \
-            pack_int(self.cooldown_tick)
+        return pack_str(self.version) + \
+            pack_str(self.password) + \
+            pack_int(self.client_version)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_tune_params.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_tune_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgSvTuneParams(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             ground_control_speed: float = 10,
             ground_control_accel: float = 2,
@@ -38,14 +39,15 @@
             laser_reach: float = 800,
             laser_bounce_delay: float = 150,
             laser_bounce_num: float = 1,
             laser_bounce_cost: float = 0,
             player_collision: float = 1,
             player_hooking: float = 1
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_tune_params'
         self.system_message: bool = False
         self.message_id: int = 6
         self.header: ChunkHeader = chunk_header
 
         self.ground_control_speed: float = ground_control_speed
         self.ground_control_accel: float = ground_control_accel
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_clear_options.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_list_add.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgSvVoteClearOptions(PrettyPrint):
+class MsgSvVoteOptionListAdd(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'sv_vote_clear_options'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_vote_option_list_add'
         self.system_message: bool = False
-        self.message_id: int = 11
+        self.message_id: int = 12
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_add.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_drop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Literal
 
-class MsgSvVoteOptionAdd(PrettyPrint):
+class MsgSvClientDrop(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            description: str = 'default'
+            client_id: int = 0,
+            reason: str = 'default',
+            silent: bool = False
     ) -> None:
-        self.message_name: str = 'sv_vote_option_add'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_client_drop'
         self.system_message: bool = False
-        self.message_id: int = 13
+        self.message_id: int = 20
         self.header: ChunkHeader = chunk_header
 
-        self.description: str = description
+        self.client_id: int = client_id
+        self.reason: str = reason
+        self.silent: bool = silent
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.description = unpacker.get_str(SANITIZE_CC)
+        self.client_id = unpacker.get_int()
+        self.reason = unpacker.get_str(SANITIZE_CC)
+        self.silent = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.description)
+        return pack_int(self.client_id) + \
+            pack_str(self.reason) + \
+            pack_int(self.silent)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_list_add.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_clear_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgSvVoteOptionListAdd(PrettyPrint):
+class MsgSvVoteClearOptions(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'sv_vote_option_list_add'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_vote_clear_options'
         self.system_message: bool = False
-        self.message_id: int = 12
+        self.message_id: int = 11
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_option_remove.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_remove.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import SANITIZE_CC, pack_str
+from typing import Literal
 
 class MsgSvVoteOptionRemove(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             description: str = 'default'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_vote_option_remove'
         self.system_message: bool = False
         self.message_id: int = 14
         self.header: ChunkHeader = chunk_header
 
         self.description: str = description
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_set.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
-import twnet_parser.enum7 as enum7
+from twnet_parser.packer import SANITIZE_CC, pack_str
+from typing import Literal
 
-class MsgSvVoteSet(PrettyPrint):
+class MsgSvCommandInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            client_id: int = 0,
-            type: int = enum7.Vote.UNKNOWN.value,
-            timeout: int = 0,
-            description: str = 'default',
-            reason: str = 'default'
+            name: str = 'default',
+            args_format: str = 'default',
+            help_text: str = 'default'
     ) -> None:
-        self.message_name: str = 'sv_vote_set'
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_command_info'
         self.system_message: bool = False
-        self.message_id: int = 15
+        self.message_id: int = 37
         self.header: ChunkHeader = chunk_header
 
-        self.client_id: int = client_id
-        self.type: int = type
-        self.timeout: int = timeout
-        self.description: str = description
-        self.reason: str = reason
+        self.name: str = name
+        self.args_format: str = args_format
+        self.help_text: str = help_text
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.client_id = unpacker.get_int()
-        self.type = unpacker.get_int() # enum VOTE
-        self.timeout = unpacker.get_int()
-        self.description = unpacker.get_str(SANITIZE_CC)
-        self.reason = unpacker.get_str(SANITIZE_CC)
+        self.name = unpacker.get_str(SANITIZE_CC)
+        self.args_format = unpacker.get_str(SANITIZE_CC)
+        self.help_text = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.client_id) + \
-            pack_int(self.type) + \
-            pack_int(self.timeout) + \
-            pack_str(self.description) + \
-            pack_str(self.reason)
+        return pack_str(self.name) + \
+            pack_str(self.args_format) + \
+            pack_str(self.help_text)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_vote_status.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgSvVoteStatus(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             yes: int = 0,
             no: int = 0,
             pass_: int = 0,
             total: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_vote_status'
         self.system_message: bool = False
         self.message_id: int = 16
         self.header: ChunkHeader = chunk_header
 
         self.yes: int = yes
         self.no: int = no
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/game/sv_weapon_pickup.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_weapon_pickup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 import twnet_parser.enum7 as enum7
 
 class MsgSvWeaponPickup(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             weapon: int = enum7.Weapon.HAMMER.value
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'game'
         self.message_name: str = 'sv_weapon_pickup'
         self.system_message: bool = False
         self.message_id: int = 9
         self.header: ChunkHeader = chunk_header
 
         self.weapon: int = weapon
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/con_ready.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_on.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgConReady(PrettyPrint):
+class MsgRconAuthOn(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'con_ready'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_auth_on'
         self.system_message: bool = True
-        self.message_id: int = 5
+        self.message_id: int = 11
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/enter_game.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/enter_game.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
 class MsgEnterGame(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'enter_game'
         self.system_message: bool = True
         self.message_id: int = 19
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgInfo(PrettyPrint):
+class MsgRconCmd(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            version: str = '0.7 802f1be60a05665f',
-            password: str = '',
-            client_version: int = 1797
+            cmd: str = 'default'
     ) -> None:
-        self.message_name: str = 'info'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'rcon_cmd'
         self.system_message: bool = True
-        self.message_id: int = 1
+        self.message_id: int = 21
         self.header: ChunkHeader = chunk_header
 
-        self.version: str = version
-        self.password: str = password
-        self.client_version: int = client_version
+        self.cmd: str = cmd
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.version = unpacker.get_str()
-        self.password = unpacker.get_str() # TODO: optionals
-        self.client_version = unpacker.get_int() # TODO: optionals
+        self.cmd = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.version) + \
-            pack_str(self.password) + \
-            pack_int(self.client_version)
+        return pack_str(self.cmd)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/input.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgInput(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             ack_snapshot: int = 0,
             intended_tick: int = 0,
             input_size: int = 0,
             input: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'input'
         self.system_message: bool = True
         self.message_id: int = 20
         self.header: ChunkHeader = chunk_header
 
         self.ack_snapshot: int = ack_snapshot
         self.intended_tick: int = intended_tick
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/input_timing.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/input_timing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal
 
 class MsgInputTiming(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             input_pred_tick: int = 0,
             time_left: int = 0
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'input_timing'
         self.system_message: bool = True
         self.message_id: int = 10
         self.header: ChunkHeader = chunk_header
 
         self.input_pred_tick: int = input_pred_tick
         self.time_left: int = time_left
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/map_change.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/map_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int, pack_str
-from typing import Annotated
+from typing import Annotated, Literal
 
 class MsgMapChange(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default',
             crc: int = 0,
             size: int = 0,
             num_response_chunks_per_request: int = 0,
             chunk_size: int = 0,
             sha256: Annotated[bytes, 32] = bytes(32)
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'map_change'
         self.system_message: bool = True
         self.message_id: int = 2
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
         self.crc: int = crc
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/map_data.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_vote.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import pack_int
+from typing import Literal
 
-class MsgMapData(PrettyPrint):
+class MsgClVote(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            data: bytes = b'\x00'
+            vote: int = 0
     ) -> None:
-        self.message_name: str = 'map_data'
-        self.system_message: bool = True
-        self.message_id: int = 3
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'cl_vote'
+        self.system_message: bool = False
+        self.message_id: int = 31
         self.header: ChunkHeader = chunk_header
 
-        self.data: bytes = data
+        self.vote: int = vote
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.data = unpacker.get_raw()
+        self.vote = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return self.data
+        return pack_int(self.vote)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/maplist_entry_add.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/con_ready.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
-from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgMaplistEntryAdd(PrettyPrint):
+class MsgConReady(PrettyPrint):
     def __init__(
             self,
-            chunk_header: ChunkHeader = ChunkHeader(),
-            name: str = 'default'
+            chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'maplist_entry_add'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'con_ready'
         self.system_message: bool = True
-        self.message_id: int = 29
+        self.message_id: int = 5
         self.header: ChunkHeader = chunk_header
 
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

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/maplist_entry_rem.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/map_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgMaplistEntryRem(PrettyPrint):
+class MsgMapData(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            name: str = 'default'
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name: str = 'maplist_entry_rem'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'map_data'
         self.system_message: bool = True
-        self.message_id: int = 30
+        self.message_id: int = 3
         self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.data = unpacker.get_raw()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return self.data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/ping.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_msg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgPing(PrettyPrint):
+class MsgSvGameMsg(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'ping'
-        self.system_message: bool = True
-        self.message_id: int = 26
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_game_msg'
+        self.system_message: bool = False
+        self.message_id: int = 21
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/ping_reply.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_motd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
+from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgPingReply(PrettyPrint):
+class MsgSvMotd(PrettyPrint):
     def __init__(
             self,
-            chunk_header: ChunkHeader = ChunkHeader()
+            chunk_header: ChunkHeader = ChunkHeader(),
+            message: str = 'default'
     ) -> None:
-        self.message_name: str = 'ping_reply'
-        self.system_message: bool = True
-        self.message_id: int = 27
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_motd'
+        self.system_message: bool = False
+        self.message_id: int = 1
         self.header: ChunkHeader = chunk_header
 
+        self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
+        unpacker = Unpacker(data)
+        self.message = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return b''
+        return pack_str(self.message)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth.py` & `twnet_parser-0.7.0/twnet_parser/messages7/connless/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
-from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.master_server import MastersrvAddr
+from twnet_parser.packer import pack_packed_addresses
+from typing import Literal
 
-class MsgRconAuth(PrettyPrint):
+class MsgList(PrettyPrint):
     def __init__(
             self,
-            chunk_header: ChunkHeader = ChunkHeader(),
-            password: str = 'default'
+            servers: list[MastersrvAddr] = []
     ) -> None:
-        self.message_name: str = 'rcon_auth'
-        self.system_message: bool = True
-        self.message_id: int = 22
-        self.header: ChunkHeader = chunk_header
+        self.message_type: Literal['connless'] = 'connless'
+        self.message_name: str = 'connless.list'
+        self.message_id: list[int] = [255, 255, 255, 255, 108, 105, 115, 50]
 
-        self.password: str = password
+        self.servers: list[MastersrvAddr] = servers
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.password = unpacker.get_str()
+        self.servers = unpacker.get_packed_addresses()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.password)
+        return pack_packed_addresses(self.servers)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth_off.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/server_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
+from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgRconAuthOff(PrettyPrint):
+class MsgServerInfo(PrettyPrint):
     def __init__(
             self,
-            chunk_header: ChunkHeader = ChunkHeader()
+            chunk_header: ChunkHeader = ChunkHeader(),
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name: str = 'rcon_auth_off'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'server_info'
         self.system_message: bool = True
-        self.message_id: int = 12
+        self.message_id: int = 4
         self.header: ChunkHeader = chunk_header
 
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
+        unpacker = Unpacker(data)
+        self.data = unpacker.get_raw()
         return True
 
     def pack(self) -> bytes:
-        return b''
+        return self.data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_auth_on.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/ping.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgRconAuthOn(PrettyPrint):
+class MsgPing(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
-        self.message_name: str = 'rcon_auth_on'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'ping'
         self.system_message: bool = True
-        self.message_id: int = 11
+        self.message_id: int = 26
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_emoticon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import pack_int
+from typing import Literal
+import twnet_parser.enum7 as enum7
 
-class MsgRconCmd(PrettyPrint):
+class MsgClEmoticon(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            cmd: str = 'default'
+            emoticon: int = enum7.Emoticon.OOP.value
     ) -> None:
-        self.message_name: str = 'rcon_cmd'
-        self.system_message: bool = True
-        self.message_id: int = 21
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'cl_emoticon'
+        self.system_message: bool = False
+        self.message_id: int = 30
         self.header: ChunkHeader = chunk_header
 
-        self.cmd: str = cmd
+        self.emoticon: int = emoticon
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.cmd = unpacker.get_str()
+        self.emoticon = unpacker.get_int() # enum EMOTICON
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.cmd)
+        return pack_int(self.emoticon)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd_add.py` & `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
+from typing import Literal
 
-class MsgRconCmdAdd(PrettyPrint):
+class MsgSvVoteOptionAdd(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            name: str = 'default',
-            help: str = 'default',
-            params: str = 'default'
+            description: str = 'default'
     ) -> None:
-        self.message_name: str = 'rcon_cmd_add'
-        self.system_message: bool = True
-        self.message_id: int = 14
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_vote_option_add'
+        self.system_message: bool = False
+        self.message_id: int = 13
         self.header: ChunkHeader = chunk_header
 
-        self.name: str = name
-        self.help: str = help
-        self.params: str = params
+        self.description: str = description
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
-        self.help = unpacker.get_str()
-        self.params = unpacker.get_str()
+        self.description = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_str(self.help) + \
-            pack_str(self.params)
+        return pack_str(self.description)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/rcon_cmd_rem.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_add.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
+from typing import Literal
 
-class MsgRconCmdRem(PrettyPrint):
+class MsgMaplistEntryAdd(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             name: str = 'default'
     ) -> None:
-        self.message_name: str = 'rcon_cmd_rem'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'maplist_entry_add'
         self.system_message: bool = True
-        self.message_id: int = 15
+        self.message_id: int = 29
         self.header: ChunkHeader = chunk_header
 
         self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/ready.py` & `twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_check.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
-from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
-class MsgReady(PrettyPrint):
+class MsgForwardCheck(PrettyPrint):
     def __init__(
-            self,
-            chunk_header: ChunkHeader = ChunkHeader()
+            self
     ) -> None:
-        self.message_name: str = 'ready'
-        self.system_message: bool = True
-        self.message_id: int = 18
-        self.header: ChunkHeader = chunk_header
+        self.message_type: Literal['connless'] = 'connless'
+        self.message_name: str = 'connless.forward_check'
+        self.message_id: list[int] = [255, 255, 255, 255, 102, 119, 63, 63]
 
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         return True
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/request_map_data.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/request_map_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.chunk_header import ChunkHeader
+from typing import Literal
 
 class MsgRequestMapData(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader()
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'request_map_data'
         self.system_message: bool = True
         self.message_id: int = 23
         self.header: ChunkHeader = chunk_header
 
 
     # first byte of data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/server_info.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/snap_empty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
+from twnet_parser.packer import pack_int
+from typing import Literal
 
-class MsgServerInfo(PrettyPrint):
+class MsgSnapEmpty(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            data: bytes = b'\x00'
+            tick: int = 0,
+            delta_tick: int = 0
     ) -> None:
-        self.message_name: str = 'server_info'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'snap_empty'
         self.system_message: bool = True
-        self.message_id: int = 4
+        self.message_id: int = 7
         self.header: ChunkHeader = chunk_header
 
-        self.data: bytes = data
+        self.tick: int = tick
+        self.delta_tick: int = delta_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.data = unpacker.get_raw()
+        self.tick = unpacker.get_int()
+        self.delta_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return self.data
+        return pack_int(self.tick) + \
+            pack_int(self.delta_tick)
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/snap.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/snap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-# generated by scripts/generate_messages.py
+from typing import Literal, Optional
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
-from typing import Optional
+from twnet_parser.snapshot7 import Snapshot
 
 class MsgSnap(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             tick: int = 0,
             delta_tick: int = 0,
             num_parts: int = 0,
             part: int = 0,
             crc: int = 0,
             data_size: Optional[int] = None,
             data: bytes = b'\x00'
     ) -> None:
+        self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'snap'
         self.system_message: bool = True
         self.message_id: int = 6
         self.header: ChunkHeader = chunk_header
 
         self.tick: int = tick
         self.delta_tick: int = delta_tick
         self.num_parts: int = num_parts
         self.part: int = part
         self.crc: int = crc
         self.data_size: int = data_size if data_size else len(data)
         self.data: bytes = data
+        self.snapshot = Snapshot()
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.tick = unpacker.get_int()
         self.delta_tick = unpacker.get_int()
         self.num_parts = unpacker.get_int()
         self.part = unpacker.get_int()
         self.crc = unpacker.get_int()
         self.data_size = unpacker.get_int()
         self.data = unpacker.get_raw(self.data_size)
+        self.snapshot.unpack(self.data)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.tick) + \
             pack_int(self.delta_tick) + \
             pack_int(self.num_parts) + \
             pack_int(self.part) + \
             pack_int(self.crc) + \
             pack_int(self.data_size) + \
-            self.data
+            self.snapshot.pack()
```

### Comparing `twnet_parser-0.6.0/twnet_parser/messages7/system/snap_empty.py` & `twnet_parser-0.7.0/twnet_parser/messages7/system/snap_single.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Literal, Optional
 
-class MsgSnapEmpty(PrettyPrint):
+class MsgSnapSingle(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             tick: int = 0,
-            delta_tick: int = 0
+            delta_tick: int = 0,
+            crc: int = 0,
+            data_size: Optional[int] = None,
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name: str = 'snap_empty'
+        self.message_type: Literal['system', 'game'] = 'system'
+        self.message_name: str = 'snap_single'
         self.system_message: bool = True
-        self.message_id: int = 7
+        self.message_id: int = 8
         self.header: ChunkHeader = chunk_header
 
         self.tick: int = tick
         self.delta_tick: int = delta_tick
+        self.crc: int = crc
+        self.data_size: int = data_size if data_size else len(data)
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.tick = unpacker.get_int()
         self.delta_tick = unpacker.get_int()
+        self.crc = unpacker.get_int()
+        self.data_size = unpacker.get_int()
+        self.data = unpacker.get_raw(self.data_size)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.tick) + \
-            pack_int(self.delta_tick)
+            pack_int(self.delta_tick) + \
+            pack_int(self.crc) + \
+            pack_int(self.data_size) + \
+            self.data
```

### Comparing `twnet_parser-0.6.0/twnet_parser/msg_matcher/control7.py` & `twnet_parser-0.7.0/twnet_parser/msg_matcher/control7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/msg_matcher/game7.py` & `twnet_parser-0.7.0/twnet_parser/msg_matcher/game7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/msg_matcher/system7.py` & `twnet_parser-0.7.0/twnet_parser/msg_matcher/system7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/twnet_parser/packer.py` & `twnet_parser-0.7.0/twnet_parser/packer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
 
-from typing import Final
+from typing import Final, Literal
+
+from twnet_parser.master_server import MastersrvAddr
 
 # Before chaning the current packer code to extend it
 # Consider having two packers
 #
 # One being this one. That is simple and fast.
 # Has no state or side effects.
 # Does no error checking.
@@ -36,14 +38,43 @@
         if size == -1:
             return self.data()
         end: int = self.idx + size
         data: bytes = self._data[self.idx:end]
         self.idx = end
         return data
 
+    def get_packed_addresses(self) -> list[MastersrvAddr]:
+        servers: list[MastersrvAddr] = []
+        while len(self.data()) >= 18:
+            ipaddr = self.get_raw(16)
+            ipv4_mapping = b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF'
+            family: Literal[4, 6] = 4
+            addr_str: str = ''
+            if ipaddr[0:12] == ipv4_mapping:
+                addr_str = f"{ipaddr[12]}.{ipaddr[13]}.{ipaddr[14]}.{ipaddr[15]}"
+            else:
+                # TODO: make ipv6 nicer
+                addr_str = str(ipaddr)
+                family = 6
+            port = self.get_be_uint16() # TODO: i randomly assumed this would work
+            servers.append(MastersrvAddr(family, addr_str, int(port)))
+        return servers
+
+    def get_uint8(self) -> int:
+        res = self.byte()
+        self.idx += 1
+        return res
+
+    def get_be_uint16(self) -> int:
+        left = self.byte()
+        self.idx += 1
+        right = self.byte()
+        self.idx += 1
+        return left << 8 | right
+
     def get_int(self) -> int:
         sign = (self.byte() >> 6) & 1
         res = self.byte() & 0x3F
         # fake loop should only loop once
         # its the poor mans goto hack
         while True:
             if (self.byte() & 0x80) == 0:
@@ -117,14 +148,35 @@
     while num != 0:
         res[i] |= 0x80 # set extend bit
         i += 1
         res.extend(bytes([num & 0x7F])) # pack 7 bit
         num >>= 7 # discard 7 bits
     return bytes(res)
 
+def pack_be_uint16(num: int) -> bytes:
+    high = (num >> 8) & 0xff
+    low = num & 0xff
+    return bytes([high, low])
+
+def pack_uint8(num: int) -> bytes:
+    return bytes([num])
+
+def pack_packed_addresses(servers: list[MastersrvAddr]) -> bytes:
+    res: bytes = b''
+    for server in servers:
+        if server.family == 4:
+            ipv4_mapping = b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xFF\xFF'
+            res += ipv4_mapping
+            res += bytes([int(x) for x in server.ipaddr.split('.')])
+        else:
+            # TODO: ipv6 is wrong
+            res += server.ipaddr.encode('utf-8')
+        res += pack_be_uint16(server.port)
+    return res
+
 def pack_str(data: str) -> bytes:
     return data.encode('utf-8') + b'\x00'
 
 # TODO: optimize performance and benchmark in tests
 def unpack_int(data: bytes) -> int:
     sign = (data[0] >> 6) & 1
     res = data[0] & 0x3F
```

### Comparing `twnet_parser-0.6.0/twnet_parser/packet.py` & `twnet_parser-0.7.0/twnet_parser/packet.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 from typing import Union, cast, Optional
 
 from twnet_parser.packer import Unpacker, pack_int
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.message_parser import MessageParser
 from twnet_parser.net_message import NetMessage
 from twnet_parser.ctrl_message import CtrlMessage
+from twnet_parser.connless_message import ConnlessMessage
 from twnet_parser.chunk_header import ChunkHeader, ChunkFlags
 from twnet_parser.msg_matcher.control7 import match_control7
-from twnet_parser.constants import NET_MAX_SEQUENCE
+from twnet_parser.msg_matcher.connless7 import match_connless7
+from twnet_parser.constants import NET_MAX_SEQUENCE, NET_PACKETVERSION
 
 from twnet_parser.external.huffman import huffman
 
 # TODO: what is a nice pythonic way of storing those?
 #       also does some version:: namespace thing make sense?
 PACKETFLAG7_CONTROL = 1
 PACKETFLAG7_RESEND = 2
 PACKETFLAG7_COMPRESSION = 4
 PACKETFLAG7_CONNLESS = 8
 
 CHUNKFLAG7_VITAL = 1
 CHUNKFLAG7_RESEND = 2
 
 PACKET_HEADER7_SIZE = 7
+CONNLESS_PACKET_HEADER7_SIZE = 9
 
 class PacketFlags7(PrettyPrint):
     def __init__(self) -> None:
         self.control: Optional[bool] = None
         self.resend: Optional[bool] = None
         self.compression: Optional[bool] = None
         self.connless: Optional[bool] = None
@@ -56,14 +59,18 @@
         if not flags:
             flags = PacketFlags7()
         self.flags: PacketFlags7 = flags
         self.ack: int = ack % NET_MAX_SEQUENCE
         self.token: bytes = token
         self.num_chunks: Optional[int] = num_chunks
 
+        # connless only
+        self.connless_version: int = NET_PACKETVERSION
+        self.response_token: bytes = b'\xff\xff\xff\xff'
+
     def pack(self) -> bytes:
         """
         Generate 7 byte teeworlds 0.7 packet header
         based on the current instance variable
         values.
 
         The layout is as follows
@@ -87,59 +94,70 @@
             flags |= PACKETFLAG7_RESEND
         if self.flags.compression:
             flags |= PACKETFLAG7_COMPRESSION
         if self.flags.connless:
             flags |= PACKETFLAG7_CONNLESS
         if self.num_chunks is None:
             self.num_chunks = 0
+        if self.flags.connless:
+            return bytes([ \
+                ((PACKETFLAG7_CONNLESS<<2)&0xfc) | (self.connless_version&0x03)
+            ]) + self.token + self.response_token
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
-        self.messages: list[Union[CtrlMessage, NetMessage]] = []
+        self.messages: list[Union[CtrlMessage, NetMessage, ConnlessMessage]] = []
 
     def pack(self, we_are_a_client = True) -> bytes:
         payload: bytes = b''
-        msg: Union[CtrlMessage, NetMessage]
+        msg: Union[CtrlMessage, NetMessage, ConnlessMessage]
         is_control: bool = False
+        is_connless: bool = False
         for msg in self.messages:
-            # TODO: this is super ugly
-            # revist https://gitlab.com/teeworlds-network/twnet_parser/-/issues/1
-            # we can not check isinstance() not sure why
-            # maybe because CtrlMessage and NetMessage are no actual classes
-            # but just ducktyping helpers
-            if not hasattr(msg, 'system_message'):
+            if msg.message_type == 'connless':
+                is_connless = True
+                msg = cast(ConnlessMessage, msg)
+                payload += bytes(msg.message_id)
+                payload += msg.pack()
+            elif msg.message_type == 'control':
                 is_control = True
                 msg = cast(CtrlMessage, msg)
                 payload += pack_int(msg.message_id)
                 payload += msg.pack(we_are_a_client)
-            else:
+            else: # game or system message
                 msg = cast(NetMessage, msg)
-                msg_payload: bytes = pack_int((msg.message_id<<1)|(int)(msg.system_message))
+                msg_payload: bytes = pack_int(
+                    (msg.message_id<<1) |
+                    (int)(msg.system_message)
+                )
                 msg_payload += msg.pack()
                 if msg.header.size is None:
                     msg.header.size = len(msg_payload)
                 payload += msg.header.pack()
                 payload += msg_payload
         if self.header.num_chunks is None:
             if is_control:
                 self.header.num_chunks = 0
             else:
                 self.header.num_chunks = len(self.messages)
         if is_control:
             if self.header.flags.control is None:
                 self.header.flags.control = True
+        if is_connless:
+            if self.header.flags.connless is None:
+                self.header.flags.connless = True
         return self.header.pack() + payload
 
 class PacketHeaderParser7():
     def parse_flags7(self, data: bytes) -> PacketFlags7:
         # FFFF FFaa
         flag_bits = (data[0] & 0xfc) >> 2
         flags = PacketFlags7()
@@ -160,20 +178,27 @@
     def parse_token(self, header_bytes: bytes) -> bytes:
         return header_bytes[3:7]
 
     def parse_header(self, data: bytes) -> PacketHeader:
         header = PacketHeader()
         # bits 2..5
         header.flags = self.parse_flags7(data)
-        # bits 6..16
-        header.ack = self.parse_ack(data)
-        # bits 17..25
-        header.num_chunks = self.parse_num_chunks(data)
-        # bits 16..57
-        header.token = self.parse_token(data)
+        if header.flags.connless:
+            # TODO: do not hardcode version field
+            #       but actually read the bits
+            header.connless_version = NET_PACKETVERSION
+            header.token = data[1:5]
+            header.response_token = data[5:9]
+        else:
+            # bits 6..16
+            header.ack = self.parse_ack(data)
+            # bits 17..25
+            header.num_chunks = self.parse_num_chunks(data)
+            # bits 16..57
+            header.token = self.parse_token(data)
         return header
 
 class ChunkHeaderParser:
     def parse_flags7(self, data: bytes) -> ChunkFlags:
         # FFss ssss  xxss ssss
         flag_bits = (data[0] >> 6) & 0x03
         flags = ChunkFlags()
@@ -235,25 +260,32 @@
         pck = TwPacket()
         pck.version = '0.7'
         # TODO: what is the most performant way in python to do this?
         #       heap allocating a PacketHeaderParser7 just to bundle a bunch of
         #       methods that do not share state seems like a waste of performance
         #       would this be nicer with class methods?
         pck.header = PacketHeaderParser7().parse_header(data)
-        pck.payload_raw = data[PACKET_HEADER7_SIZE:]
+        header_size = PACKET_HEADER7_SIZE
+        if pck.header.flags.connless:
+            header_size = CONNLESS_PACKET_HEADER7_SIZE
+        pck.payload_raw = data[header_size:]
         pck.payload_decompressed = pck.payload_raw
         if pck.header.flags.control:
             ctrl_msg: CtrlMessage = match_control7(data[7], data[8:], client)
             pck.messages.append(ctrl_msg)
             return pck
+        if pck.header.flags.connless:
+            connless_msg: ConnlessMessage = match_connless7(data[9:17], data[17:])
+            pck.messages.append(connless_msg)
+            return pck
         if pck.header.flags.compression:
             payload = bytearray(pck.payload_raw)
             pck.payload_decompressed = huffman.decompress(payload)
         pck.messages = cast(
-                list[Union[CtrlMessage, NetMessage]],
+                list[Union[CtrlMessage, NetMessage, ConnlessMessage]],
                 self.get_messages(pck.payload_decompressed))
         return pck
 
 def parse6(data: bytes) -> TwPacket:
     raise NotImplementedError()
 
 def parse7(data: bytes, we_are_a_client: bool = True) -> TwPacket:
```

### Comparing `twnet_parser-0.6.0/twnet_parser.egg-info/PKG-INFO` & `twnet_parser-0.7.0/twnet_parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet-parser
-Version: 0.6.0
+Version: 0.7.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -42,23 +42,26 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                    | 0.7                | 0.6                |
-| -------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers | :heavy_check_mark: |                    |
-| Deserialize chunk headers  | :heavy_check_mark: |                    |
-| Deserialize messages       | 85%                |                    |
-| Deserialize snapshots      |                    |                    |
-| Serialize packet headers   | :heavy_check_mark: |                    |
-| Serialize chunk headers    | :heavy_check_mark: |                    |
-| Serialize messages         | 85%                |                    |
+| Feature                      | 0.7                | 0.6                |
+| ---------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers   | :heavy_check_mark: |                    |
+| Deserialize chunk headers    | :heavy_check_mark: |                    |
+| Deserialize messages         | 85%                |                    |
+| Deserialize snapshots        |                    |                    |
+| Deserialize connless packets | :heavy_check_mark: |                    |
+| Serialize packet headers     | :heavy_check_mark: |                    |
+| Serialize chunk headers      | :heavy_check_mark: |                    |
+| Serialize messages           | 85%                |                    |
+| Serialize snapshots          |                    |                    |
+| Serialize connless packets   | :heavy_check_mark: |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.6.0/twnet_parser.egg-info/SOURCES.txt` & `twnet_parser-0.7.0/twnet_parser.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,42 @@
 tests/packet_invalid_test.py
 tests/packet_with_chunks7_test.py
 tests/repack_chunks7_test.py
 tests/unpacker_state_test.py
 tests/msg7/sv_tune_params_test.py
 twnet_parser/__init__.py
 twnet_parser/chunk_header.py
+twnet_parser/connless_message.py
 twnet_parser/constants.py
 twnet_parser/ctrl_message.py
 twnet_parser/enum7.py
+twnet_parser/master_server.py
 twnet_parser/message_parser.py
 twnet_parser/msg7.py
 twnet_parser/net_message.py
 twnet_parser/packer.py
 twnet_parser/packet.py
 twnet_parser/pretty_print.py
+twnet_parser/snapshot7.py
 twnet_parser.egg-info/PKG-INFO
 twnet_parser.egg-info/SOURCES.txt
 twnet_parser.egg-info/dependency_links.txt
 twnet_parser.egg-info/top_level.txt
 twnet_parser/external/huffman.py
+twnet_parser/messages7/connless/count.py
+twnet_parser/messages7/connless/forward_check.py
+twnet_parser/messages7/connless/forward_error.py
+twnet_parser/messages7/connless/forward_ok.py
+twnet_parser/messages7/connless/forward_response.py
+twnet_parser/messages7/connless/heartbeat.py
+twnet_parser/messages7/connless/info.py
+twnet_parser/messages7/connless/list.py
+twnet_parser/messages7/connless/request_count.py
+twnet_parser/messages7/connless/request_info.py
+twnet_parser/messages7/connless/request_list.py
 twnet_parser/messages7/control/accept.py
 twnet_parser/messages7/control/close.py
 twnet_parser/messages7/control/connect.py
 twnet_parser/messages7/control/keep_alive.py
 twnet_parser/messages7/control/token.py
 twnet_parser/messages7/game/cl_call_vote.py
 twnet_parser/messages7/game/cl_command.py
@@ -97,14 +111,15 @@
 twnet_parser/messages7/system/rcon_line.py
 twnet_parser/messages7/system/ready.py
 twnet_parser/messages7/system/request_map_data.py
 twnet_parser/messages7/system/server_info.py
 twnet_parser/messages7/system/snap.py
 twnet_parser/messages7/system/snap_empty.py
 twnet_parser/messages7/system/snap_single.py
+twnet_parser/msg_matcher/connless7.py
 twnet_parser/msg_matcher/control7.py
 twnet_parser/msg_matcher/game7.py
 twnet_parser/msg_matcher/system7.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
 venv/bin/rst2html5.py
 venv/bin/rst2latex.py
```

### Comparing `twnet_parser-0.6.0/venv/bin/rst2html.py` & `twnet_parser-0.7.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2html4.py` & `twnet_parser-0.7.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2html5.py` & `twnet_parser-0.7.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2latex.py` & `twnet_parser-0.7.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2man.py` & `twnet_parser-0.7.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2odt.py` & `twnet_parser-0.7.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2odt_prepstyles.py` & `twnet_parser-0.7.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2pseudoxml.py` & `twnet_parser-0.7.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2s5.py` & `twnet_parser-0.7.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2xetex.py` & `twnet_parser-0.7.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rst2xml.py` & `twnet_parser-0.7.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.6.0/venv/bin/rstpep2html.py` & `twnet_parser-0.7.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

