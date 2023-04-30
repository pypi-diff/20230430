# Comparing `tmp/ms_api-0.9.59.tar.gz` & `tmp/ms_api-0.9.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms_api-0.9.59.tar", last modified: Sat Apr 10 03:58:47 2021, max compression
+gzip compressed data, was "dist/ms_api-0.9.70.tar", last modified: Wed Apr 28 05:30:17 2021, max compression
```

## Comparing `ms_api-0.9.59.tar` & `ms_api-0.9.70.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-10 03:58:47.444373 ms_api-0.9.59/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      608 2021-04-10 03:58:47.444373 ms_api-0.9.59/PKG-INFO
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1264 2020-09-08 05:27:18.000000 ms_api-0.9.59/README.md
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-10 03:58:47.444373 ms_api-0.9.59/ms/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        0 2020-09-08 05:08:56.000000 ms_api-0.9.59/ms/__init__.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3351 2020-09-08 05:08:56.000000 ms_api-0.9.59/ms/base.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1943 2020-09-08 05:08:56.000000 ms_api-0.9.59/ms/generate_proto_file.py
--rwxrwxr-x   0 nihisil   (1000) nihisil   (1000)     2811 2020-09-08 05:08:56.000000 ms_api-0.9.59/ms/ms-plugin.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)  1485615 2021-04-10 03:58:04.000000 ms_api-0.9.59/ms/protocol_pb2.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    53810 2021-04-10 03:56:32.000000 ms_api-0.9.59/ms/rpc.py
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-10 03:58:47.444373 ms_api-0.9.59/ms_api.egg-info/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      608 2021-04-10 03:58:47.000000 ms_api-0.9.59/ms_api.egg-info/PKG-INFO
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      264 2021-04-10 03:58:47.000000 ms_api-0.9.59/ms_api.egg-info/SOURCES.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        1 2021-04-10 03:58:47.000000 ms_api-0.9.59/ms_api.egg-info/dependency_links.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       48 2021-04-10 03:58:47.000000 ms_api-0.9.59/ms_api.egg-info/requires.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        3 2021-04-10 03:58:47.000000 ms_api-0.9.59/ms_api.egg-info/top_level.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       38 2021-04-10 03:58:47.444373 ms_api-0.9.59/setup.cfg
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      819 2021-04-10 03:58:04.000000 ms_api-0.9.59/setup.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-28 05:30:17.697175 ms_api-0.9.70/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      608 2021-04-28 05:30:17.697175 ms_api-0.9.70/PKG-INFO
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1277 2021-04-28 05:26:36.000000 ms_api-0.9.70/README.md
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-28 05:30:17.697175 ms_api-0.9.70/ms/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        0 2020-09-08 05:08:56.000000 ms_api-0.9.70/ms/__init__.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3351 2020-09-08 05:08:56.000000 ms_api-0.9.70/ms/base.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1943 2020-09-08 05:08:56.000000 ms_api-0.9.70/ms/generate_proto_file.py
+-rwxrwxr-x   0 nihisil   (1000) nihisil   (1000)     2811 2020-09-08 05:08:56.000000 ms_api-0.9.70/ms/ms-plugin.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)  1504477 2021-04-28 05:26:47.000000 ms_api-0.9.70/ms/protocol_pb2.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    53810 2021-04-28 05:26:51.000000 ms_api-0.9.70/ms/rpc.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-04-28 05:30:17.697175 ms_api-0.9.70/ms_api.egg-info/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      608 2021-04-28 05:30:17.000000 ms_api-0.9.70/ms_api.egg-info/PKG-INFO
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      264 2021-04-28 05:30:17.000000 ms_api-0.9.70/ms_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        1 2021-04-28 05:30:17.000000 ms_api-0.9.70/ms_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       54 2021-04-28 05:30:17.000000 ms_api-0.9.70/ms_api.egg-info/requires.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        3 2021-04-28 05:30:17.000000 ms_api-0.9.70/ms_api.egg-info/top_level.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       38 2021-04-28 05:30:17.697175 ms_api-0.9.70/setup.cfg
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      819 2021-04-28 05:29:56.000000 ms_api-0.9.70/setup.py
```

### Comparing `ms_api-0.9.59/PKG-INFO` & `ms_api-0.9.70/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ms_api
-Version: 0.9.59
+Version: 0.9.70
 Summary: Python wrapper for the Mahjong Soul (Majsoul) Protobuf objects. It allows to use their API.
 Home-page: https://github.com/MahjongRepository/mahjong_soul_api
 Author: Nihisil
 Author-email: alexey@nihisil.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ms_api-0.9.59/README.md` & `ms_api-0.9.70/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 The idea of repository based on https://github.com/chaserhkj/PyMajSoul/
 
 Python wrappers for Majsoul allow you to interact with their servers from Python scripts.
 
 ## For User
 
-1. Install python packages from `requerements.txt`
+1. Install python packages from `requirements.txt`
 2. `python example.py -u username -p password`
 
 This example is working only with **Python3.7+**.
 
-Also, you need to have a Chinese account to run this example, because only accounts from these servers has the ability to login with login and password.
+Also, you need to have an account fron CN server to run this example, because only accounts from CN server has the ability to login with login and password.
 
-If you want to login to EN or JP servers you need to write your code to authenticate via email code or social network. Protobuf wrapper from this repository contains all needed API objects.
+If you want to login to EN or JP servers you need to write your code to authenticate via email code or social network. Protobuf wrapper from this repository contains all needed API objects for that.
 
 ## For Developer
 
 ### Requirements
 
 1. Install python packages from `requerements.txt`
 1. Install protobuf compiler `sudo apt install protobuf-compiler`
```

### Comparing `ms_api-0.9.59/ms/base.py` & `ms_api-0.9.70/ms/base.py`

 * *Files identical despite different names*

### Comparing `ms_api-0.9.59/ms/generate_proto_file.py` & `ms_api-0.9.70/ms/generate_proto_file.py`

 * *Files identical despite different names*

### Comparing `ms_api-0.9.59/ms/ms-plugin.py` & `ms_api-0.9.70/ms/ms-plugin.py`

 * *Files identical despite different names*

### Comparing `ms_api-0.9.59/ms/protocol_pb2.py` & `ms_api-0.9.70/ms/protocol_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='protocol.proto',
   package='lq',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n\x0eprotocol.proto\x12\x02lq\"c\n\x13NotifyRoomGameStart\x12\x10\n\x08game_url\x18\x01 \x01(\t\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\"{\n\x14NotifyMatchGameStart\x12\x10\n\x08game_url\x18\x01 \x01(\t\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x15\n\rmatch_mode_id\x18\x04 \x01(\r\x12\x10\n\x08location\x18\x05 \x01(\t\"\xc2\x01\n\x15NotifyRoomPlayerReady\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05ready\x18\x02 \x01(\x08\x12\x41\n\x0c\x61\x63\x63ount_list\x18\x03 \x01(\x0b\x32+.lq.NotifyRoomPlayerReady.AccountReadyState\x12\x0b\n\x03seq\x18\x04 \x01(\r\x1a\x36\n\x11\x41\x63\x63ountReadyState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05ready\x18\x02 \x01(\x08\"\xd4\x01\n\x18NotifyRoomPlayerDressing\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08\x64ressing\x18\x02 \x01(\x08\x12G\n\x0c\x61\x63\x63ount_list\x18\x03 \x01(\x0b\x32\x31.lq.NotifyRoomPlayerDressing.AccountDressingState\x12\x0b\n\x03seq\x18\x04 \x01(\r\x1a<\n\x14\x41\x63\x63ountDressingState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08\x64ressing\x18\x02 \x01(\x08\"\xb3\x01\n\x16NotifyRoomPlayerUpdate\x12\'\n\x0bupdate_list\x18\x01 \x03(\x0b\x32\x12.lq.PlayerBaseView\x12\x13\n\x0bremove_list\x18\x02 \x03(\r\x12\x10\n\x08owner_id\x18\x03 \x01(\r\x12\x13\n\x0brobot_count\x18\x04 \x01(\r\x12\'\n\x0bplayer_list\x18\x05 \x03(\x0b\x32\x12.lq.PlayerBaseView\x12\x0b\n\x03seq\x18\x06 \x01(\r\"\x13\n\x11NotifyRoomKickOut\"Z\n\x17NotifyFriendStateChange\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12,\n\x0c\x61\x63tive_state\x18\x02 \x01(\x0b\x32\x16.lq.AccountActiveState\"M\n\x16NotifyFriendViewChange\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12 \n\x04\x62\x61se\x18\x02 \x01(\x0b\x32\x12.lq.PlayerBaseView\"R\n\x12NotifyFriendChange\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x1a\n\x06\x66riend\x18\x03 \x01(\x0b\x32\n.lq.Friend\"R\n\x14NotifyNewFriendApply\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\napply_time\x18\x02 \x01(\r\x12\x12\n\nremoved_id\x18\x03 \x01(\r\"X\n\x13NotifyClientMessage\x12\"\n\x06sender\x18\x01 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"8\n\x13NotifyAccountUpdate\x12!\n\x06update\x18\x01 \x01(\x0b\x32\x11.lq.AccountUpdate\"\x14\n\x12NotifyAnotherLogin\"\x15\n\x13NotifyAccountLogout\"_\n\x18NotifyAnnouncementUpdate\x12\'\n\rannouncements\x18\x01 \x03(\x0b\x32\x10.lq.Announcement\x12\x0c\n\x04sort\x18\x02 \x03(\r\x12\x0c\n\x04lang\x18\x03 \x01(\t\"\'\n\rNotifyNewMail\x12\x16\n\x04mail\x18\x01 \x01(\x0b\x32\x08.lq.Mail\"(\n\x10NotifyDeleteMail\x12\x14\n\x0cmail_id_list\x18\x01 \x03(\r\",\n\x16NotifyReviveCoinUpdate\x12\x12\n\nhas_gained\x18\x01 \x01(\x08\"r\n\x15NotifyDailyTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x1c\n\x14max_daily_task_count\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\"@\n\x18NotifyActivityTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"F\n\x1eNotifyActivityPeriodTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"E\n\x1dNotifyAccountRandomTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"\xaf\x01\n NotifyAccountChallengeTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\r\n\x05level\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\x13\n\x0bmatch_count\x18\x04 \x01(\r\x12\x11\n\tticket_id\x18\x05 \x01(\r\x12\x17\n\x0frewarded_season\x18\x06 \x03(\r\"\x12\n\x10NotifyNewComment\"8\n\x13NotifyRollingNotice\x12!\n\x06notice\x18\x01 \x01(\x0b\x32\x11.lq.RollingNotice\"\x17\n\x15NotifyGiftSendRefresh\"3\n\x10NotifyShopUpdate\x12\x1f\n\tshop_info\x18\x01 \x01(\x0b\x32\x0c.lq.ShopInfo\"\xb7\x01\n\x14NotifyVipLevelChange\x12\x12\n\ngift_limit\x18\x01 \x01(\r\x12\x18\n\x10\x66riend_max_count\x18\x02 \x01(\r\x12\x1e\n\x16zhp_free_refresh_limit\x18\x03 \x01(\r\x12\x1e\n\x16zhp_cost_refresh_limit\x18\x04 \x01(\r\x12\x13\n\x0b\x62uddy_bonus\x18\x05 \x01(\x02\x12\x1c\n\x14record_collect_limit\x18\x06 \x01(\r\";\n\x13NotifyServerSetting\x12$\n\x08settings\x18\x01 \x01(\x0b\x32\x12.lq.ServerSettings\"\xdc\x01\n\x0fNotifyPayResult\x12\x12\n\npay_result\x18\x01 \x01(\r\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x10\n\x08goods_id\x18\x03 \x01(\r\x12\x18\n\x10new_month_ticket\x18\x04 \x01(\r\x12;\n\x0fresource_modify\x18\x05 \x03(\x0b\x32\".lq.NotifyPayResult.ResourceModify\x1a:\n\x0eResourceModify\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\"y\n\x1dNotifyCustomContestAccountMsg\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x0e\n\x06sender\x18\x03 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12\x10\n\x08verified\x18\x05 \x01(\r\"\xb1\x01\n\x1cNotifyCustomContestSystemMsg\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x32\n\ngame_start\x18\x04 \x01(\x0b\x32\x1e.lq.CustomizedContestGameStart\x12.\n\x08game_end\x18\x05 \x01(\x0b\x32\x1c.lq.CustomizedContestGameEnd\"!\n\x12NotifyMatchTimeout\x12\x0b\n\x03sid\x18\x01 \x01(\t\"<\n\x18NotifyCustomContestState\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\"T\n\x14NotifyActivityChange\x12$\n\x0enew_activities\x18\x01 \x03(\x0b\x32\x0c.lq.Activity\x12\x16\n\x0e\x65nd_activities\x18\x02 \x03(\r\"H\n\x0fNotifyAFKResult\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x62\x61n_end_time\x18\x02 \x01(\r\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\"Q\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x12\n\nu32_params\x18\x02 \x03(\r\x12\x12\n\nstr_params\x18\x03 \x03(\t\x12\x12\n\njson_param\x18\x04 \x01(\t\"%\n\x07Wrapper\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"@\n\x0fNetworkEndpoint\x12\x0e\n\x06\x66\x61mily\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x0b\n\tReqCommon\"%\n\tResCommon\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"O\n\x10ResAccountUpdate\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x06update\x18\x02 \x01(\x0b\x32\x11.lq.AccountUpdate\"(\n\rAntiAddiction\x12\x17\n\x0fonline_duration\x18\x01 \x01(\r\"\xcf\x07\n\x17\x41\x63\x63ountMahjongStatistic\x12\x1d\n\x15\x66inal_position_counts\x18\x01 \x03(\r\x12>\n\x0crecent_round\x18\x02 \x01(\x0b\x32(.lq.AccountMahjongStatistic.RoundSummary\x12\x38\n\trecent_hu\x18\x03 \x01(\x0b\x32%.lq.AccountMahjongStatistic.HuSummary\x12?\n\nhighest_hu\x18\x04 \x01(\x0b\x32+.lq.AccountMahjongStatistic.HighestHuRecord\x12G\n\x14recent_20_hu_summary\x18\x06 \x01(\x0b\x32).lq.AccountMahjongStatistic.Liqi20Summary\x12G\n\x14recent_10_hu_summary\x18\x07 \x01(\x0b\x32).lq.AccountMahjongStatistic.LiQi10Summary\x12\x45\n\x15recent_10_game_result\x18\x08 \x03(\x0b\x32&.lq.AccountMahjongStatistic.GameResult\x1a\x64\n\x0cRoundSummary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x12\n\nrong_count\x18\x02 \x01(\r\x12\x12\n\nzimo_count\x18\x03 \x01(\r\x12\x17\n\x0f\x66\x61ngchong_count\x18\x04 \x01(\r\x1aM\n\tHuSummary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x18\n\x10\x64ora_round_count\x18\x02 \x01(\r\x12\x11\n\ttotal_fan\x18\x03 \x01(\r\x1a\x7f\n\x0fHighestHuRecord\x12\x0e\n\x06\x66\x61nshu\x18\x01 \x01(\r\x12\x0f\n\x07\x64oranum\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\t\x12\r\n\x05hands\x18\x04 \x03(\t\x12\x0c\n\x04ming\x18\x05 \x03(\t\x12\r\n\x05hupai\x18\x06 \x01(\t\x12\x10\n\x08title_id\x18\x07 \x01(\r\x1aZ\n\rLiqi20Summary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x1a\n\x12total_lidora_count\x18\x02 \x01(\r\x12\x18\n\x10\x61verage_hu_point\x18\x03 \x01(\r\x1a>\n\rLiQi10Summary\x12\x17\n\x0ftotal_xuanshang\x18\x01 \x01(\r\x12\x14\n\x0ctotal_fanshu\x18\x02 \x01(\r\x1a/\n\nGameResult\x12\x0c\n\x04rank\x18\x01 \x01(\r\x12\x13\n\x0b\x66inal_point\x18\x02 \x01(\x05\"\x8a\x01\n\x14\x41\x63\x63ountStatisticData\x12\x18\n\x10mahjong_category\x18\x01 \x01(\r\x12\x15\n\rgame_category\x18\x02 \x01(\r\x12.\n\tstatistic\x18\x03 \x01(\x0b\x32\x1b.lq.AccountMahjongStatistic\x12\x11\n\tgame_type\x18\x04 \x01(\r\")\n\x0c\x41\x63\x63ountLevel\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\r\")\n\x08ViewSlot\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\x0f\n\x07item_id\x18\x02 \x01(\r\"\x84\x07\n\x07\x41\x63\x63ount\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x12\n\nlogin_time\x18\x03 \x01(\r\x12\x13\n\x0blogout_time\x18\x04 \x01(\r\x12\x0f\n\x07room_id\x18\x05 \x01(\r\x12)\n\x0e\x61nti_addiction\x18\x06 \x01(\x0b\x32\x11.lq.AntiAddiction\x12\r\n\x05title\x18\x07 \x01(\r\x12\x11\n\tsignature\x18\x08 \x01(\t\x12\r\n\x05\x65mail\x18\t \x01(\t\x12\x14\n\x0c\x65mail_verify\x18\n \x01(\r\x12\x0c\n\x04gold\x18\x0b \x01(\r\x12\x0f\n\x07\x64iamond\x18\x0c \x01(\r\x12\x11\n\tavatar_id\x18\r \x01(\r\x12\x0b\n\x03vip\x18\x0e \x01(\r\x12\x10\n\x08\x62irthday\x18\x0f \x01(\x05\x12\r\n\x05phone\x18\x10 \x01(\t\x12\x14\n\x0cphone_verify\x18\x11 \x01(\r\x12\x35\n\x10platform_diamond\x18\x12 \x03(\x0b\x32\x1b.lq.Account.PlatformDiamond\x12\x1f\n\x05level\x18\x15 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x16 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x17 \x01(\r\x12\x13\n\x0bskin_ticket\x18\x18 \x01(\r\x12<\n\x14platform_skin_ticket\x18\x19 \x03(\x0b\x32\x1e.lq.Account.PlatformSkinTicket\x12\x10\n\x08verified\x18\x1a \x01(\r\x12\x34\n\x10\x63hallenge_levels\x18\x1b \x03(\x0b\x32\x1a.lq.Account.ChallengeLevel\x12\x37\n\x11\x61\x63hievement_count\x18\x1c \x03(\x0b\x32\x1c.lq.Account.AchievementCount\x1a,\n\x0fPlatformDiamond\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x1a/\n\x12PlatformSkinTicket\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x1a=\n\x0e\x43hallengeLevel\x12\x0e\n\x06season\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0c\n\x04rank\x18\x03 \x01(\r\x1a/\n\x10\x41\x63hievementCount\x12\x0c\n\x04rare\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"-\n\x10\x41\x63\x63ountOwnerData\x12\x19\n\x11unlock_characters\x18\x01 \x03(\r\"\xde\x0c\n\rAccountUpdate\x12\x34\n\tnumerical\x18\x01 \x03(\x0b\x32!.lq.AccountUpdate.NumericalUpdate\x12\x34\n\tcharacter\x18\x02 \x01(\x0b\x32!.lq.AccountUpdate.CharacterUpdate\x12\x1a\n\x03\x62\x61g\x18\x03 \x01(\x0b\x32\r.lq.BagUpdate\x12\x38\n\x0b\x61\x63hievement\x18\x04 \x01(\x0b\x32#.lq.AccountUpdate.AchievementUpdate\x12#\n\x07shilian\x18\x05 \x01(\x0b\x32\x12.lq.AccountShiLian\x12\x35\n\ndaily_task\x18\x06 \x01(\x0b\x32!.lq.AccountUpdate.DailyTaskUpdate\x12,\n\x05title\x18\x07 \x01(\x0b\x32\x1d.lq.AccountUpdate.TitleUpdate\x12\x1a\n\x12new_recharged_list\x18\x08 \x03(\r\x12\x33\n\ractivity_task\x18\t \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12\x38\n\x12\x61\x63tivity_flip_task\x18\n \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12:\n\x14\x61\x63tivity_period_task\x18\x0b \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12:\n\x14\x61\x63tivity_random_task\x18\x0c \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12;\n\tchallenge\x18\r \x01(\x0b\x32(.lq.AccountUpdate.AccountChallengeUpdate\x12\x38\n\x08\x61\x62_match\x18\x0e \x01(\x0b\x32&.lq.AccountUpdate.AccountABMatchUpdate\x1a,\n\x0fNumericalUpdate\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\x1aw\n\x0f\x43haracterUpdate\x12!\n\ncharacters\x18\x02 \x03(\x0b\x32\r.lq.Character\x12\r\n\x05skins\x18\x03 \x03(\r\x12\x18\n\x10\x66inished_endings\x18\x04 \x03(\r\x12\x18\n\x10rewarded_endings\x18\x05 \x03(\r\x1aX\n\x11\x41\x63hievementUpdate\x12+\n\nprogresses\x18\x01 \x03(\x0b\x32\x17.lq.AchievementProgress\x12\x16\n\x0erewarded_group\x18\x02 \x03(\r\x1aJ\n\x0f\x44\x61ilyTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x11\n\ttask_list\x18\x02 \x03(\r\x1a\x38\n\x0bTitleUpdate\x12\x12\n\nnew_titles\x18\x01 \x03(\r\x12\x15\n\rremove_titles\x18\x02 \x03(\r\x1a\x45\n\nTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x11\n\ttask_list\x18\x02 \x03(\r\x1a\xb8\x01\n\x16\x41\x63\x63ountChallengeUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\r\n\x05level\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\x13\n\x0bmatch_count\x18\x04 \x01(\r\x12\x11\n\tticket_id\x18\x05 \x01(\r\x12\x11\n\ttask_list\x18\x06 \x03(\r\x12\x17\n\x0frewarded_season\x18\x07 \x03(\r\x1a\xfd\x01\n\x14\x41\x63\x63ountABMatchUpdate\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\x13\n\x0bmatch_count\x18\x02 \x01(\r\x12\x14\n\x0c\x62uy_in_count\x18\x03 \x01(\r\x12\r\n\x05point\x18\x04 \x01(\r\x12\x10\n\x08rewarded\x18\x05 \x01(\x08\x12J\n\x0fmatch_max_point\x18\x06 \x03(\x0b\x32\x31.lq.AccountUpdate.AccountABMatchUpdate.MatchPoint\x12\x0c\n\x04quit\x18\x07 \x01(\x08\x1a-\n\nMatchPoint\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"E\n\x0cGameMetaData\x12\x0f\n\x07room_id\x18\x01 \x01(\r\x12\x0f\n\x07mode_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63ontest_uid\x18\x03 \x01(\r\"Y\n\x12\x41\x63\x63ountPlayingGame\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\r\x12\x1e\n\x04meta\x18\x03 \x01(\x0b\x32\x10.lq.GameMetaData\"\xa2\x03\n\x10\x41\x63\x63ountCacheView\x12\x15\n\rcache_version\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x12\n\nlogin_time\x18\x04 \x01(\r\x12\x13\n\x0blogout_time\x18\x05 \x01(\r\x12\x11\n\tis_online\x18\x06 \x01(\x08\x12\x0f\n\x07room_id\x18\x07 \x01(\r\x12\r\n\x05title\x18\x08 \x01(\r\x12\x11\n\tavatar_id\x18\t \x01(\r\x12\x0b\n\x03vip\x18\n \x01(\r\x12\x1f\n\x05level\x18\x0b \x01(\x0b\x32\x10.lq.AccountLevel\x12,\n\x0cplaying_game\x18\x0c \x01(\x0b\x32\x16.lq.AccountPlayingGame\x12 \n\x06level3\x18\r \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x0e \x01(\r\x12\x10\n\x08verified\x18\x0f \x01(\r\x12\x14\n\x0c\x62\x61n_deadline\x18\x10 \x01(\r\x12\x13\n\x0b\x63omment_ban\x18\x11 \x01(\r\x12\x11\n\tban_state\x18\x12 \x01(\r\"\xd6\x01\n\x0ePlayerBaseView\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x11\n\tavatar_id\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\r\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x1f\n\x05level\x18\x05 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x06 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x07 \x01(\r\x12\x10\n\x08verified\x18\x08 \x01(\r\x12\x11\n\tis_banned\x18\t \x01(\r\"\x82\x02\n\x0ePlayerGameView\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x11\n\tavatar_id\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\r\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x1f\n\x05level\x18\x05 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\tcharacter\x18\x06 \x01(\x0b\x32\r.lq.Character\x12 \n\x06level3\x18\x07 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x08 \x01(\r\x12\x10\n\x08verified\x18\t \x01(\r\x12\x1b\n\x05views\x18\n \x03(\x0b\x32\x0c.lq.ViewSlot\"#\n\x0bGameSetting\x12\x14\n\x0c\x65moji_switch\x18\x01 \x01(\r\"\xc4\x01\n\x08GameMode\x12\x0c\n\x04mode\x18\x01 \x01(\r\x12\n\n\x02\x61i\x18\x04 \x01(\x08\x12\x12\n\nextendinfo\x18\x05 \x01(\t\x12\'\n\x0b\x64\x65tail_rule\x18\x06 \x01(\x0b\x32\x12.lq.GameDetailRule\x12:\n\x13testing_environment\x18\x07 \x01(\x0b\x32\x1d.lq.GameTestingEnvironmentSet\x12%\n\x0cgame_setting\x18\x08 \x01(\x0b\x32\x0f.lq.GameSetting\"@\n\x19GameTestingEnvironmentSet\x12\x0f\n\x07paixing\x18\x01 \x01(\r\x12\x12\n\nleft_count\x18\x02 \x01(\r\"\xa6\t\n\x0eGameDetailRule\x12\x12\n\ntime_fixed\x18\x01 \x01(\r\x12\x10\n\x08time_add\x18\x02 \x01(\r\x12\x12\n\ndora_count\x18\x03 \x01(\r\x12\x0f\n\x07shiduan\x18\x04 \x01(\r\x12\x12\n\ninit_point\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61ndian\x18\x06 \x01(\r\x12\x11\n\tcan_jifei\x18\x07 \x01(\x08\x12\x16\n\x0etianbian_value\x18\x08 \x01(\r\x12\x16\n\x0eliqibang_value\x18\t \x01(\r\x12\x17\n\x0f\x63hangbang_value\x18\n \x01(\r\x12\x15\n\rnoting_fafu_1\x18\x0b \x01(\r\x12\x15\n\rnoting_fafu_2\x18\x0c \x01(\r\x12\x15\n\rnoting_fafu_3\x18\r \x01(\r\x12\x19\n\x11have_liujumanguan\x18\x0e \x01(\x08\x12\x1c\n\x14have_qieshangmanguan\x18\x0f \x01(\x08\x12\x16\n\x0ehave_biao_dora\x18\x10 \x01(\x08\x12\x1b\n\x13have_gang_biao_dora\x18\x11 \x01(\x08\x12\"\n\x1aming_dora_immediately_open\x18\x12 \x01(\x08\x12\x14\n\x0chave_li_dora\x18\x13 \x01(\x08\x12\x19\n\x11have_gang_li_dora\x18\x14 \x01(\x08\x12\x19\n\x11have_sifenglianda\x18\x15 \x01(\x08\x12\x18\n\x10have_sigangsanle\x18\x16 \x01(\x08\x12\x17\n\x0fhave_sijializhi\x18\x17 \x01(\x08\x12\x1b\n\x13have_jiuzhongjiupai\x18\x18 \x01(\x08\x12\x17\n\x0fhave_sanjiahele\x18\x19 \x01(\x08\x12\x14\n\x0chave_toutiao\x18\x1a \x01(\x08\x12\x1b\n\x13have_helelianzhuang\x18\x1b \x01(\x08\x12\x18\n\x10have_helezhongju\x18\x1c \x01(\x08\x12\x1e\n\x16have_tingpailianzhuang\x18\x1d \x01(\x08\x12\x1b\n\x13have_tingpaizhongju\x18\x1e \x01(\x08\x12\x11\n\thave_yifa\x18\x1f \x01(\x08\x12\x16\n\x0ehave_nanruxiru\x18  \x01(\x08\x12\x18\n\x10jingsuanyuandian\x18! \x01(\r\x12\x13\n\x0bshunweima_2\x18\" \x01(\x05\x12\x13\n\x0bshunweima_3\x18# \x01(\x05\x12\x13\n\x0bshunweima_4\x18$ \x01(\x05\x12\x14\n\x0c\x62ianjietishi\x18% \x01(\x08\x12\x10\n\x08\x61i_level\x18& \x01(\r\x12\x14\n\x0chave_zimosun\x18\' \x01(\x08\x12\x1d\n\x15\x64isable_multi_yukaman\x18( \x01(\x08\x12\r\n\x05\x66\x61nfu\x18) \x01(\r\x12\x11\n\tguyi_mode\x18* \x01(\r\x12\x12\n\ndora3_mode\x18+ \x01(\r\x12\x17\n\x0f\x62\x65gin_open_mode\x18, \x01(\r\x12\x14\n\x0cjiuchao_mode\x18- \x01(\r\x12\x11\n\tmuyu_mode\x18. \x01(\r\x12\x11\n\topen_hand\x18/ \x01(\r\x12\x14\n\x0cxuezhandaodi\x18\x30 \x01(\r\x12\x14\n\x0chuansanzhang\x18\x31 \x01(\r\x12\x1a\n\x12\x64isable_leijiyiman\x18< \x01(\x08\"\xfa\x01\n\x04Room\x12\x0f\n\x07room_id\x18\x01 \x01(\r\x12\x10\n\x08owner_id\x18\x02 \x01(\r\x12\x1a\n\x04mode\x18\x03 \x01(\x0b\x32\x0c.lq.GameMode\x12\x18\n\x10max_player_count\x18\x04 \x01(\r\x12#\n\x07persons\x18\x05 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x12\n\nready_list\x18\x06 \x03(\r\x12\x12\n\nis_playing\x18\x07 \x01(\x08\x12\x13\n\x0bpublic_live\x18\x08 \x01(\x08\x12\x13\n\x0brobot_count\x18\t \x01(\r\x12\x15\n\rtournament_id\x18\n \x01(\r\x12\x0b\n\x03seq\x18\x0b \x01(\r\"\xc1\x01\n\rGameEndResult\x12-\n\x07players\x18\x01 \x03(\x0b\x32\x1c.lq.GameEndResult.PlayerItem\x1a\x80\x01\n\nPlayerItem\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x13\n\x0btotal_point\x18\x02 \x01(\x05\x12\x14\n\x0cpart_point_1\x18\x03 \x01(\x05\x12\x14\n\x0cpart_point_2\x18\x04 \x01(\x05\x12\x15\n\rgrading_score\x18\x05 \x01(\x05\x12\x0c\n\x04gold\x18\x06 \x01(\x05\"M\n\x0fGameConnectInfo\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\"0\n\x0eItemGainRecord\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"d\n\x0fItemGainRecords\x12\x13\n\x0brecord_time\x18\x01 \x01(\r\x12\x17\n\x0flimit_source_id\x18\x02 \x01(\r\x12#\n\x07records\x18\x03 \x03(\x0b\x32\x12.lq.ItemGainRecord\"&\n\x04Item\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05stack\x18\x02 \x01(\r\"N\n\x03\x42\x61g\x12\x17\n\x05items\x18\x01 \x03(\x0b\x32\x08.lq.Item\x12.\n\x11\x64\x61ily_gain_record\x18\x02 \x03(\x0b\x32\x13.lq.ItemGainRecords\"b\n\tBagUpdate\x12\x1e\n\x0cupdate_items\x18\x01 \x03(\x0b\x32\x08.lq.Item\x12\x35\n\x18update_daily_gain_record\x18\x02 \x03(\x0b\x32\x13.lq.ItemGainRecords\"\'\n\nRewardSlot\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"M\n\nOpenResult\x12\x1e\n\x06reward\x18\x01 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x1f\n\x07replace\x18\x02 \x01(\x0b\x32\x0e.lq.RewardSlot\"\x97\x01\n\x10RewardPlusResult\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12/\n\x08\x65xchange\x18\x03 \x01(\x0b\x32\x1d.lq.RewardPlusResult.Exchange\x1a\x37\n\x08\x45xchange\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x10\n\x08\x65xchange\x18\x03 \x01(\r\"g\n\rExecuteReward\x12\x1e\n\x06reward\x18\x01 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x1f\n\x07replace\x18\x02 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x15\n\rreplace_count\x18\x03 \x01(\r\"\xc8\x02\n\x04Mail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\x12\x17\n\x0ftake_attachment\x18\x03 \x01(\x08\x12\r\n\x05title\x18\x04 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x05 \x01(\t\x12#\n\x0b\x61ttachments\x18\x06 \x03(\x0b\x32\x0e.lq.RewardSlot\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\r\x12\x13\n\x0b\x65xpire_time\x18\x08 \x01(\r\x12\x14\n\x0creference_id\x18\t \x01(\r\x12(\n\ntitle_i18n\x18\n \x03(\x0b\x32\x14.lq.Mail.I18nContext\x12*\n\x0c\x63ontent_i18n\x18\x0b \x03(\x0b\x32\x14.lq.Mail.I18nContext\x1a,\n\x0bI18nContext\x12\x0c\n\x04lang\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontext\x18\x02 \x01(\t\"m\n\x13\x41\x63hievementProgress\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ounter\x18\x02 \x01(\r\x12\x10\n\x08\x61\x63hieved\x18\x03 \x01(\x08\x12\x10\n\x08rewarded\x18\x04 \x01(\x08\x12\x15\n\rachieved_time\x18\x05 \x01(\r\"\x97\x04\n\x1a\x41\x63\x63ountStatisticByGameMode\x12\x0c\n\x04mode\x18\x01 \x01(\r\x12\x16\n\x0egame_count_sum\x18\x02 \x01(\r\x12\x1b\n\x13game_final_position\x18\x03 \x03(\r\x12\x11\n\tfly_count\x18\x04 \x01(\r\x12\x15\n\rgold_earn_sum\x18\x05 \x01(\x02\x12\x17\n\x0fround_count_sum\x18\x06 \x01(\r\x12\x12\n\ndadian_sum\x18\x07 \x01(\x02\x12>\n\tround_end\x18\x08 \x03(\x0b\x32+.lq.AccountStatisticByGameMode.RoundEndData\x12\x16\n\x0eming_count_sum\x18\t \x01(\r\x12\x16\n\x0eliqi_count_sum\x18\n \x01(\r\x12\x15\n\rxun_count_sum\x18\x0b \x01(\r\x12\x1a\n\x12highest_lianzhuang\x18\x0c \x01(\r\x12\x16\n\x0escore_earn_sum\x18\r \x01(\r\x12<\n\nrank_score\x18\x0e \x03(\x0b\x32(.lq.AccountStatisticByGameMode.RankScore\x1a)\n\x0cRoundEndData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0b\n\x03sum\x18\x02 \x01(\r\x1a;\n\tRankScore\x12\x0c\n\x04rank\x18\x01 \x01(\r\x12\x11\n\tscore_sum\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"4\n\x15\x41\x63\x63ountStatisticByFan\x12\x0e\n\x06\x66\x61n_id\x18\x01 \x01(\r\x12\x0b\n\x03sum\x18\x02 \x01(\r\"l\n\x12\x41\x63\x63ountFanAchieved\x12\x18\n\x10mahjong_category\x18\x01 \x01(\r\x12&\n\x03\x66\x61n\x18\x02 \x03(\x0b\x32\x19.lq.AccountStatisticByFan\x12\x14\n\x0cliujumanguan\x18\x03 \x01(\r\"\xb7\x01\n\x16\x41\x63\x63ountDetailStatistic\x12\x31\n\tgame_mode\x18\x01 \x03(\x0b\x32\x1e.lq.AccountStatisticByGameMode\x12&\n\x03\x66\x61n\x18\x02 \x03(\x0b\x32\x19.lq.AccountStatisticByFan\x12\x14\n\x0cliujumanguan\x18\x03 \x01(\r\x12,\n\x0c\x66\x61n_achieved\x18\x04 \x03(\x0b\x32\x16.lq.AccountFanAchieved\"j\n AccountDetailStatisticByCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\r\x12\x34\n\x10\x64\x65tail_statistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\"\xd1\n\n\x18\x41\x63\x63ountDetailStatisticV2\x12\x39\n\x15\x66riend_room_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x42\n\x0erank_statistic\x18\x02 \x01(\x0b\x32*.lq.AccountDetailStatisticV2.RankStatistic\x12]\n\x1c\x63ustomized_contest_statistic\x18\x03 \x01(\x0b\x32\x37.lq.AccountDetailStatisticV2.CustomizedContestStatistic\x12;\n\x17leisure_match_statistic\x18\x04 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12R\n\x19\x63hallenge_match_statistic\x18\x05 \x01(\x0b\x32/.lq.AccountDetailStatisticV2.ChallengeStatistic\x12<\n\x18\x61\x63tivity_match_statistic\x18\x06 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x36\n\x12\x61\x62_match_statistic\x18\x07 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x1a\xbd\x03\n\rRankStatistic\x12L\n\x0ftotal_statistic\x18\x01 \x01(\x0b\x32\x33.lq.AccountDetailStatisticV2.RankStatistic.RankData\x12L\n\x0fmonth_statistic\x18\x02 \x01(\x0b\x32\x33.lq.AccountDetailStatisticV2.RankStatistic.RankData\x12\x1a\n\x12month_refresh_time\x18\x03 \x01(\r\x1a\xf3\x01\n\x08RankData\x12\x37\n\x13\x61ll_level_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12Z\n\x0flevel_data_list\x18\x02 \x03(\x0b\x32\x41.lq.AccountDetailStatisticV2.RankStatistic.RankData.RankLevelData\x1aR\n\rRankLevelData\x12\x12\n\nrank_level\x18\x01 \x01(\r\x12-\n\tstatistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x1a\xa2\x01\n\x1a\x43ustomizedContestStatistic\x12\x33\n\x0ftotal_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x33\n\x0fmonth_statistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x1a\n\x12month_refresh_time\x18\x03 \x01(\r\x1a\xea\x01\n\x12\x43hallengeStatistic\x12.\n\nall_season\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12T\n\x10season_data_list\x18\x02 \x03(\x0b\x32:.lq.AccountDetailStatisticV2.ChallengeStatistic.SeasonData\x1aN\n\nSeasonData\x12\x11\n\tseason_id\x18\x01 \x01(\r\x12-\n\tstatistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\"-\n\x0e\x41\x63\x63ountShiLian\x12\x0c\n\x04step\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\"\xc2\x01\n\x10\x43lientDeviceInfo\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x10\n\x08hardware\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x12\n\nos_version\x18\x04 \x01(\t\x12\x12\n\nis_browser\x18\x05 \x01(\x08\x12\x10\n\x08software\x18\x06 \x01(\t\x12\x15\n\rsale_platform\x18\x07 \x01(\t\x12\x17\n\x0fhardware_vendor\x18\x08 \x01(\t\x12\x14\n\x0cmodel_number\x18\t \x01(\t\"6\n\x11\x43lientVersionInfo\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\x0f\n\x07package\x18\x02 \x01(\t\":\n\x0c\x41nnouncement\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"_\n\x0cTaskProgress\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ounter\x18\x02 \x01(\r\x12\x10\n\x08\x61\x63hieved\x18\x03 \x01(\x08\x12\x10\n\x08rewarded\x18\x04 \x01(\x08\x12\x0e\n\x06\x66\x61iled\x18\x05 \x01(\x08\"Z\n\nGameConfig\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\r\x12\x1a\n\x04mode\x18\x02 \x01(\x0b\x32\x0c.lq.GameMode\x12\x1e\n\x04meta\x18\x03 \x01(\x0b\x32\x10.lq.GameMetaData\"\x8d\x01\n\x12\x41\x63\x63ountActiveState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\nlogin_time\x18\x02 \x01(\r\x12\x13\n\x0blogout_time\x18\x03 \x01(\r\x12\x11\n\tis_online\x18\x04 \x01(\x08\x12\'\n\x07playing\x18\x05 \x01(\x0b\x32\x16.lq.AccountPlayingGame\"Q\n\x06\x46riend\x12 \n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12%\n\x05state\x18\x02 \x01(\x0b\x32\x16.lq.AccountActiveState\"O\n\x0cGameLiveUnit\x12\x11\n\ttimestamp\x18\x01 \x01(\r\x12\x17\n\x0f\x61\x63tion_category\x18\x02 \x01(\r\x12\x13\n\x0b\x61\x63tion_data\x18\x03 \x01(\x0c\"4\n\x0fGameLiveSegment\x12!\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x10.lq.GameLiveUnit\"=\n\x12GameLiveSegmentUri\x12\x12\n\nsegment_id\x18\x01 \x01(\r\x12\x13\n\x0bsegment_uri\x18\x02 \x01(\t\"\x8d\x01\n\x0cGameLiveHead\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12#\n\x0bgame_config\x18\x03 \x01(\x0b\x32\x0e.lq.GameConfig\x12#\n\x07players\x18\x04 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x11\n\tseat_list\x18\x05 \x03(\r\"(\n\x11GameNewRoundState\x12\x13\n\x0bseat_states\x18\x01 \x03(\r\"\x1e\n\rGameEndAction\x12\r\n\x05state\x18\x01 \x01(\r\"\x10\n\x0eGameNoopAction\"\x7f\n\x0b\x43ommentItem\x12\x12\n\ncomment_id\x18\x01 \x01(\r\x12\x11\n\ttimestamp\x18\x02 \x01(\r\x12%\n\tcommenter\x18\x03 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12\x11\n\tis_banned\x18\x05 \x01(\r\"y\n\rRollingNotice\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\x12\x17\n\x0frepeat_interval\x18\x05 \x01(\r\x12\x0c\n\x04lang\x18\x06 \x01(\t\"q\n\x0c\x42illingGoods\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\x13\n\x0bresource_id\x18\x05 \x01(\r\x12\x16\n\x0eresource_count\x18\x06 \x01(\r\"<\n\x0c\x42illShortcut\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tdealPrice\x18\x03 \x01(\r\"u\n\x0e\x42illingProduct\x12\x1f\n\x05goods\x18\x01 \x01(\x0b\x32\x10.lq.BillingGoods\x12\x15\n\rcurrency_code\x18\x02 \x01(\t\x12\x16\n\x0e\x63urrency_price\x18\x03 \x01(\r\x12\x13\n\x0bsort_weight\x18\x04 \x01(\r\"\x8c\x01\n\tCharacter\x12\x0e\n\x06\x63harid\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0b\n\x03\x65xp\x18\x03 \x01(\r\x12\x1b\n\x05views\x18\x04 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\x0c\n\x04skin\x18\x05 \x01(\r\x12\x13\n\x0bis_upgraded\x18\x06 \x01(\x08\x12\x13\n\x0b\x65xtra_emoji\x18\x07 \x03(\r\"&\n\tBuyRecord\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\xca\x01\n\x07ZHPShop\x12\r\n\x05goods\x18\x01 \x03(\r\x12\"\n\x0b\x62uy_records\x18\x02 \x03(\x0b\x32\r.lq.BuyRecord\x12.\n\x0c\x66ree_refresh\x18\x03 \x01(\x0b\x32\x18.lq.ZHPShop.RefreshCount\x12.\n\x0c\x63ost_refresh\x18\x04 \x01(\x0b\x32\x18.lq.ZHPShop.RefreshCount\x1a,\n\x0cRefreshCount\x12\r\n\x05\x63ount\x18\x01 \x01(\r\x12\r\n\x05limit\x18\x02 \x01(\r\"F\n\x0fMonthTicketInfo\x12\n\n\x02id\x18\x01 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\r\x12\x15\n\rlast_pay_time\x18\x03 \x01(\r\"c\n\x08ShopInfo\x12\x18\n\x03zhp\x18\x01 \x01(\x0b\x32\x0b.lq.ZHPShop\x12\"\n\x0b\x62uy_records\x18\x02 \x03(\x0b\x32\r.lq.BuyRecord\x12\x19\n\x11last_refresh_time\x18\x03 \x01(\r\">\n\x14\x43hangeNicknameRecord\x12\x0c\n\x04\x66rom\x18\x01 \x01(\t\x12\n\n\x02to\x18\x02 \x01(\t\x12\x0c\n\x04time\x18\x03 \x01(\r\"o\n\x0eServerSettings\x12+\n\x0fpayment_setting\x18\x03 \x01(\x0b\x32\x12.lq.PaymentSetting\x12\x30\n\x12payment_setting_v2\x18\x04 \x01(\x0b\x32\x14.lq.PaymentSettingV2\"\x83\x03\n\x10PaymentSettingV2\x12\x14\n\x0copen_payment\x18\x01 \x01(\r\x12\x42\n\x11payment_platforms\x18\x02 \x03(\x0b\x32\'.lq.PaymentSettingV2.PaymentSettingUnit\x1am\n\x0fPaymentMaintain\x12\x12\n\nstart_time\x18\x01 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\r\x12\x1a\n\x12goods_click_action\x18\x03 \x01(\r\x12\x18\n\x10goods_click_text\x18\x04 \x01(\t\x1a\xa5\x01\n\x12PaymentSettingUnit\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0f\n\x07is_show\x18\x02 \x01(\x08\x12\x1a\n\x12goods_click_action\x18\x03 \x01(\r\x12\x18\n\x10goods_click_text\x18\x04 \x01(\t\x12\x36\n\x08maintain\x18\x05 \x01(\x0b\x32$.lq.PaymentSettingV2.PaymentMaintain\"\xdf\x02\n\x0ePaymentSetting\x12\x14\n\x0copen_payment\x18\x01 \x01(\r\x12\x1e\n\x16payment_info_show_type\x18\x02 \x01(\r\x12\x14\n\x0cpayment_info\x18\x03 \x01(\t\x12-\n\x06wechat\x18\x04 \x01(\x0b\x32\x1d.lq.PaymentSetting.WechatData\x12-\n\x06\x61lipay\x18\x05 \x01(\x0b\x32\x1d.lq.PaymentSetting.AlipayData\x1a\\\n\nWechatData\x12\x16\n\x0e\x64isable_create\x18\x01 \x01(\x08\x12\x1f\n\x17payment_source_platform\x18\x02 \x01(\r\x12\x15\n\renable_credit\x18\x03 \x01(\x08\x1a\x45\n\nAlipayData\x12\x16\n\x0e\x64isable_create\x18\x01 \x01(\x08\x12\x1f\n\x17payment_source_platform\x18\x02 \x01(\r\",\n\x0e\x41\x63\x63ountSetting\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"h\n\tChestData\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x18\n\x10\x66\x61\x63\x65_black_count\x18\x04 \x01(\r\"S\n\x0b\x43hestDataV2\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x18\n\x10\x66\x61\x63\x65_black_count\x18\x03 \x01(\r\"d\n\tFaithData\x12\x10\n\x08\x66\x61ith_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x14\n\x0cmodify_count\x18\x04 \x01(\x05\"\xd9\x01\n\x15\x43ustomizedContestBase\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x14\n\x0c\x63ontest_type\x18\n \x01(\r\"C\n\x17\x43ustomizedContestExtend\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x15\n\rpublic_notice\x18\x02 \x01(\t\"\xde\x01\n\x19\x43ustomizedContestAbstract\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x15\n\rpublic_notice\x18\n \x01(\t\"\xc0\x02\n\x17\x43ustomizedContestDetail\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x11\n\trank_rule\x18\n \x01(\r\x12\x1f\n\tgame_mode\x18\x0b \x01(\x0b\x32\x0c.lq.GameMode\x12\x16\n\x0eprivate_notice\x18\x0c \x01(\t\x12\x17\n\x0fobserver_switch\x18\r \x01(\r\x12\x14\n\x0c\x65moji_switch\x18\x0e \x01(\r\"}\n\x1d\x43ustomizedContestPlayerReport\x12\x11\n\trank_rule\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12\r\n\x05point\x18\x03 \x01(\x05\x12\x12\n\ngame_ranks\x18\x04 \x03(\r\x12\x18\n\x10total_game_count\x18\x05 \x01(\r\"\xc1\x03\n\nRecordGame\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\x1e\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x0e.lq.GameConfig\x12,\n\x08\x61\x63\x63ounts\x18\x0b \x03(\x0b\x32\x1a.lq.RecordGame.AccountInfo\x12!\n\x06result\x18\x0c \x01(\x0b\x32\x11.lq.GameEndResult\x1a\x8d\x02\n\x0b\x41\x63\x63ountInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04seat\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x11\n\tavatar_id\x18\x04 \x01(\r\x12 \n\tcharacter\x18\x05 \x01(\x0b\x32\r.lq.Character\x12\r\n\x05title\x18\x06 \x01(\r\x12\x1f\n\x05level\x18\x07 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x08 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\t \x01(\r\x12\x10\n\x08verified\x18\n \x01(\r\x12\x1b\n\x05views\x18\x0b \x03(\x0b\x32\x0c.lq.ViewSlot\"\x80\x01\n\x1a\x43ustomizedContestGameStart\x12\x34\n\x07players\x18\x01 \x03(\x0b\x32#.lq.CustomizedContestGameStart.Item\x1a,\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x91\x01\n\x18\x43ustomizedContestGameEnd\x12\x32\n\x07players\x18\x01 \x03(\x0b\x32!.lq.CustomizedContestGameEnd.Item\x1a\x41\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x13\n\x0btotal_point\x18\x03 \x01(\x05\"S\n\x08\x41\x63tivity\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\x0c\n\x04type\x18\x04 \x01(\t\"4\n\x0e\x45xchangeRecord\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"^\n\x1c\x41\x63tivityAccumulatedPointData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\x05\x12\x1a\n\x12gained_reward_list\x18\x03 \x03(\r\"l\n\x15\x41\x63tivityRankPointData\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\x05\x12\x15\n\rgained_reward\x18\x03 \x01(\x08\x12\x15\n\rgainable_time\x18\x04 \x01(\r\"\xa1\x03\n\x0fGameRoundHuData\x12(\n\x05hupai\x18\x01 \x01(\x0b\x32\x19.lq.GameRoundHuData.HuPai\x12%\n\x04\x66\x61ns\x18\x02 \x03(\x0b\x32\x17.lq.GameRoundHuData.Fan\x12\r\n\x05score\x18\x03 \x01(\r\x12\x0b\n\x03xun\x18\x04 \x01(\r\x12\x10\n\x08title_id\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61n_sum\x18\x06 \x01(\r\x12\x0e\n\x06\x66u_sum\x18\x07 \x01(\r\x12\x15\n\ryakuman_count\x18\x08 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\t \x01(\r\x12\x16\n\x0ered_dora_count\x18\n \x01(\r\x12\x15\n\rli_dora_count\x18\x0b \x01(\r\x12\x13\n\x0b\x62\x61\x62\x65i_count\x18\x0c \x01(\r\x12\x18\n\x10xuan_shang_count\x18\r \x01(\r\x1a\x31\n\x05HuPai\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0c\n\x04seat\x18\x02 \x01(\r\x12\x0c\n\x04liqi\x18\x03 \x01(\r\x1a-\n\x03\x46\x61n\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x0b\n\x03\x66\x61n\x18\x03 \x01(\r\"\xb5\x01\n\x15GameRoundPlayerResult\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05hands\x18\x02 \x03(\t\x12\x0c\n\x04ming\x18\x03 \x03(\t\x12\x11\n\tliqi_type\x18\x04 \x01(\r\x12\x0f\n\x07is_fulu\x18\x05 \x01(\x08\x12\x17\n\x0fis_liujumanguan\x18\x06 \x01(\x08\x12\x13\n\x0blian_zhuang\x18\x07 \x01(\r\x12\x1f\n\x02hu\x18\x08 \x01(\x0b\x32\x13.lq.GameRoundHuData\"Y\n\x0fGameRoundPlayer\x12\r\n\x05score\x18\x01 \x01(\x05\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12)\n\x06result\x18\x03 \x01(\x0b\x32\x19.lq.GameRoundPlayerResult\"R\n\x11GameRoundSnapshot\x12\n\n\x02ju\x18\x01 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x02 \x01(\r\x12$\n\x07players\x18\x03 \x03(\x0b\x32\x13.lq.GameRoundPlayer\"\x92\x07\n\x11GameFinalSnapshot\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\r\x12\x10\n\x08\x63\x61tegory\x18\x03 \x01(\r\x12\x1a\n\x04mode\x18\x04 \x01(\x0b\x32\x0c.lq.GameMode\x12\x1e\n\x04meta\x18\x05 \x01(\x0b\x32\x10.lq.GameMetaData\x12=\n\x0f\x63\x61lculate_param\x18\x06 \x01(\x0b\x32$.lq.GameFinalSnapshot.CalculateParam\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\r\x12\x12\n\nstart_time\x18\x08 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\t \x01(\r\x12-\n\x05seats\x18\n \x03(\x0b\x32\x1e.lq.GameFinalSnapshot.GameSeat\x12%\n\x06rounds\x18\x0b \x03(\x0b\x32\x15.lq.GameRoundSnapshot\x12)\n\raccount_views\x18\x0c \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x38\n\rfinal_players\x18\r \x03(\x0b\x32!.lq.GameFinalSnapshot.FinalPlayer\x12/\n\x08\x61\x66k_info\x18\x0e \x03(\x0b\x32\x1d.lq.GameFinalSnapshot.AFKInfo\x1aS\n\x0e\x43\x61lculateParam\x12\x12\n\ninit_point\x18\x01 \x01(\r\x12\x18\n\x10jingsuanyuandian\x18\x02 \x01(\r\x12\x13\n\x0brank_points\x18\x03 \x03(\x05\x1a\x88\x01\n\x08GameSeat\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12,\n\x0fnotify_endpoint\x18\x03 \x01(\x0b\x32\x13.lq.NetworkEndpoint\x12\x16\n\x0e\x63lient_address\x18\x04 \x01(\t\x12\x14\n\x0cis_connected\x18\x05 \x01(\x08\x1a\x81\x01\n\x0b\x46inalPlayer\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x13\n\x0btotal_point\x18\x02 \x01(\x05\x12\x14\n\x0cpart_point_1\x18\x03 \x01(\x05\x12\x14\n\x0cpart_point_2\x18\x04 \x01(\x05\x12\x15\n\rgrading_score\x18\x05 \x01(\x05\x12\x0c\n\x04gold\x18\x06 \x01(\x05\x1a\x45\n\x07\x41\x46KInfo\x12\x17\n\x0f\x64\x65\x61l_tile_count\x18\x01 \x01(\r\x12\x13\n\x0bmoqie_count\x18\x02 \x01(\r\x12\x0c\n\x04seat\x18\x03 \x01(\r\"Z\n\x13RecordCollectedData\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\"\xba\x07\n\x11\x43ontestDetailRule\x12\x12\n\ninit_point\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61ndian\x18\x06 \x01(\r\x12\x11\n\tcan_jifei\x18\x07 \x01(\x08\x12\x16\n\x0etianbian_value\x18\x08 \x01(\r\x12\x16\n\x0eliqibang_value\x18\t \x01(\r\x12\x17\n\x0f\x63hangbang_value\x18\n \x01(\r\x12\x15\n\rnoting_fafu_1\x18\x0b \x01(\r\x12\x15\n\rnoting_fafu_2\x18\x0c \x01(\r\x12\x15\n\rnoting_fafu_3\x18\r \x01(\r\x12\x19\n\x11have_liujumanguan\x18\x0e \x01(\x08\x12\x1c\n\x14have_qieshangmanguan\x18\x0f \x01(\x08\x12\x16\n\x0ehave_biao_dora\x18\x10 \x01(\x08\x12\x1b\n\x13have_gang_biao_dora\x18\x11 \x01(\x08\x12\"\n\x1aming_dora_immediately_open\x18\x12 \x01(\x08\x12\x14\n\x0chave_li_dora\x18\x13 \x01(\x08\x12\x19\n\x11have_gang_li_dora\x18\x14 \x01(\x08\x12\x19\n\x11have_sifenglianda\x18\x15 \x01(\x08\x12\x18\n\x10have_sigangsanle\x18\x16 \x01(\x08\x12\x17\n\x0fhave_sijializhi\x18\x17 \x01(\x08\x12\x1b\n\x13have_jiuzhongjiupai\x18\x18 \x01(\x08\x12\x17\n\x0fhave_sanjiahele\x18\x19 \x01(\x08\x12\x14\n\x0chave_toutiao\x18\x1a \x01(\x08\x12\x1b\n\x13have_helelianzhuang\x18\x1b \x01(\x08\x12\x18\n\x10have_helezhongju\x18\x1c \x01(\x08\x12\x1e\n\x16have_tingpailianzhuang\x18\x1d \x01(\x08\x12\x1b\n\x13have_tingpaizhongju\x18\x1e \x01(\x08\x12\x11\n\thave_yifa\x18\x1f \x01(\x08\x12\x16\n\x0ehave_nanruxiru\x18  \x01(\x08\x12\x18\n\x10jingsuanyuandian\x18! \x01(\r\x12\x13\n\x0bshunweima_2\x18\" \x01(\x05\x12\x13\n\x0bshunweima_3\x18# \x01(\x05\x12\x13\n\x0bshunweima_4\x18$ \x01(\x05\x12\x14\n\x0c\x62ianjietishi\x18% \x01(\x08\x12\x10\n\x08\x61i_level\x18& \x01(\r\x12\x14\n\x0chave_zimosun\x18\' \x01(\x08\x12\x1d\n\x15\x64isable_multi_yukaman\x18( \x01(\x08\x12\x11\n\tguyi_mode\x18) \x01(\r\x12\x1a\n\x12\x64isable_leijiyiman\x18* \x01(\x08\"\xb3\x01\n\x13\x43ontestDetailRuleV2\x12(\n\tgame_rule\x18\x01 \x01(\x0b\x32\x15.lq.ContestDetailRule\x12\x35\n\nextra_rule\x18\x02 \x01(\x0b\x32!.lq.ContestDetailRuleV2.ExtraRule\x1a;\n\tExtraRule\x12\x16\n\x0erequired_level\x18\x01 \x01(\r\x12\x16\n\x0emax_game_count\x18\x02 \x01(\r\"\xab\x01\n\x0fGameRuleSetting\x12\x12\n\nround_type\x18\x01 \x01(\r\x12\x0f\n\x07shiduan\x18\x02 \x01(\x08\x12\x12\n\ndora_count\x18\x03 \x01(\r\x12\x15\n\rthinking_type\x18\x04 \x01(\r\x12\x17\n\x0fuse_detail_rule\x18\x05 \x01(\x08\x12/\n\x0e\x64\x65tail_rule_v2\x18\x06 \x01(\x0b\x32\x17.lq.ContestDetailRuleV2\"\xad\x01\n\x11RecordTingPaiInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0e\n\x06haveyi\x18\x02 \x01(\x08\x12\r\n\x05yiman\x18\x03 \x01(\x08\x12\r\n\x05\x63ount\x18\x04 \x01(\r\x12\n\n\x02\x66u\x18\x05 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\x06 \x01(\r\x12\x12\n\nyiman_zimo\x18\x07 \x01(\x08\x12\x12\n\ncount_zimo\x18\x08 \x01(\r\x12\x0f\n\x07\x66u_zimo\x18\t \x01(\r\"m\n\x16RecordNoTilePlayerInfo\x12\x0f\n\x07tingpai\x18\x03 \x01(\x08\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12$\n\x05tings\x18\x05 \x03(\x0b\x32\x15.lq.RecordTingPaiInfo\x12\x0e\n\x06liuman\x18\x06 \x01(\x08\"\xb8\x03\n\x0eRecordHuleInfo\x12\x0c\n\x04hand\x18\x01 \x03(\t\x12\x0c\n\x04ming\x18\x02 \x03(\t\x12\x0f\n\x07hu_tile\x18\x03 \x01(\t\x12\x0c\n\x04seat\x18\x04 \x01(\r\x12\x0c\n\x04zimo\x18\x05 \x01(\x08\x12\x0e\n\x06qinjia\x18\x06 \x01(\x08\x12\x0c\n\x04liqi\x18\x07 \x01(\x08\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08li_doras\x18\t \x03(\t\x12\r\n\x05yiman\x18\n \x01(\x08\x12\r\n\x05\x63ount\x18\x0b \x01(\r\x12.\n\x04\x66\x61ns\x18\x0c \x03(\x0b\x32 .lq.RecordHuleInfo.RecordFanInfo\x12\n\n\x02\x66u\x18\r \x01(\r\x12\x16\n\x0epoint_zimo_qin\x18\x0e \x01(\r\x12\x17\n\x0fpoint_zimo_xian\x18\x0f \x01(\r\x12\x10\n\x08title_id\x18\x10 \x01(\r\x12\x11\n\tpoint_sum\x18\x11 \x01(\r\x12\x0e\n\x06\x64\x61\x64ian\x18\x12 \x01(\r\x12\x14\n\x0cis_jue_zhang\x18\x13 \x01(\x08\x12\x0b\n\x03xun\x18\x14 \x01(\r\x12\x11\n\tting_type\x18\x15 \x01(\r\x1a(\n\rRecordFanInfo\x12\x0b\n\x03val\x18\x01 \x01(\r\x12\n\n\x02id\x18\x02 \x01(\r\"B\n\x0fRecordHulesInfo\x12\x0c\n\x04seat\x18\x01 \x01(\x05\x12!\n\x05hules\x18\x02 \x03(\x0b\x32\x12.lq.RecordHuleInfo\"-\n\x0fRecordLiujuInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\"U\n\x10RecordNoTileInfo\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12+\n\x07players\x18\x02 \x03(\x0b\x32\x1a.lq.RecordNoTilePlayerInfo\"r\n\x0eRecordLiqiInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\r\x12\x0c\n\x04is_w\x18\x03 \x01(\x08\x12\x14\n\x0cis_zhen_ting\x18\x04 \x01(\x08\x12\x0b\n\x03xun\x18\x05 \x01(\r\x12\x12\n\nis_success\x18\x06 \x01(\x08\"W\n\x0eRecordGangInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0b\n\x03pai\x18\x03 \x01(\t\x12\x0f\n\x07is_dora\x18\x04 \x01(\x08\x12\x0b\n\x03xun\x18\x05 \x01(\r\"S\n\x0fRecordBaBeiInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x10\n\x08is_zi_mo\x18\x02 \x01(\x08\x12\x10\n\x08is_chong\x18\x03 \x01(\x08\x12\x0e\n\x06is_bei\x18\x04 \x01(\x08\"O\n\x10RecordPeiPaiInfo\x12\x12\n\ndora_count\x18\x01 \x01(\r\x12\x14\n\x0cr_dora_count\x18\x02 \x01(\r\x12\x11\n\tbei_count\x18\x03 \x01(\r\"\xfb\x02\n\x0fRecordRoundInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63hang\x18\x02 \x01(\r\x12\n\n\x02ju\x18\x03 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\r\x12&\n\nliqi_infos\x18\x07 \x03(\x0b\x32\x12.lq.RecordLiqiInfo\x12&\n\ngang_infos\x18\x08 \x03(\x0b\x32\x12.lq.RecordGangInfo\x12*\n\x0cpeipai_infos\x18\t \x03(\x0b\x32\x14.lq.RecordPeiPaiInfo\x12(\n\x0b\x62\x61\x62\x61i_infos\x18\n \x03(\x0b\x32\x13.lq.RecordBaBeiInfo\x12\'\n\nhules_info\x18\x0b \x01(\x0b\x32\x13.lq.RecordHulesInfo\x12\'\n\nliuju_info\x18\x0c \x01(\x0b\x32\x13.lq.RecordLiujuInfo\x12*\n\x0cno_tile_info\x18\r \x01(\x0b\x32\x14.lq.RecordNoTileInfo\"@\n\x14RecordAnalysisedData\x12(\n\x0bround_infos\x18\x01 \x03(\x0b\x32\x13.lq.RecordRoundInfo\"[\n\x11ResConnectionInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x0f\x63lient_endpoint\x18\x02 \x01(\x0b\x32\x13.lq.NetworkEndpoint\"w\n\x10ReqSignupAccount\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\r\x12$\n\x06\x64\x65vice\x18\x05 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\",\n\x10ResSignupAccount\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"\xfe\x01\n\x08ReqLogin\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\x12\x0c\n\x04type\x18\t \x01(\r\x12\x0f\n\x07version\x18\n \x01(\r\"\xa9\x02\n\x08ResLogin\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x1c\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.lq.Account\x12&\n\tgame_info\x18\x04 \x01(\x0b\x32\x13.lq.GameConnectInfo\x12\x1f\n\x17has_unread_announcement\x18\x05 \x01(\x08\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x06 \x01(\t\x12\x13\n\x0bsignup_time\x18\x07 \x01(\r\x12\x19\n\x11is_id_card_authed\x18\x08 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\t \x01(\t\x12\x17\n\x0flogined_version\x18\n \x03(\r\x12\x18\n\x10rewarded_version\x18\x0b \x03(\r\"\xcb\x01\n\rReqEmailLogin\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12\x16\n\x0e\x63lient_version\x18\x06 \x01(\t\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\"3\n\x0eReqBindAccount\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"8\n\x18ReqCreatePhoneVerifyCode\x12\r\n\x05phone\x18\x01 \x01(\t\x12\r\n\x05usage\x18\x02 \x01(\r\"8\n\x18ReqCreateEmailVerifyCode\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\r\n\x05usage\x18\x02 \x01(\r\"9\n\x16ReqVerifyCodeForSecure\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\r\"H\n\x16ResVerfiyCodeForSecure\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0csecure_token\x18\x02 \x01(\t\"_\n\x12ReqBindPhoneNumber\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05phone\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1a\n\x12multi_bind_version\x18\x04 \x01(\x08\"E\n\x14ReqUnbindPhoneNumber\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05phone\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"G\n\x16ResFetchPhoneLoginBind\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bphone_login\x18\x02 \x01(\r\"+\n\x17ReqCreatePhoneLoginBind\x12\x10\n\x08password\x18\x01 \x01(\t\"=\n\x0cReqBindEmail\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"U\n\x11ReqModifyPassword\x12\x14\n\x0cnew_password\x18\x01 \x01(\t\x12\x14\n\x0cold_password\x18\x02 \x01(\t\x12\x14\n\x0csecure_token\x18\x03 \x01(\t\"8\n\rReqOauth2Auth\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03uid\x18\x03 \x01(\t\"?\n\rResOauth2Auth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\"4\n\x0eReqOauth2Check\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\"?\n\x0eResOauth2Check\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bhas_account\x18\x02 \x01(\x08\"\xb0\x01\n\x0fReqOauth2Signup\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x15\n\radvertise_str\x18\x04 \x01(\t\x12$\n\x06\x64\x65vice\x18\x05 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\"+\n\x0fResOauth2Signup\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"\xf7\x01\n\x0eReqOauth2Login\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\x12\x0f\n\x07version\x18\t \x01(\r\"$\n\x0eReqDMMPreLogin\x12\x12\n\nfinish_url\x18\x01 \x01(\t\"#\n\x0eResDMMPreLogin\x12\x11\n\tparameter\x18\x01 \x01(\t\"\x0b\n\tReqLogout\"%\n\tResLogout\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"+\n\x0bReqHeatBeat\x12\x1c\n\x14no_operation_counter\x18\x01 \x01(\r\" \n\x0cReqLoginBeat\x12\x10\n\x08\x63ontract\x18\x01 \x01(\t\"\'\n\x11ReqJoinMatchQueue\x12\x12\n\nmatch_mode\x18\x01 \x01(\r\")\n\x13ReqCancelMatchQueue\x12\x12\n\nmatch_mode\x18\x01 \x01(\r\"$\n\x0eReqAccountInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\"`\n\x0eResAccountInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1c\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.lq.Account\x12\x16\n\x04room\x18\x03 \x01(\x0b\x32\x08.lq.Room\"<\n\x11ReqCreateNickname\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x15\n\radvertise_str\x18\x02 \x01(\t\":\n\x11ReqModifyNickname\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x13\n\x0buse_item_id\x18\x02 \x01(\r\"%\n\x11ReqModifyBirthday\x12\x10\n\x08\x62irthday\x18\x01 \x01(\x05\"?\n\x0bResSelfRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"V\n\rReqCreateRoom\x12\x14\n\x0cplayer_count\x18\x01 \x01(\r\x12\x1a\n\x04mode\x18\x02 \x01(\x0b\x32\x0c.lq.GameMode\x12\x13\n\x0bpublic_live\x18\x03 \x01(\x08\"A\n\rResCreateRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"\x1e\n\x0bReqJoinRoom\x12\x0f\n\x07room_id\x18\x01 \x01(\r\"?\n\x0bResJoinRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"\x1d\n\x0cReqRoomReady\x12\r\n\x05ready\x18\x01 \x01(\x08\"#\n\x0fReqRoomDressing\x12\x10\n\x08\x64ressing\x18\x01 \x01(\x08\"\x0e\n\x0cReqRoomStart\"!\n\x0bReqRoomKick\x12\x12\n\naccount_id\x18\x01 \x01(\r\"$\n\rReqModifyRoom\x12\x13\n\x0brobot_count\x18\x01 \x01(\r\"$\n\x0fReqChangeAvatar\x12\x11\n\tavatar_id\x18\x01 \x01(\r\"-\n\x17ReqAccountStatisticInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\"\x98\x01\n\x17ResAccountStatisticInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0estatistic_data\x18\x02 \x03(\x0b\x32\x18.lq.AccountStatisticData\x12\x31\n\x0b\x64\x65tail_data\x18\x03 \x01(\x0b\x32\x1c.lq.AccountDetailStatisticV2\"\xb9\x01\n\x1bResAccountChallengeRankInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x42\n\x0bseason_info\x18\x02 \x03(\x0b\x32-.lq.ResAccountChallengeRankInfo.ChallengeRank\x1a<\n\rChallengeRank\x12\x0e\n\x06season\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12\r\n\x05level\x18\x03 \x01(\r\".\n\x17ResAccountCharacterInfo\x12\x13\n\x0bunlock_list\x18\x01 \x03(\r\"+\n\x0fReqShopPurchase\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\r\"N\n\x0fResShopPurchase\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x06update\x18\x02 \x01(\x0b\x32\x11.lq.AccountUpdate\"\"\n\rReqGameRecord\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"g\n\rResGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1c\n\x04head\x18\x03 \x01(\x0b\x32\x0e.lq.RecordGame\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x10\n\x08\x64\x61ta_url\x18\x05 \x01(\t\"?\n\x11ReqGameRecordList\x12\r\n\x05start\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x0c\n\x04type\x18\x03 \x01(\r\"g\n\x11ResGameRecordList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0btotal_count\x18\x02 \x01(\r\x12#\n\x0brecord_list\x18\x03 \x03(\x0b\x32\x0e.lq.RecordGame\"\x82\x01\n\x1aResCollectedGameRecordList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x0brecord_list\x18\x02 \x03(\x0b\x32\x17.lq.RecordCollectedData\x12\x1c\n\x14record_collect_limit\x18\x03 \x01(\r\")\n\x14ReqGameRecordsDetail\x12\x11\n\tuuid_list\x18\x01 \x03(\t\"U\n\x14ResGameRecordsDetail\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x0brecord_list\x18\x02 \x03(\x0b\x32\x0e.lq.RecordGame\"`\n\x19ReqAddCollectedGameRecord\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\"5\n\x19ResAddCollectedGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\",\n\x1cReqRemoveCollectedGameRecord\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"8\n\x1cResRemoveCollectedGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"D\n#ReqChangeCollectedGameRecordRemarks\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\"?\n#ResChangeCollectedGameRecordRemarks\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"#\n\x13ReqLevelLeaderboard\x12\x0c\n\x04type\x18\x01 \x01(\r\"\xac\x01\n\x13ResLevelLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x05items\x18\x02 \x03(\x0b\x32\x1c.lq.ResLevelLeaderboard.Item\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a;\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x1f\n\x05level\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\")\n\x17ReqChallangeLeaderboard\x12\x0e\n\x06season\x18\x01 \x01(\r\"\xb4\x01\n\x17ResChallengeLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12/\n\x05items\x18\x02 \x03(\x0b\x32 .lq.ResChallengeLeaderboard.Item\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a;\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\"@\n\x15ReqMutiChallengeLevel\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\x12\x0e\n\x06season\x18\x02 \x01(\r\"\x8b\x01\n\x15ResMutiChallengeLevel\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12-\n\x05items\x18\x02 \x03(\x0b\x32\x1e.lq.ResMutiChallengeLevel.Item\x1a)\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\",\n\x11ReqMultiAccountId\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\"U\n\x14ResMultiAccountBrief\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x07players\x18\x02 \x03(\x0b\x32\x12.lq.PlayerBaseView\"v\n\rResFriendList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1b\n\x07\x66riends\x18\x02 \x03(\x0b\x32\n.lq.Friend\x12\x18\n\x10\x66riend_max_count\x18\x03 \x01(\r\x12\x14\n\x0c\x66riend_count\x18\x04 \x01(\r\"\x9a\x01\n\x12ResFriendApplyList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x07\x61pplies\x18\x02 \x03(\x0b\x32\".lq.ResFriendApplyList.FriendApply\x1a\x35\n\x0b\x46riendApply\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\napply_time\x18\x02 \x01(\r\"#\n\x0eReqApplyFriend\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"9\n\x14ReqHandleFriendApply\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0e\n\x06method\x18\x02 \x01(\r\"$\n\x0fReqRemoveFriend\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"A\n\x19ReqSearchAccountByPattern\x12\x13\n\x0bsearch_next\x18\x01 \x01(\x08\x12\x0f\n\x07pattern\x18\x02 \x01(\t\"u\n\x19ResSearchAccountByPattern\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bis_finished\x18\x02 \x01(\x08\x12\x16\n\x0ematch_accounts\x18\x03 \x03(\r\x12\x11\n\tdecode_id\x18\x04 \x01(\r\")\n\x0eReqAccountList\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\"T\n\x10ResAccountStates\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12&\n\x06states\x18\x02 \x03(\x0b\x32\x16.lq.AccountActiveState\"*\n\x14ReqSearchAccountById\x12\x12\n\naccount_id\x18\x01 \x01(\r\"T\n\x14ResSearchAccountById\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x06player\x18\x02 \x01(\x0b\x32\x12.lq.PlayerBaseView\"<\n\nResBagInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x03\x62\x61g\x18\x02 \x01(\x0b\x32\x07.lq.Bag\" \n\rReqUseBagItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"F\n\x11ReqOpenManualItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tselect_id\x18\x03 \x01(\r\"*\n\x17ReqOpenRandomRewardItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"T\n\x17ResOpenRandomRewardItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\"\'\n\x14ReqOpenAllRewardItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"Q\n\x14ResOpenAllRewardItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\"\"\n\x0fReqComposeShard\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"$\n\x14ReqFetchAnnouncement\x12\x0c\n\x04lang\x18\x01 \x01(\t\"u\n\x0fResAnnouncement\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rannouncements\x18\x02 \x03(\x0b\x32\x10.lq.Announcement\x12\x0c\n\x04sort\x18\x03 \x03(\r\x12\x11\n\tread_list\x18\x04 \x03(\r\"@\n\x0bResMailInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x17\n\x05mails\x18\x02 \x03(\x0b\x32\x08.lq.Mail\"\x1e\n\x0bReqReadMail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\" \n\rReqDeleteMail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\"$\n\x11ReqTakeAttachment\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\"4\n ReqReceiveAchievementGroupReward\x12\x10\n\x08group_id\x18\x01 \x01(\r\"g\n ResReceiveAchievementGroupReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"5\n\x1bReqReceiveAchievementReward\x12\x16\n\x0e\x61\x63hievement_id\x18\x01 \x01(\r\"b\n\x1bResReceiveAchievementReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"\x81\x01\n\x17ResFetchAchievementRate\x12\x39\n\x04rate\x18\x01 \x03(\x0b\x32+.lq.ResFetchAchievementRate.AchievementRate\x1a+\n\x0f\x41\x63hievementRate\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04rate\x18\x02 \x01(\r\"o\n\x0eResAchievement\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\nprogresses\x18\x02 \x03(\x0b\x32\x17.lq.AchievementProgress\x12\x16\n\x0erewarded_group\x18\x03 \x03(\r\"<\n\x0cResTitleList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\ntitle_list\x18\x02 \x03(\r\"\x1c\n\x0bReqUseTitle\x12\r\n\x05title\x18\x01 \x01(\r\"\x1d\n\rReqBuyShiLian\x12\x0c\n\x04type\x18\x01 \x01(\r\"2\n\x14ReqUpdateClientValue\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"w\n\x0eResClientValue\x12\'\n\x05\x64\x61tas\x18\x01 \x03(\x0b\x32\x18.lq.ResClientValue.Value\x12\x17\n\x0frecharged_count\x18\x02 \x01(\r\x1a#\n\x05Value\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"6\n\x10ReqClientMessage\x12\x11\n\ttimestamp\x18\x01 \x01(\r\x12\x0f\n\x07message\x18\x02 \x01(\t\"(\n\x13ReqCurrentMatchInfo\x12\x11\n\tmode_list\x18\x01 \x03(\r\"\xa6\x01\n\x13ResCurrentMatchInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x39\n\x07matches\x18\x02 \x03(\x0b\x32(.lq.ResCurrentMatchInfo.CurrentMatchInfo\x1a:\n\x10\x43urrentMatchInfo\x12\x0f\n\x07mode_id\x18\x01 \x01(\r\x12\x15\n\rplaying_count\x18\x02 \x01(\r\"2\n\x0fReqUserComplain\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\".\n\x13ReqReadAnnouncement\x12\x17\n\x0f\x61nnouncement_id\x18\x01 \x01(\r\"A\n\x11ResReviveCoinInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nhas_gained\x18\x02 \x01(\x08\"\x9e\x01\n\x0cResDailyTask\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\nprogresses\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x19\n\x11has_refresh_count\x18\x03 \x01(\x08\x12\x1c\n\x14max_daily_task_count\x18\x04 \x01(\r\x12\x15\n\rrefresh_count\x18\x05 \x01(\r\"&\n\x13ReqRefreshDailyTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"j\n\x13ResRefreshDailyTask\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x08progress\x18\x02 \x01(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\"\x1e\n\x0eReqUseGiftCode\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"K\n\x0eResUseGiftCode\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07rewards\x18\x06 \x03(\x0b\x32\x0e.lq.RewardSlot\"U\n\x15ResUseSpecialGiftCode\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x07rewards\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"H\n\x14ReqSendClientMessage\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"$\n\x0fReqGameLiveInfo\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"\xaf\x01\n\x0fResGameLiveInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1a\n\x12left_start_seconds\x18\x02 \x01(\r\x12#\n\tlive_head\x18\x03 \x01(\x0b\x32\x10.lq.GameLiveHead\x12(\n\x08segments\x18\x04 \x03(\x0b\x32\x16.lq.GameLiveSegmentUri\x12\x17\n\x0fnow_millisecond\x18\x05 \x01(\r\"D\n\x16ReqGameLiveLeftSegment\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x17\n\x0flast_segment_id\x18\x02 \x01(\r\"\xaa\x01\n\x16ResGameLiveLeftSegment\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nlive_state\x18\x02 \x01(\r\x12(\n\x08segments\x18\x04 \x03(\x0b\x32\x16.lq.GameLiveSegmentUri\x12\x17\n\x0fnow_millisecond\x18\x05 \x01(\r\x12\x1f\n\x17segment_end_millisecond\x18\x06 \x01(\r\"$\n\x0fReqGameLiveList\x12\x11\n\tfilter_id\x18\x01 \x01(\r\"P\n\x0fResGameLiveList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\tlive_list\x18\x02 \x03(\x0b\x32\x10.lq.GameLiveHead\"D\n\x11ResCommentSetting\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rcomment_allow\x18\x02 \x01(\r\"0\n\x17ReqUpdateCommentSetting\x12\x15\n\rcomment_allow\x18\x01 \x01(\r\"(\n\x13ReqFetchCommentList\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"u\n\x13ResFetchCommentList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rcomment_allow\x18\x02 \x01(\r\x12\x17\n\x0f\x63omment_id_list\x18\x03 \x03(\r\x12\x14\n\x0clast_read_id\x18\x04 \x01(\r\"D\n\x16ReqFetchCommentContent\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x17\n\x0f\x63omment_id_list\x18\x02 \x03(\r\"U\n\x16ResFetchCommentContent\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x08\x63omments\x18\x02 \x03(\x0b\x32\x0f.lq.CommentItem\"5\n\x0fReqLeaveComment\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\":\n\x10ReqDeleteComment\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65lete_list\x18\x02 \x03(\r\"\'\n\x14ReqUpdateReadComment\x12\x0f\n\x07read_id\x18\x01 \x01(\r\"5\n\x10ReqRollingNotice\x12!\n\x06notice\x18\x01 \x03(\x0b\x32\x11.lq.RollingNotice\"$\n\rResServerTime\x12\x13\n\x0bserver_time\x18\x01 \x01(\r\"0\n\x1aReqPlatformBillingProducts\x12\x12\n\nshelves_id\x18\x01 \x01(\r\"\\\n\x1aResPlatformBillingProducts\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\x08products\x18\x02 \x03(\x0b\x32\x12.lq.BillingProduct\"l\n\x15ReqCreateBillingOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x18\n\x10payment_platform\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\x12\x12\n\naccount_id\x18\x04 \x01(\r\"C\n\x15ResCreateBillingOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"T\n\x17ReqSolveGooglePlayOrder\x12\x1b\n\x13inapp_purchase_data\x18\x02 \x01(\t\x12\x1c\n\x14inapp_data_signature\x18\x03 \x01(\t\"h\n\x19ReqSolveGooglePlayOrderV3\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x16\n\x0etransaction_id\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\r\",\n\x18ReqCancelGooglePlayOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\"k\n\x1aReqCreateWechatNativeOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\naccount_ip\x18\x04 \x01(\t\"_\n\x1aResCreateWechatNativeOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rqrcode_buffer\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\"h\n\x17ReqCreateWechatAppOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\naccount_ip\x18\x04 \x01(\t\"\x91\x02\n\x17ResCreateWechatAppOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12M\n\x15\x63\x61ll_wechat_app_param\x18\x02 \x01(\x0b\x32..lq.ResCreateWechatAppOrder.CallWechatAppParam\x1a\x8c\x01\n\x12\x43\x61llWechatAppParam\x12\r\n\x05\x61ppid\x18\x01 \x01(\t\x12\x11\n\tpartnerid\x18\x02 \x01(\t\x12\x10\n\x08prepayid\x18\x03 \x01(\t\x12\x0f\n\x07package\x18\x04 \x01(\t\x12\x10\n\x08noncestr\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04sign\x18\x07 \x01(\t\"\x80\x01\n\x14ReqCreateAlipayOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x19\n\x11\x61lipay_trade_type\x18\x04 \x01(\t\x12\x12\n\nreturn_url\x18\x05 \x01(\t\"D\n\x14ResCreateAlipayOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nalipay_url\x18\x02 \x01(\t\"U\n\x18ReqCreateAlipayScanOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"n\n\x18ResCreateAlipayScanOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rqrcode_buffer\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\x12\x0f\n\x07qr_code\x18\x04 \x01(\t\"T\n\x17ReqCreateAlipayAppOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"G\n\x17ResCreateAlipayAppOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nalipay_url\x18\x02 \x01(\t\"\x81\x01\n\x1aReqCreateJPCreditCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"H\n\x1aResCreateJPCreditCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateJPPaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateJPPaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"y\n\x12ReqCreateJPAuOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"@\n\x12ResCreateJPAuOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateJPDocomoOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateJPDocomoOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x7f\n\x18ReqCreateJPWebMoneyOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"F\n\x18ResCreateJPWebMoneyOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x7f\n\x18ReqCreateJPSoftbankOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"F\n\x18ResCreateJPSoftbankOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"e\n\x14ReqCreateYostarOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\norder_type\x18\x04 \x01(\r\"B\n\x14ResCreateYostarOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateENPaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateENPaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"z\n\x13ReqCreateENJCBOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"A\n\x13ResCreateENJCBOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x81\x01\n\x1aReqCreateENMasterCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"H\n\x1aResCreateENMasterCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"{\n\x14ReqCreateENVisaOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"B\n\x14ResCreateENVisaOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateENAlipayOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateENAlipayOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"N\n\x11ReqCreateDMMOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\"\xbb\x01\n\x11ResCreateDmmOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x16\n\x0etransaction_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64mm_user_id\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x06 \x01(\t\x12\x14\n\x0crequest_time\x18\t \x01(\t\x12\x12\n\ndmm_app_id\x18\n \x01(\t\"d\n\x11ReqCreateIAPOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\t\"?\n\x11ResCreateIAPOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"m\n\x17ReqVerificationIAPOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x16\n\x0etransaction_id\x18\x02 \x01(\t\x12\x14\n\x0creceipt_data\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\r\"3\n\x17ResVerificationIAPOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"t\n\x13ReqCreateSteamOrder\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\x12\x10\n\x08goods_id\x18\x04 \x01(\r\x12\x10\n\x08steam_id\x18\x05 \x01(\t\"\\\n\x13ResCreateSteamOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x19\n\x11platform_order_id\x18\x03 \x01(\t\";\n\x13ReqVerifySteamOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\"Q\n\x14ReqCreateMyCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"U\n\x14ResCreateMyCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tauth_code\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\"<\n\x14ReqVerifyMyCardOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\"Q\n\x14ReqCreatePaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"O\n\x14ResCreatePaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"i\n\x14ReqCreateXsollaOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x16\n\x0epayment_method\x18\x04 \x01(\r\"O\n\x14ResCreateXsollaOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"C\n\x0cReqOpenChest\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x12\n\nuse_ticket\x18\x03 \x01(\x08\"\xee\x01\n\x0cResOpenChest\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\x12\x18\n\x10total_open_count\x18\x03 \x01(\r\x12\x13\n\x0b\x66\x61ith_count\x18\x04 \x01(\r\x12@\n\x10\x63hest_replace_up\x18\x05 \x03(\x0b\x32&.lq.ResOpenChest.ChestReplaceCountData\x1a\x32\n\x15\x43hestReplaceCountData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"6\n\x13ReqBuyFromChestShop\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"m\n\x13ResBuyFromChestShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08\x63hest_id\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x13\n\x0b\x66\x61ith_count\x18\x04 \x01(\r\"D\n\x12ResDailySignInInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0csign_in_days\x18\x02 \x01(\r\"*\n\x13ReqDoActivitySignIn\x12\x13\n\x0b\x61\x63tivity_id\x18\x02 \x01(\r\"\xad\x01\n\x13ResDoActivitySignIn\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x07rewards\x18\x02 \x03(\x0b\x32\".lq.ResDoActivitySignIn.RewardData\x12\x15\n\rsign_in_count\x18\x03 \x01(\r\x1a\x30\n\nRewardData\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\xf7\x01\n\x10ResCharacterInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\ncharacters\x18\x02 \x03(\x0b\x32\r.lq.Character\x12\r\n\x05skins\x18\x03 \x03(\r\x12\x19\n\x11main_character_id\x18\x04 \x01(\r\x12\x17\n\x0fsend_gift_count\x18\x05 \x01(\r\x12\x17\n\x0fsend_gift_limit\x18\x06 \x01(\r\x12\x18\n\x10\x66inished_endings\x18\x07 \x03(\r\x12\x18\n\x10rewarded_endings\x18\x08 \x03(\r\x12\x16\n\x0e\x63haracter_sort\x18\t \x03(\r\"&\n\x16ReqUpdateCharacterSort\x12\x0c\n\x04sort\x18\x01 \x03(\r\".\n\x16ReqChangeMainCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\"<\n\x16ReqChangeCharacterSkin\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x0c\n\x04skin\x18\x02 \x01(\r\"M\n\x16ReqChangeCharacterView\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x0c\n\x04slot\x18\x02 \x01(\r\x12\x0f\n\x07item_id\x18\x03 \x01(\r\"\x86\x01\n\x16ReqSendGiftToCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12.\n\x05gifts\x18\x02 \x03(\x0b\x32\x1f.lq.ReqSendGiftToCharacter.Gift\x1a&\n\x04Gift\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"N\n\x16ResSendGiftToCharacter\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0b\n\x03\x65xp\x18\x03 \x01(\r\"Z\n\x0bReqSellItem\x12#\n\x05sells\x18\x01 \x03(\x0b\x32\x14.lq.ReqSellItem.Item\x1a&\n\x04Item\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"u\n\rResCommonView\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12%\n\x05slots\x18\x02 \x03(\x0b\x32\x16.lq.ResCommonView.Slot\x1a#\n\x04Slot\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"2\n\x13ReqChangeCommonView\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"U\n\x12ReqSaveCommonViews\x12\x1b\n\x05views\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\x12\n\nsave_index\x18\x02 \x01(\r\x12\x0e\n\x06is_use\x18\x03 \x01(\r\"\x1f\n\x0eReqCommonViews\x12\r\n\x05index\x18\x01 \x01(\r\"-\n\x0eResCommonViews\x12\x1b\n\x05views\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\"\x9c\x01\n\x11ResAllcommonViews\x12*\n\x05views\x18\x01 \x03(\x0b\x32\x1b.lq.ResAllcommonViews.Views\x12\x0b\n\x03use\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\x1a\x34\n\x05Views\x12\x1c\n\x06values\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\r\n\x05index\x18\x02 \x01(\r\"!\n\x10ReqUseCommonView\x12\r\n\x05index\x18\x03 \x01(\r\"+\n\x13ReqUpgradeCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\"Q\n\x13ResUpgradeCharacter\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12 \n\tcharacter\x18\x02 \x01(\x0b\x32\r.lq.Character\"N\n\x11ReqFinishedEnding\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x10\n\x08story_id\x18\x02 \x01(\r\x12\x11\n\tending_id\x18\x03 \x01(\r\"\x1f\n\x0cReqGMCommand\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"H\n\x0bResShopInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\tshop_info\x18\x02 \x01(\x0b\x32\x0c.lq.ShopInfo\"o\n\x0eReqBuyFromShop\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12(\n\x0e\x62ill_short_cut\x18\x03 \x03(\x0b\x32\x10.lq.BillShortcut\x12\x12\n\ndeal_price\x18\x04 \x01(\r\"K\n\x0eResBuyFromShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07rewards\x18\x02 \x03(\x0b\x32\x0e.lq.RewardSlot\"0\n\rReqBuyFromZHP\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"&\n\x11ReqPayMonthTicket\x12\x11\n\tticket_id\x18\x01 \x01(\r\"Z\n\x11ResPayMonthTicket\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bresource_id\x18\x02 \x01(\r\x12\x16\n\x0eresource_count\x18\x03 \x01(\r\"<\n\x0eReqReshZHPShop\x12\x14\n\x0c\x66ree_refresh\x18\x01 \x01(\r\x12\x14\n\x0c\x63ost_refresh\x18\x02 \x01(\r\"G\n\x11ResRefreshZHPShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x18\n\x03zhp\x18\x02 \x01(\x0b\x32\x0b.lq.ZHPShop\"D\n\x12ResMonthTicketInfo\x12.\n\x11month_ticket_info\x18\x01 \x03(\x0b\x32\x13.lq.MonthTicketInfo\"0\n\x13ReqExchangeCurrency\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"9\n\x11ResServerSettings\x12$\n\x08settings\x18\x01 \x01(\x0b\x32\x12.lq.ServerSettings\"T\n\x12ResAccountSettings\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\x08settings\x18\x02 \x03(\x0b\x32\x12.lq.AccountSetting\"?\n\x18ReqUpdateAccountSettings\x12#\n\x07setting\x18\x01 \x01(\x0b\x32\x12.lq.AccountSetting\"+\n\x12ResModNicknameTime\x12\x15\n\rlast_mod_time\x18\x01 \x01(\r\"\x98\x01\n\x07ResMisc\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x0erecharged_list\x18\x02 \x03(\r\x12)\n\x06\x66\x61iths\x18\x03 \x03(\x0b\x32\x19.lq.ResMisc.MiscFaithData\x1a\x30\n\rMiscFaithData\x12\x10\n\x08\x66\x61ith_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\'\n\x12ReqModifySignature\x12\x11\n\tsignature\x18\x01 \x01(\t\"M\n\rResIDCardInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tis_authed\x18\x02 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\"8\n\x13ReqUpdateIDCardInfo\x12\x10\n\x08\x66ullname\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61rd_no\x18\x02 \x01(\t\"C\n\x0cResVipReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x19\n\x11gained_vip_levels\x18\x02 \x03(\r\"%\n\x10ReqGainVipReward\x12\x11\n\tvip_level\x18\x01 \x01(\r\"=\n\x1dReqFetchCustomizedContestList\x12\r\n\x05start\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\x9a\x01\n\x1dResFetchCustomizedContestList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x08\x63ontests\x18\x02 \x03(\x0b\x32\x19.lq.CustomizedContestBase\x12\x32\n\x0f\x66ollow_contests\x18\x03 \x03(\x0b\x32\x19.lq.CustomizedContestBase\"7\n#ReqFetchCustomizedContestExtendInfo\x12\x10\n\x08uid_list\x18\x01 \x03(\r\"q\n#ResFetchCustomizedContestExtendInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0b\x65xtend_list\x18\x02 \x03(\x0b\x32\x1b.lq.CustomizedContestExtend\"6\n!ReqFetchCustomizedContestAuthInfo\x12\x11\n\tunique_id\x18\x01 \x01(\r\"U\n!ResFetchCustomizedContestAuthInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x0eobserver_level\x18\x02 \x01(\r\".\n\x19ReqEnterCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"\xb6\x01\n\x19ResEnterCustomizedContest\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0b\x64\x65tail_info\x18\x02 \x01(\x0b\x32\x1b.lq.CustomizedContestDetail\x12\x38\n\rplayer_report\x18\x03 \x01(\x0b\x32!.lq.CustomizedContestPlayerReport\x12\x13\n\x0bis_followed\x18\x04 \x01(\x08\"8\n#ReqFetchCustomizedContestOnlineInfo\x12\x11\n\tunique_id\x18\x01 \x01(\r\"V\n#ResFetchCustomizedContestOnlineInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\ronline_player\x18\x02 \x01(\r\":\n$ReqFetchCustomizedContestByContestId\x12\x12\n\ncontest_id\x18\x01 \x01(\r\"u\n$ResFetchCustomizedContestByContestId\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x0c\x63ontest_info\x18\x02 \x01(\x0b\x32\x1d.lq.CustomizedContestAbstract\".\n\x19ReqStartCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"5\n ReqJoinCustomizedContestChatRoom\x12\x11\n\tunique_id\x18\x01 \x01(\r\"R\n ResJoinCustomizedContestChatRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0c\x63hat_history\x18\x02 \x03(\x0c\"$\n\x11ReqSayChatMessage\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\":\n%ReqFetchCustomizedContestGameLiveList\x12\x11\n\tunique_id\x18\x01 \x01(\r\"f\n%ResFetchCustomizedContestGameLiveList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\tlive_list\x18\x02 \x03(\x0b\x32\x10.lq.GameLiveHead\"M\n$ReqFetchCustomizedContestGameRecords\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\nlast_index\x18\x02 \x01(\r\"y\n$ResFetchCustomizedContestGameRecords\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nnext_index\x18\x02 \x01(\r\x12#\n\x0brecord_list\x18\x03 \x03(\x0b\x32\x0e.lq.RecordGame\"/\n\x1aReqTargetCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"M\n\x0fResActivityList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12 \n\nactivities\x18\x02 \x03(\x0b\x32\x0c.lq.Activity\"\xed\x07\n\x16ResAccountActivityData\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x10\x65xchange_records\x18\x02 \x03(\x0b\x32\x12.lq.ExchangeRecord\x12,\n\x12task_progress_list\x18\x03 \x03(\x0b\x32\x10.lq.TaskProgress\x12@\n\x16\x61\x63\x63umulated_point_list\x18\x04 \x03(\x0b\x32 .lq.ActivityAccumulatedPointData\x12\x31\n\x0erank_data_list\x18\x05 \x03(\x0b\x32\x19.lq.ActivityRankPointData\x12\x31\n\x17\x66lip_task_progress_list\x18\x06 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x43\n\x0csign_in_data\x18\x07 \x03(\x0b\x32-.lq.ResAccountActivityData.ActivitySignInData\x12\x44\n\x0crichman_data\x18\x08 \x03(\x0b\x32..lq.ResAccountActivityData.ActivityRichmanData\x12\x33\n\x19period_task_progress_list\x18\t \x03(\x0b\x32\x10.lq.TaskProgress\x12\x33\n\x19random_task_progress_list\x18\n \x03(\x0b\x32\x10.lq.TaskProgress\x12=\n\rchest_up_data\x18\x0b \x03(\x0b\x32&.lq.ResAccountActivityData.ChestUpData\x1a[\n\x12\x41\x63tivitySignInData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x15\n\rsign_in_count\x18\x02 \x01(\r\x12\x19\n\x11last_sign_in_time\x18\x03 \x01(\r\x1a\x38\n\x08\x42uffData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0e\n\x06remain\x18\x02 \x01(\r\x12\x0e\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\r\x1a\xbf\x01\n\x13\x41\x63tivityRichmanData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x10\n\x08location\x18\x02 \x01(\r\x12\x16\n\x0e\x66inished_count\x18\x03 \x01(\r\x12\x16\n\x0e\x63hest_position\x18\x04 \x01(\r\x12\x11\n\tbank_save\x18\x05 \x01(\r\x12\x0b\n\x03\x65xp\x18\x06 \x01(\r\x12\x31\n\x04\x62uff\x18\x07 \x03(\x0b\x32#.lq.ResAccountActivityData.BuffData\x1a(\n\x0b\x43hestUpData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"=\n\x17ReqExchangeActivityItem\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"^\n\x17ResExchangeActivityItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"*\n\x17ReqCompleteActivityTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"-\n\x1aReqReceiveActivityFlipTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"E\n\x1aResReceiveActivityFlipTask\x12\r\n\x05\x63ount\x18\x01 \x01(\r\x12\x18\n\x05\x65rror\x18\x02 \x01(\x0b\x32\t.lq.Error\"/\n\x18ReqFetchActivityFlipInfo\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"T\n\x18ResFetchActivityFlipInfo\x12\x0f\n\x07rewards\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\"O\n%ReqGainAccumulatedPointActivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x11\n\treward_id\x18\x02 \x01(\r\"N\n\x1fReqGainMultiPointActivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x16\n\x0ereward_id_list\x18\x02 \x03(\r\"6\n\x1cReqFetchRankPointLeaderboard\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\"\xe4\x01\n\x1cResFetchRankPointLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x34\n\x05items\x18\x02 \x03(\x0b\x32%.lq.ResFetchRankPointLeaderboard.Item\x12\x19\n\x11last_refresh_time\x18\x03 \x01(\r\x1aY\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12 \n\x04view\x18\x03 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\r\n\x05point\x18\x04 \x01(\r\"E\n\x16ReqGainRankPointReward\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\x13\n\x0b\x61\x63tivity_id\x18\x02 \x01(\r\")\n\x12ReqRichmanNextMove\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x94\x04\n\x12ResRichmanNextMove\x12.\n\x05paths\x18\x01 \x03(\x0b\x32\x1f.lq.ResRichmanNextMove.PathData\x12\x0c\n\x04\x64ice\x18\x02 \x01(\r\x12\x10\n\x08location\x18\x03 \x01(\r\x12\x16\n\x0e\x66inished_count\x18\x04 \x01(\r\x12\x0c\n\x04step\x18\x05 \x01(\r\x12-\n\x04\x62uff\x18\x06 \x03(\x0b\x32\x1f.lq.ResRichmanNextMove.BuffData\x12\x11\n\tbank_save\x18\x07 \x01(\r\x12\x16\n\x0e\x63hest_position\x18\x08 \x01(\r\x12\x0b\n\x03\x65xp\x18\t \x01(\r\x12\x15\n\rbank_save_add\x18\n \x01(\r\x12\x18\n\x05\x65rror\x18\x0b \x01(\x0b\x32\t.lq.Error\x1aT\n\nRewardData\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x14\n\x0corigin_count\x18\x03 \x01(\r\x12\x0c\n\x04type\x18\x05 \x01(\r\x1a`\n\x08PathData\x12\x10\n\x08location\x18\x01 \x01(\r\x12\x32\n\x07rewards\x18\x02 \x03(\x0b\x32!.lq.ResRichmanNextMove.RewardData\x12\x0e\n\x06\x65vents\x18\x03 \x03(\r\x1a\x38\n\x08\x42uffData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0e\n\x06remain\x18\x02 \x01(\r\x12\x0e\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\r\":\n\x15ReqRichmanSpecialMove\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x0c\n\x04step\x18\x02 \x01(\r\"*\n\x13ReqRichmanChestInfo\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x87\x01\n\x13ResRichmanChestInfo\x12/\n\x05items\x18\x01 \x03(\x0b\x32 .lq.ResRichmanChestInfo.ItemData\x12\x18\n\x05\x65rror\x18\x02 \x01(\x0b\x32\t.lq.Error\x1a%\n\x08ItemData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"-\n\x18ReqCreateGameObserveAuth\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"U\n\x18ResCreateGameObserveAuth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\"*\n\x19ReqRefreshGameObserveAuth\x12\r\n\x05token\x18\x01 \x01(\t\"B\n\x19ResRefreshGameObserveAuth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0b\n\x03ttl\x18\x02 \x01(\r\"\x98\x01\n\x0fResActivityBuff\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x37\n\tbuff_list\x18\x02 \x03(\x0b\x32$.lq.ResActivityBuff.ActivityBuffData\x1a\x32\n\x10\x41\x63tivityBuffData\x12\x0f\n\x07\x62uff_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\")\n\x16ReqUpgradeActivityBuff\x12\x0f\n\x07\x62uff_id\x18\x01 \x01(\r\"\xa6\x01\n\x13ResUpgradeChallenge\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\"\xa6\x01\n\x13ResRefreshChallenge\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\"\xc1\x01\n\x15ResFetchChallengeInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\x12\x17\n\x0frewarded_season\x18\x07 \x03(\r\"0\n\x1dReqForceCompleteChallengeTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"\xff\x01\n\x0fResFetchABMatch\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08match_id\x18\x02 \x01(\r\x12\x13\n\x0bmatch_count\x18\x03 \x01(\r\x12\x14\n\x0c\x62uy_in_count\x18\x04 \x01(\r\x12\r\n\x05point\x18\x05 \x01(\r\x12\x10\n\x08rewarded\x18\x06 \x01(\x08\x12\x37\n\x0fmatch_max_point\x18\x07 \x03(\x0b\x32\x1e.lq.ResFetchABMatch.MatchPoint\x12\x0c\n\x04quit\x18\x08 \x01(\x08\x1a-\n\nMatchPoint\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\")\n\x14ReqStartUnifiedMatch\x12\x11\n\tmatch_sid\x18\x01 \x01(\t\"*\n\x15ReqCancelUnifiedMatch\x12\x11\n\tmatch_sid\x18\x01 \x01(\t\"\xba\x01\n\x16ResChallengeSeasonInfo\x12G\n\x15\x63hallenge_season_list\x18\x01 \x03(\x0b\x32(.lq.ResChallengeSeasonInfo.ChallengeInfo\x1aW\n\rChallengeInfo\x12\x11\n\tseason_id\x18\x01 \x01(\r\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\r\n\x05state\x18\x04 \x01(\r\"2\n\x1dReqReceiveChallengeRankReward\x12\x11\n\tseason_id\x18\x01 \x01(\r\"\x88\x01\n\x1dResReceiveChallengeRankReward\x12\x39\n\x07rewards\x18\x01 \x03(\x0b\x32(.lq.ResReceiveChallengeRankReward.Reward\x1a,\n\x06Reward\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"#\n\x0fReqBuyInABMatch\x12\x10\n\x08match_id\x18\x01 \x01(\r\"\'\n\x10ReqGamePointRank\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x9b\x01\n\x10ResGamePointRank\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x04rank\x18\x02 \x03(\x0b\x32\x1d.lq.ResGamePointRank.RankInfo\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a-\n\x08RankInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"H\n\x19ResFetchSelfGamePointRank\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tself_rate\x18\x02 \x01(\r\"\x0f\n\rActionMJStart\"A\n\x13NewRoundOpenedTiles\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05tiles\x18\x02 \x03(\t\x12\r\n\x05\x63ount\x18\x03 \x03(\r\"F\n\x08MuyuInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tcount_max\x18\x03 \x01(\r\x12\n\n\x02id\x18\x04 \x01(\r\"\xf9\x02\n\x0e\x41\x63tionNewRound\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x0c\n\x04\x64ora\x18\x05 \x01(\t\x12\x0e\n\x06scores\x18\x06 \x03(\x05\x12,\n\toperation\x18\x07 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x10\n\x08liqibang\x18\x08 \x01(\r\x12)\n\ttingpais0\x18\t \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\"\n\ttingpais1\x18\n \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\n\n\x02\x61l\x18\x0b \x01(\x08\x12\x0b\n\x03md5\x18\x0c \x01(\t\x12\x17\n\x0fleft_tile_count\x18\r \x01(\r\x12\r\n\x05\x64oras\x18\x0e \x03(\t\x12&\n\x05opens\x18\x0f \x03(\x0b\x32\x17.lq.NewRoundOpenedTiles\x12\x1a\n\x04muyu\x18\x10 \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xf9\x03\n\x0eRecordNewRound\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\x0c\n\x04\x64ora\x18\x04 \x01(\t\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x10\n\x08liqibang\x18\x06 \x01(\r\x12\x0e\n\x06tiles0\x18\x07 \x03(\t\x12\x0e\n\x06tiles1\x18\x08 \x03(\t\x12\x0e\n\x06tiles2\x18\t \x03(\t\x12\x0e\n\x06tiles3\x18\n \x03(\t\x12+\n\x07tingpai\x18\x0b \x03(\x0b\x32\x1a.lq.RecordNewRound.TingPai\x12,\n\toperation\x18\x0c \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x0b\n\x03md5\x18\r \x01(\t\x12\x0f\n\x07paishan\x18\x0e \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x0f \x01(\r\x12\r\n\x05\x64oras\x18\x10 \x03(\t\x12&\n\x05opens\x18\x11 \x03(\x0b\x32\x17.lq.NewRoundOpenedTiles\x12\x1a\n\x04muyu\x18\x12 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12-\n\noperations\x18\x13 \x03(\x0b\x32\x19.lq.OptionalOperationList\x1a;\n\x07TingPai\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\ttingpais1\x18\x02 \x03(\x0b\x32\x0f.lq.TingPaiInfo\"\x99\x03\n\x0cGameSnapshot\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\x14\n\x0cindex_player\x18\x04 \x01(\r\x12\x17\n\x0fleft_tile_count\x18\x05 \x01(\r\x12\r\n\x05hands\x18\x06 \x03(\t\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x10\n\x08liqibang\x18\x08 \x01(\r\x12\x30\n\x07players\x18\t \x03(\x0b\x32\x1f.lq.GameSnapshot.PlayerSnapshot\x12\x10\n\x08zhenting\x18\n \x01(\x08\x1a\xbd\x01\n\x0ePlayerSnapshot\x12\r\n\x05score\x18\x01 \x01(\x05\x12\x14\n\x0cliqiposition\x18\x02 \x01(\x05\x12\x0f\n\x07tilenum\x18\x03 \x01(\r\x12\x0e\n\x06qipais\x18\x04 \x03(\t\x12\x33\n\x05mings\x18\x05 \x03(\x0b\x32$.lq.GameSnapshot.PlayerSnapshot.Fulu\x1a\x30\n\x04\x46ulu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x03(\t\x12\x0c\n\x04\x66rom\x18\x03 \x03(\r\";\n\x0f\x41\x63tionPrototype\x12\x0c\n\x04step\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"$\n\x11GameDetailRecords\x12\x0f\n\x07records\x18\x01 \x03(\x0c\"h\n\x11OptionalOperation\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x13\n\x0b\x63ombination\x18\x02 \x03(\t\x12\x14\n\x0c\x63hange_tiles\x18\x03 \x03(\t\x12\x1a\n\x12\x63hange_tile_states\x18\x04 \x03(\x05\"z\n\x15OptionalOperationList\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12-\n\x0eoperation_list\x18\x02 \x03(\x0b\x32\x15.lq.OptionalOperation\x12\x10\n\x08time_add\x18\x04 \x01(\r\x12\x12\n\ntime_fixed\x18\x05 \x01(\r\"L\n\x0bLiQiSuccess\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\x05\x12\x10\n\x08liqibang\x18\x03 \x01(\r\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\"0\n\x07\x46\x61nInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03val\x18\x02 \x01(\r\x12\n\n\x02id\x18\x03 \x01(\r\"\xe0\x02\n\x08HuleInfo\x12\x0c\n\x04hand\x18\x01 \x03(\t\x12\x0c\n\x04ming\x18\x02 \x03(\t\x12\x0f\n\x07hu_tile\x18\x03 \x01(\t\x12\x0c\n\x04seat\x18\x04 \x01(\r\x12\x0c\n\x04zimo\x18\x05 \x01(\x08\x12\x0e\n\x06qinjia\x18\x06 \x01(\x08\x12\x0c\n\x04liqi\x18\x07 \x01(\x08\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08li_doras\x18\t \x03(\t\x12\r\n\x05yiman\x18\n \x01(\x08\x12\r\n\x05\x63ount\x18\x0b \x01(\r\x12\x19\n\x04\x66\x61ns\x18\x0c \x03(\x0b\x32\x0b.lq.FanInfo\x12\n\n\x02\x66u\x18\r \x01(\r\x12\r\n\x05title\x18\x0e \x01(\t\x12\x12\n\npoint_rong\x18\x0f \x01(\r\x12\x16\n\x0epoint_zimo_qin\x18\x10 \x01(\r\x12\x17\n\x0fpoint_zimo_xian\x18\x11 \x01(\r\x12\x10\n\x08title_id\x18\x12 \x01(\r\x12\x11\n\tpoint_sum\x18\x13 \x01(\r\x12\x0e\n\x06\x64\x61\x64ian\x18\x14 \x01(\r\"\xa7\x01\n\x0bTingPaiInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0e\n\x06haveyi\x18\x02 \x01(\x08\x12\r\n\x05yiman\x18\x03 \x01(\x08\x12\r\n\x05\x63ount\x18\x04 \x01(\r\x12\n\n\x02\x66u\x18\x05 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\x06 \x01(\r\x12\x12\n\nyiman_zimo\x18\x07 \x01(\x08\x12\x12\n\ncount_zimo\x18\x08 \x01(\r\x12\x0f\n\x07\x66u_zimo\x18\t \x01(\r\"T\n\x12TingPaiDiscardInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x10\n\x08zhenting\x18\x02 \x01(\x08\x12\x1e\n\x05infos\x18\x03 \x03(\x0b\x32\x0f.lq.TingPaiInfo\"\x19\n\x07GameEnd\x12\x0e\n\x06scores\x18\x01 \x03(\x05\"\x89\x02\n\x10\x41\x63tionChangeTile\x12\x10\n\x08in_tiles\x18\x01 \x03(\t\x12\x16\n\x0ein_tile_states\x18\x02 \x03(\x05\x12\x11\n\tout_tiles\x18\x03 \x03(\t\x12\x17\n\x0fout_tile_states\x18\x04 \x03(\x05\x12\r\n\x05\x64oras\x18\x05 \x03(\t\x12)\n\ttingpais0\x18\x06 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\"\n\ttingpais1\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0b\x63hange_type\x18\t \x01(\r\"\xf0\x02\n\x10RecordChangeTile\x12\r\n\x05\x64oras\x18\x01 \x03(\t\x12-\n\x07tingpai\x18\x02 \x03(\x0b\x32\x1c.lq.RecordChangeTile.TingPai\x12:\n\x11\x63hange_tile_infos\x18\x03 \x03(\x0b\x32\x1f.lq.RecordChangeTile.ChangeTile\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0b\x63hange_type\x18\x05 \x01(\r\x1a;\n\x07TingPai\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\ttingpais1\x18\x02 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x1a\x62\n\nChangeTile\x12\x10\n\x08in_tiles\x18\x01 \x03(\t\x12\x16\n\x0ein_tile_states\x18\x02 \x03(\x05\x12\x11\n\tout_tiles\x18\x03 \x03(\t\x12\x17\n\x0fout_tile_states\x18\x04 \x03(\x05\"\x83\x02\n\x11\x41\x63tionDiscardTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x0f\n\x07is_liqi\x18\x03 \x01(\x08\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x10\n\x08zhenting\x18\x06 \x01(\x08\x12!\n\x08tingpais\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08is_wliqi\x18\t \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x84\x02\n\x11RecordDiscardTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x0f\n\x07is_liqi\x18\x03 \x01(\x08\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x10\n\x08zhenting\x18\x06 \x03(\x08\x12!\n\x08tingpais\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08is_wliqi\x18\t \x01(\x08\x12-\n\noperations\x18\n \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\x12\n\ntile_state\x18\x0b \x01(\r\x12\x1a\n\x04muyu\x18\x0c \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x8d\x02\n\x0e\x41\x63tionDealTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x03 \x01(\r\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12(\n\x08tingpais\x18\x08 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\x12\n\ntile_state\x18\t \x01(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xe3\x01\n\x0eRecordDealTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x03 \x01(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x03(\x08\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x12\n\ntile_state\x18\t \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x87\x02\n\x11\x41\x63tionChiPengGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x03(\t\x12\r\n\x05\x66roms\x18\x04 \x03(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12,\n\toperation\x18\x06 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12(\n\x08tingpais\x18\x08 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\x13\n\x0btile_states\x18\t \x03(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xdd\x01\n\x11RecordChiPengGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x03(\t\x12\r\n\x05\x66roms\x18\x04 \x03(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\x07 \x03(\x08\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0btile_states\x18\t \x03(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xce\x01\n\x13\x41\x63tionAnGangAddGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x01(\t\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12!\n\x08tingpais\x18\x08 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\x1a\n\x04muyu\x18\t \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x9a\x01\n\x13RecordAnGangAddGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x01(\t\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12-\n\noperations\x18\x07 \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xcc\x01\n\x0b\x41\x63tionBaBei\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12!\n\x08tingpais\x18\x08 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05moqie\x18\t \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x98\x01\n\x0bRecordBaBei\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12-\n\noperations\x18\x07 \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05moqie\x18\x08 \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xc2\x01\n\nActionHule\x12\x1b\n\x05hules\x18\x01 \x03(\x0b\x32\x0c.lq.HuleInfo\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xc2\x01\n\nRecordHule\x12\x1b\n\x05hules\x18\x01 \x03(\x0b\x32\x0c.lq.HuleInfo\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xc6\x01\n\x10HuInfoXueZhanMid\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x12\n\nhand_count\x18\x02 \x01(\r\x12\x0c\n\x04hand\x18\x03 \x03(\t\x12\x0c\n\x04ming\x18\x04 \x03(\t\x12\x0f\n\x07hu_tile\x18\x05 \x01(\t\x12\x0c\n\x04zimo\x18\x06 \x01(\x08\x12\r\n\x05yiman\x18\x07 \x01(\x08\x12\r\n\x05\x63ount\x18\x08 \x01(\r\x12\x19\n\x04\x66\x61ns\x18\t \x03(\x0b\x32\x0b.lq.FanInfo\x12\n\n\x02\x66u\x18\n \x01(\r\x12\x10\n\x08title_id\x18\x0b \x01(\r\"\xd1\x01\n\x14\x41\x63tionHuleXueZhanMid\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x1d\n\x04liqi\x18\t \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\n \x01(\x08\"\xd1\x01\n\x14RecordHuleXueZhanMid\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x1d\n\x04liqi\x18\t \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\n \x03(\x08\"\xf9\x01\n\x14\x41\x63tionHuleXueZhanEnd\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x04 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x05 \x01(\r\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xf9\x01\n\x14RecordHuleXueZhanEnd\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x04 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x05 \x01(\r\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xce\x01\n\x0b\x41\x63tionLiuJu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x1c\n\x07gameend\x18\x02 \x01(\x0b\x32\x0b.lq.GameEnd\x12\x0c\n\x04seat\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x16\n\x0e\x61llplayertiles\x18\x06 \x03(\t\x12\x1a\n\x04muyu\x18\x07 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xce\x01\n\x0bRecordLiuJu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x1c\n\x07gameend\x18\x02 \x01(\x0b\x32\x0b.lq.GameEnd\x12\x0c\n\x04seat\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x16\n\x0e\x61llplayertiles\x18\x06 \x03(\t\x12\x1a\n\x04muyu\x18\x07 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"g\n\x10NoTilePlayerInfo\x12\x0f\n\x07tingpai\x18\x03 \x01(\x08\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12\x1e\n\x05tings\x18\x05 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\x14\n\x0c\x61lready_hule\x18\x06 \x01(\x08\"\x83\x01\n\x0fNoTileScoreInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12\x0c\n\x04ming\x18\x05 \x03(\t\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\r\n\x05score\x18\x07 \x01(\r\"\xc2\x01\n\x0c\x41\x63tionNoTile\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12%\n\x07players\x18\x02 \x03(\x0b\x32\x14.lq.NoTilePlayerInfo\x12#\n\x06scores\x18\x03 \x03(\x0b\x32\x13.lq.NoTileScoreInfo\x12\x0f\n\x07gameend\x18\x04 \x01(\x08\x12\x1a\n\x04muyu\x18\x05 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xc2\x01\n\x0cRecordNoTile\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12%\n\x07players\x18\x02 \x03(\x0b\x32\x14.lq.NoTilePlayerInfo\x12#\n\x06scores\x18\x03 \x03(\x0b\x32\x13.lq.NoTileScoreInfo\x12\x0f\n\x07gameend\x18\x04 \x01(\x08\x12\x1a\n\x04muyu\x18\x05 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\x1d\n\rPlayerLeaving\x12\x0c\n\x04seat\x18\x01 \x01(\r\"C\n\x0bReqAuthGame\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\"\xb2\x01\n\x0bResAuthGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x07players\x18\x02 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x11\n\tseat_list\x18\x03 \x03(\r\x12\x15\n\ris_game_start\x18\x04 \x01(\x08\x12#\n\x0bgame_config\x18\x05 \x01(\x0b\x32\x0e.lq.GameConfig\x12\x15\n\rready_id_list\x18\x06 \x03(\r\"\xb8\x01\n\x0bGameRestore\x12\"\n\x08snapshot\x18\x01 \x01(\x0b\x32\x10.lq.GameSnapshot\x12$\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32\x13.lq.ActionPrototype\x12\x1b\n\x13passed_waiting_time\x18\x03 \x01(\r\x12\x12\n\ngame_state\x18\x04 \x01(\r\x12\x12\n\nstart_time\x18\x05 \x01(\r\x12\x1a\n\x12last_pause_time_ms\x18\x06 \x01(\r\"m\n\x0cResEnterGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0e\n\x06is_end\x18\x02 \x01(\x08\x12\x0c\n\x04step\x18\x03 \x01(\r\x12%\n\x0cgame_restore\x18\x04 \x01(\x0b\x32\x0f.lq.GameRestore\"-\n\x0bReqSyncGame\x12\x10\n\x08round_id\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\r\"l\n\x0bResSyncGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0e\n\x06is_end\x18\x02 \x01(\x08\x12\x0c\n\x04step\x18\x03 \x01(\r\x12%\n\x0cgame_restore\x18\x04 \x01(\x0b\x32\x0f.lq.GameRestore\"\xb6\x01\n\x10ReqSelfOperation\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05index\x18\x02 \x01(\r\x12\x0c\n\x04tile\x18\x03 \x01(\t\x12\x18\n\x10\x63\x61ncel_operation\x18\x04 \x01(\x08\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x0f\n\x07timeuse\x18\x06 \x01(\r\x12\x12\n\ntile_state\x18\x07 \x01(\x05\x12\x14\n\x0c\x63hange_tiles\x18\x08 \x03(\t\x12\x13\n\x0btile_states\x18\t \x03(\x05\"X\n\x0eReqChiPengGang\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05index\x18\x02 \x01(\r\x12\x18\n\x10\x63\x61ncel_operation\x18\x03 \x01(\x08\x12\x0f\n\x07timeuse\x18\x06 \x01(\r\":\n\x12ReqBroadcastInGame\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\x12\x13\n\x0b\x65xcept_self\x18\x02 \x01(\x08\")\n\x14ReqGMCommandInGaming\x12\x11\n\tjson_data\x18\x01 \x01(\t\"W\n\x12ResGamePlayerState\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\nstate_list\x18\x02 \x03(\x0e\x32\x13.lq.GamePlayerState\"\x1d\n\x0eReqVoteGameEnd\x12\x0b\n\x03yes\x18\x01 \x01(\x08\"U\n\x0eResGameEndVote\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x18\n\x10vote_cd_end_time\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\"\x1f\n\x0eReqAuthObserve\x12\r\n\x05token\x18\x01 \x01(\t\"V\n\x0fResStartObserve\x12\x1e\n\x04head\x18\x01 \x01(\x0b\x32\x10.lq.GameLiveHead\x12#\n\x06passed\x18\x02 \x01(\x0b\x32\x13.lq.GameLiveSegment\"7\n\rNotifyNewGame\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x13\n\x0bplayer_list\x18\x02 \x03(\t\"2\n\x19NotifyPlayerLoadGameReady\x12\x15\n\rready_id_list\x18\x01 \x03(\r\"4\n\x13NotifyGameBroadcast\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"8\n\x13NotifyGameEndResult\x12!\n\x06result\x18\x01 \x01(\x0b\x32\x11.lq.GameEndResult\"%\n\x13NotifyGameTerminate\x12\x0e\n\x06reason\x18\x01 \x01(\t\"O\n\x1bNotifyPlayerConnectionState\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\x05state\x18\x02 \x01(\x0e\x32\x13.lq.GamePlayerState\"k\n\x18NotifyAccountLevelChange\x12 \n\x06origin\x18\x01 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x1f\n\x05\x66inal\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x0c\n\x04type\x18\x03 \x01(\r\"\x84\x05\n\x16NotifyGameFinishReward\x12\x0f\n\x07mode_id\x18\x01 \x01(\r\x12<\n\x0clevel_change\x18\x02 \x01(\x0b\x32&.lq.NotifyGameFinishReward.LevelChange\x12:\n\x0bmatch_chest\x18\x03 \x01(\x0b\x32%.lq.NotifyGameFinishReward.MatchChest\x12@\n\x0emain_character\x18\x04 \x01(\x0b\x32(.lq.NotifyGameFinishReward.MainCharacter\x12@\n\x0e\x63haracter_gift\x18\x05 \x01(\x0b\x32(.lq.NotifyGameFinishReward.CharacterGift\x1a^\n\x0bLevelChange\x12 \n\x06origin\x18\x01 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x1f\n\x05\x66inal\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x0c\n\x04type\x18\x03 \x01(\r\x1aq\n\nMatchChest\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x0e\n\x06origin\x18\x02 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\x12\x11\n\tis_graded\x18\x04 \x01(\x08\x12\x1f\n\x07rewards\x18\x05 \x03(\x0b\x32\x0e.lq.RewardSlot\x1a\x38\n\rMainCharacter\x12\r\n\x05level\x18\x01 \x01(\r\x12\x0b\n\x03\x65xp\x18\x02 \x01(\r\x12\x0b\n\x03\x61\x64\x64\x18\x03 \x01(\r\x1aN\n\rCharacterGift\x12\x0e\n\x06origin\x18\x01 \x01(\r\x12\r\n\x05\x66inal\x18\x02 \x01(\r\x12\x0b\n\x03\x61\x64\x64\x18\x03 \x01(\r\x12\x11\n\tis_graded\x18\x04 \x01(\x08\"\xa0\x01\n\x14NotifyActivityReward\x12@\n\x0f\x61\x63tivity_reward\x18\x01 \x03(\x0b\x32\'.lq.NotifyActivityReward.ActivityReward\x1a\x46\n\x0e\x41\x63tivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x1f\n\x07rewards\x18\x02 \x03(\x0b\x32\x0e.lq.RewardSlot\"\x8a\x01\n\x13NotifyActivityPoint\x12>\n\x0f\x61\x63tivity_points\x18\x01 \x03(\x0b\x32%.lq.NotifyActivityPoint.ActivityPoint\x1a\x33\n\rActivityPoint\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"\x9c\x01\n\x16NotifyLeaderboardPoint\x12G\n\x12leaderboard_points\x18\x01 \x03(\x0b\x32+.lq.NotifyLeaderboardPoint.LeaderboardPoint\x1a\x39\n\x10LeaderboardPoint\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"!\n\x0fNotifyGamePause\x12\x0e\n\x06paused\x18\x01 \x01(\x08\"\xa0\x01\n\x11NotifyEndGameVote\x12\x31\n\x07results\x18\x01 \x03(\x0b\x32 .lq.NotifyEndGameVote.VoteResult\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x15\n\rduration_time\x18\x03 \x01(\r\x1a-\n\nVoteResult\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0b\n\x03yes\x18\x02 \x01(\x08\"3\n\x11NotifyObserveData\x12\x1e\n\x04unit\x18\x01 \x01(\x0b\x32\x10.lq.GameLiveUnit*=\n\x0fGamePlayerState\x12\x08\n\x04NULL\x10\x00\x12\x08\n\x04\x41UTH\x10\x01\x12\x0b\n\x07SYNCING\x10\x02\x12\t\n\x05READY\x10\x03\x32\xd4x\n\x05Lobby\x12;\n\x13\x66\x65tchConnectionInfo\x12\r.lq.ReqCommon\x1a\x15.lq.ResConnectionInfo\x12\x34\n\x06signup\x12\x14.lq.ReqSignupAccount\x1a\x14.lq.ResSignupAccount\x12#\n\x05login\x12\x0c.lq.ReqLogin\x1a\x0c.lq.ResLogin\x12,\n\x0cloginSuccess\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\nemailLogin\x12\x11.lq.ReqEmailLogin\x1a\x0c.lq.ResLogin\x12\x32\n\noauth2Auth\x12\x11.lq.ReqOauth2Auth\x1a\x11.lq.ResOauth2Auth\x12\x35\n\x0boauth2Check\x12\x12.lq.ReqOauth2Check\x1a\x12.lq.ResOauth2Check\x12\x38\n\x0coauth2Signup\x12\x13.lq.ReqOauth2Signup\x1a\x13.lq.ResOauth2Signup\x12/\n\x0boauth2Login\x12\x12.lq.ReqOauth2Login\x1a\x0c.lq.ResLogin\x12\x35\n\x0b\x64mmPreLogin\x12\x12.lq.ReqDMMPreLogin\x1a\x12.lq.ResDMMPreLogin\x12\x44\n\x15\x63reatePhoneVerifyCode\x12\x1c.lq.ReqCreatePhoneVerifyCode\x1a\r.lq.ResCommon\x12\x44\n\x15\x63reateEmailVerifyCode\x12\x1c.lq.ReqCreateEmailVerifyCode\x1a\r.lq.ResCommon\x12N\n\x14verfifyCodeForSecure\x12\x1a.lq.ReqVerifyCodeForSecure\x1a\x1a.lq.ResVerfiyCodeForSecure\x12\x38\n\x0f\x62indPhoneNumber\x12\x16.lq.ReqBindPhoneNumber\x1a\r.lq.ResCommon\x12<\n\x11unbindPhoneNumber\x12\x18.lq.ReqUnbindPhoneNumber\x1a\r.lq.ResCommon\x12@\n\x13\x66\x65tchPhoneLoginBind\x12\r.lq.ReqCommon\x1a\x1a.lq.ResFetchPhoneLoginBind\x12\x42\n\x14\x63reatePhoneLoginBind\x12\x1b.lq.ReqCreatePhoneLoginBind\x1a\r.lq.ResCommon\x12,\n\tbindEmail\x12\x10.lq.ReqBindEmail\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyPassword\x12\x15.lq.ReqModifyPassword\x1a\r.lq.ResCommon\x12\x30\n\x0b\x62indAccount\x12\x12.lq.ReqBindAccount\x1a\r.lq.ResCommon\x12&\n\x06logout\x12\r.lq.ReqLogout\x1a\r.lq.ResLogout\x12*\n\x08heatbeat\x12\x0f.lq.ReqHeatBeat\x1a\r.lq.ResCommon\x12,\n\tloginBeat\x12\x10.lq.ReqLoginBeat\x1a\r.lq.ResCommon\x12\x36\n\x0e\x63reateNickname\x12\x15.lq.ReqCreateNickname\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyNickname\x12\x15.lq.ReqModifyNickname\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyBirthday\x12\x15.lq.ReqModifyBirthday\x1a\r.lq.ResCommon\x12+\n\tfetchRoom\x12\r.lq.ReqCommon\x1a\x0f.lq.ResSelfRoom\x12\x32\n\ncreateRoom\x12\x11.lq.ReqCreateRoom\x1a\x11.lq.ResCreateRoom\x12,\n\x08joinRoom\x12\x0f.lq.ReqJoinRoom\x1a\x0f.lq.ResJoinRoom\x12)\n\tleaveRoom\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12,\n\treadyPlay\x12\x10.lq.ReqRoomReady\x1a\r.lq.ResCommon\x12\x34\n\x0e\x64ressingStatus\x12\x13.lq.ReqRoomDressing\x1a\r.lq.ResCommon\x12,\n\tstartRoom\x12\x10.lq.ReqRoomStart\x1a\r.lq.ResCommon\x12,\n\nkickPlayer\x12\x0f.lq.ReqRoomKick\x1a\r.lq.ResCommon\x12.\n\nmodifyRoom\x12\x11.lq.ReqModifyRoom\x1a\r.lq.ResCommon\x12\x31\n\tmatchGame\x12\x15.lq.ReqJoinMatchQueue\x1a\r.lq.ResCommon\x12\x35\n\x0b\x63\x61ncelMatch\x12\x17.lq.ReqCancelMatchQueue\x1a\r.lq.ResCommon\x12:\n\x10\x66\x65tchAccountInfo\x12\x12.lq.ReqAccountInfo\x1a\x12.lq.ResAccountInfo\x12\x32\n\x0c\x63hangeAvatar\x12\x13.lq.ReqChangeAvatar\x1a\r.lq.ResCommon\x12\x34\n\x14receiveVersionReward\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12U\n\x19\x66\x65tchAccountStatisticInfo\x12\x1b.lq.ReqAccountStatisticInfo\x1a\x1b.lq.ResAccountStatisticInfo\x12T\n\x1d\x66\x65tchAccountChallengeRankInfo\x12\x12.lq.ReqAccountInfo\x1a\x1f.lq.ResAccountChallengeRankInfo\x12G\n\x19\x66\x65tchAccountCharacterInfo\x12\r.lq.ReqCommon\x1a\x1b.lq.ResAccountCharacterInfo\x12\x38\n\x0cshopPurchase\x12\x13.lq.ReqShopPurchase\x1a\x13.lq.ResShopPurchase\x12\x37\n\x0f\x66\x65tchGameRecord\x12\x11.lq.ReqGameRecord\x1a\x11.lq.ResGameRecord\x12\x32\n\x0ereadGameRecord\x12\x11.lq.ReqGameRecord\x1a\r.lq.ResCommon\x12\x43\n\x13\x66\x65tchGameRecordList\x12\x15.lq.ReqGameRecordList\x1a\x15.lq.ResGameRecordList\x12M\n\x1c\x66\x65tchCollectedGameRecordList\x12\r.lq.ReqCommon\x1a\x1e.lq.ResCollectedGameRecordList\x12L\n\x16\x66\x65tchGameRecordsDetail\x12\x18.lq.ReqGameRecordsDetail\x1a\x18.lq.ResGameRecordsDetail\x12V\n\x16\x61\x64\x64\x43ollectedGameRecord\x12\x1d.lq.ReqAddCollectedGameRecord\x1a\x1d.lq.ResAddCollectedGameRecord\x12_\n\x19removeCollectedGameRecord\x12 .lq.ReqRemoveCollectedGameRecord\x1a .lq.ResRemoveCollectedGameRecord\x12t\n changeCollectedGameRecordRemarks\x12\'.lq.ReqChangeCollectedGameRecordRemarks\x1a\'.lq.ResChangeCollectedGameRecordRemarks\x12I\n\x15\x66\x65tchLevelLeaderboard\x12\x17.lq.ReqLevelLeaderboard\x1a\x17.lq.ResLevelLeaderboard\x12U\n\x19\x66\x65tchChallengeLeaderboard\x12\x1b.lq.ReqChallangeLeaderboard\x1a\x1b.lq.ResChallengeLeaderboard\x12O\n\x17\x66\x65tchMutiChallengeLevel\x12\x19.lq.ReqMutiChallengeLevel\x1a\x19.lq.ResMutiChallengeLevel\x12I\n\x16\x66\x65tchMultiAccountBrief\x12\x15.lq.ReqMultiAccountId\x1a\x18.lq.ResMultiAccountBrief\x12\x33\n\x0f\x66\x65tchFriendList\x12\r.lq.ReqCommon\x1a\x11.lq.ResFriendList\x12=\n\x14\x66\x65tchFriendApplyList\x12\r.lq.ReqCommon\x1a\x16.lq.ResFriendApplyList\x12\x30\n\x0b\x61pplyFriend\x12\x12.lq.ReqApplyFriend\x1a\r.lq.ResCommon\x12<\n\x11handleFriendApply\x12\x18.lq.ReqHandleFriendApply\x1a\r.lq.ResCommon\x12\x32\n\x0cremoveFriend\x12\x13.lq.ReqRemoveFriend\x1a\r.lq.ResCommon\x12G\n\x11searchAccountById\x12\x18.lq.ReqSearchAccountById\x1a\x18.lq.ResSearchAccountById\x12V\n\x16searchAccountByPattern\x12\x1d.lq.ReqSearchAccountByPattern\x1a\x1d.lq.ResSearchAccountByPattern\x12=\n\x11\x66\x65tchAccountState\x12\x12.lq.ReqAccountList\x1a\x14.lq.ResAccountStates\x12-\n\x0c\x66\x65tchBagInfo\x12\r.lq.ReqCommon\x1a\x0e.lq.ResBagInfo\x12.\n\nuseBagItem\x12\x11.lq.ReqUseBagItem\x1a\r.lq.ResCommon\x12\x36\n\x0eopenManualItem\x12\x15.lq.ReqOpenManualItem\x1a\r.lq.ResCommon\x12P\n\x14openRandomRewardItem\x12\x1b.lq.ReqOpenRandomRewardItem\x1a\x1b.lq.ResOpenRandomRewardItem\x12G\n\x11openAllRewardItem\x12\x18.lq.ReqOpenAllRewardItem\x1a\x18.lq.ResOpenAllRewardItem\x12\x32\n\x0c\x63omposeShard\x12\x13.lq.ReqComposeShard\x1a\r.lq.ResCommon\x12\x42\n\x11\x66\x65tchAnnouncement\x12\x18.lq.ReqFetchAnnouncement\x1a\x13.lq.ResAnnouncement\x12:\n\x10readAnnouncement\x12\x17.lq.ReqReadAnnouncement\x1a\r.lq.ResCommon\x12/\n\rfetchMailInfo\x12\r.lq.ReqCommon\x1a\x0f.lq.ResMailInfo\x12*\n\x08readMail\x12\x0f.lq.ReqReadMail\x1a\r.lq.ResCommon\x12.\n\ndeleteMail\x12\x11.lq.ReqDeleteMail\x1a\r.lq.ResCommon\x12>\n\x16takeAttachmentFromMail\x12\x15.lq.ReqTakeAttachment\x1a\r.lq.ResCommon\x12\\\n\x18receiveAchievementReward\x12\x1f.lq.ReqReceiveAchievementReward\x1a\x1f.lq.ResReceiveAchievementReward\x12k\n\x1dreceiveAchievementGroupReward\x12$.lq.ReqReceiveAchievementGroupReward\x1a$.lq.ResReceiveAchievementGroupReward\x12\x42\n\x14\x66\x65tchAchievementRate\x12\r.lq.ReqCommon\x1a\x1b.lq.ResFetchAchievementRate\x12\x35\n\x10\x66\x65tchAchievement\x12\r.lq.ReqCommon\x1a\x12.lq.ResAchievement\x12.\n\nbuyShiLian\x12\x11.lq.ReqBuyShiLian\x1a\r.lq.ResCommon\x12,\n\x0cmatchShiLian\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\rgoNextShiLian\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12<\n\x11updateClientValue\x12\x18.lq.ReqUpdateClientValue\x1a\r.lq.ResCommon\x12\x35\n\x10\x66\x65tchClientValue\x12\r.lq.ReqCommon\x1a\x12.lq.ResClientValue\x12\x34\n\rclientMessage\x12\x14.lq.ReqClientMessage\x1a\r.lq.ResCommon\x12I\n\x15\x66\x65tchCurrentMatchInfo\x12\x17.lq.ReqCurrentMatchInfo\x1a\x17.lq.ResCurrentMatchInfo\x12\x32\n\x0cuserComplain\x12\x13.lq.ReqUserComplain\x1a\r.lq.ResCommon\x12;\n\x13\x66\x65tchReviveCoinInfo\x12\r.lq.ReqCommon\x1a\x15.lq.ResReviveCoinInfo\x12.\n\x0egainReviveCoin\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x31\n\x0e\x66\x65tchDailyTask\x12\r.lq.ReqCommon\x1a\x10.lq.ResDailyTask\x12\x44\n\x10refreshDailyTask\x12\x17.lq.ReqRefreshDailyTask\x1a\x17.lq.ResRefreshDailyTask\x12\x35\n\x0buseGiftCode\x12\x12.lq.ReqUseGiftCode\x1a\x12.lq.ResUseGiftCode\x12\x43\n\x12useSpecialGiftCode\x12\x12.lq.ReqUseGiftCode\x1a\x19.lq.ResUseSpecialGiftCode\x12\x31\n\x0e\x66\x65tchTitleList\x12\r.lq.ReqCommon\x1a\x10.lq.ResTitleList\x12*\n\x08useTitle\x12\x0f.lq.ReqUseTitle\x1a\r.lq.ResCommon\x12<\n\x11sendClientMessage\x12\x18.lq.ReqSendClientMessage\x1a\r.lq.ResCommon\x12=\n\x11\x66\x65tchGameLiveInfo\x12\x13.lq.ReqGameLiveInfo\x1a\x13.lq.ResGameLiveInfo\x12R\n\x18\x66\x65tchGameLiveLeftSegment\x12\x1a.lq.ReqGameLiveLeftSegment\x1a\x1a.lq.ResGameLiveLeftSegment\x12=\n\x11\x66\x65tchGameLiveList\x12\x13.lq.ReqGameLiveList\x1a\x13.lq.ResGameLiveList\x12;\n\x13\x66\x65tchCommentSetting\x12\r.lq.ReqCommon\x1a\x15.lq.ResCommentSetting\x12\x42\n\x14updateCommentSetting\x12\x1b.lq.ReqUpdateCommentSetting\x1a\r.lq.ResCommon\x12\x44\n\x10\x66\x65tchCommentList\x12\x17.lq.ReqFetchCommentList\x1a\x17.lq.ResFetchCommentList\x12M\n\x13\x66\x65tchCommentContent\x12\x1a.lq.ReqFetchCommentContent\x1a\x1a.lq.ResFetchCommentContent\x12\x32\n\x0cleaveComment\x12\x13.lq.ReqLeaveComment\x1a\r.lq.ResCommon\x12\x34\n\rdeleteComment\x12\x14.lq.ReqDeleteComment\x1a\r.lq.ResCommon\x12<\n\x11updateReadComment\x12\x18.lq.ReqUpdateReadComment\x1a\r.lq.ResCommon\x12\x39\n\x12\x66\x65tchRollingNotice\x12\r.lq.ReqCommon\x1a\x14.lq.ReqRollingNotice\x12\x33\n\x0f\x66\x65tchServerTime\x12\r.lq.ReqCommon\x1a\x11.lq.ResServerTime\x12W\n\x15\x66\x65tchPlatformProducts\x12\x1e.lq.ReqPlatformBillingProducts\x1a\x1e.lq.ResPlatformBillingProducts\x12\x44\n\x15\x63\x61ncelGooglePlayOrder\x12\x1c.lq.ReqCancelGooglePlayOrder\x1a\r.lq.ResCommon\x12/\n\topenChest\x12\x10.lq.ReqOpenChest\x1a\x10.lq.ResOpenChest\x12\x44\n\x10\x62uyFromChestShop\x12\x17.lq.ReqBuyFromChestShop\x1a\x17.lq.ResBuyFromChestShop\x12=\n\x14\x66\x65tchDailySignInInfo\x12\r.lq.ReqCommon\x1a\x16.lq.ResDailySignInInfo\x12-\n\rdoDailySignIn\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x44\n\x10\x64oActivitySignIn\x12\x17.lq.ReqDoActivitySignIn\x1a\x17.lq.ResDoActivitySignIn\x12\x39\n\x12\x66\x65tchCharacterInfo\x12\r.lq.ReqCommon\x1a\x14.lq.ResCharacterInfo\x12@\n\x13updateCharacterSort\x12\x1a.lq.ReqUpdateCharacterSort\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeMainCharacter\x12\x1a.lq.ReqChangeMainCharacter\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeCharacterSkin\x12\x1a.lq.ReqChangeCharacterSkin\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeCharacterView\x12\x1a.lq.ReqChangeCharacterView\x1a\r.lq.ResCommon\x12M\n\x13sendGiftToCharacter\x12\x1a.lq.ReqSendGiftToCharacter\x1a\x1a.lq.ResSendGiftToCharacter\x12*\n\x08sellItem\x12\x0f.lq.ReqSellItem\x1a\r.lq.ResCommon\x12\x33\n\x0f\x66\x65tchCommonView\x12\r.lq.ReqCommon\x1a\x11.lq.ResCommonView\x12:\n\x10\x63hangeCommonView\x12\x17.lq.ReqChangeCommonView\x1a\r.lq.ResCommon\x12\x38\n\x0fsaveCommonViews\x12\x16.lq.ReqSaveCommonViews\x1a\r.lq.ResCommon\x12:\n\x10\x66\x65tchCommonViews\x12\x12.lq.ReqCommonViews\x1a\x12.lq.ResCommonViews\x12;\n\x13\x66\x65tchAllCommonViews\x12\r.lq.ReqCommon\x1a\x15.lq.ResAllcommonViews\x12\x34\n\ruseCommonView\x12\x14.lq.ReqUseCommonView\x1a\r.lq.ResCommon\x12\x44\n\x10upgradeCharacter\x12\x17.lq.ReqUpgradeCharacter\x1a\x17.lq.ResUpgradeCharacter\x12\x39\n\x11\x61\x64\x64\x46inishedEnding\x12\x15.lq.ReqFinishedEnding\x1a\r.lq.ResCommon\x12;\n\x13receiveEndingReward\x12\x15.lq.ReqFinishedEnding\x1a\r.lq.ResCommon\x12\x34\n\x11gameMasterCommand\x12\x10.lq.ReqGMCommand\x1a\r.lq.ResCommon\x12/\n\rfetchShopInfo\x12\r.lq.ReqCommon\x1a\x0f.lq.ResShopInfo\x12\x35\n\x0b\x62uyFromShop\x12\x12.lq.ReqBuyFromShop\x1a\x12.lq.ResBuyFromShop\x12.\n\nbuyFromZHP\x12\x11.lq.ReqBuyFromZHP\x1a\r.lq.ResCommon\x12;\n\x0erefreshZHPShop\x12\x12.lq.ReqReshZHPShop\x1a\x15.lq.ResRefreshZHPShop\x12=\n\x14\x66\x65tchMonthTicketInfo\x12\r.lq.ReqCommon\x1a\x16.lq.ResMonthTicketInfo\x12>\n\x0epayMonthTicket\x12\x15.lq.ReqPayMonthTicket\x1a\x15.lq.ResPayMonthTicket\x12:\n\x10\x65xchangeCurrency\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12<\n\x12\x65xchangeChestStone\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12\x39\n\x0f\x65xchangeDiamond\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12;\n\x13\x66\x65tchServerSettings\x12\r.lq.ReqCommon\x1a\x15.lq.ResServerSettings\x12=\n\x14\x66\x65tchAccountSettings\x12\r.lq.ReqCommon\x1a\x16.lq.ResAccountSettings\x12\x44\n\x15updateAccountSettings\x12\x1c.lq.ReqUpdateAccountSettings\x1a\r.lq.ResCommon\x12=\n\x14\x66\x65tchModNicknameTime\x12\r.lq.ReqCommon\x1a\x16.lq.ResModNicknameTime\x12Y\n\x17\x63reateWechatNativeOrder\x12\x1e.lq.ReqCreateWechatNativeOrder\x1a\x1e.lq.ResCreateWechatNativeOrder\x12P\n\x14\x63reateWechatAppOrder\x12\x1b.lq.ReqCreateWechatAppOrder\x1a\x1b.lq.ResCreateWechatAppOrder\x12G\n\x11\x63reateAlipayOrder\x12\x18.lq.ReqCreateAlipayOrder\x1a\x18.lq.ResCreateAlipayOrder\x12S\n\x15\x63reateAlipayScanOrder\x12\x1c.lq.ReqCreateAlipayScanOrder\x1a\x1c.lq.ResCreateAlipayScanOrder\x12P\n\x14\x63reateAlipayAppOrder\x12\x1b.lq.ReqCreateAlipayAppOrder\x1a\x1b.lq.ResCreateAlipayAppOrder\x12Y\n\x17\x63reateJPCreditCardOrder\x12\x1e.lq.ReqCreateJPCreditCardOrder\x1a\x1e.lq.ResCreateJPCreditCardOrder\x12M\n\x13\x63reateJPPaypalOrder\x12\x1a.lq.ReqCreateJPPaypalOrder\x1a\x1a.lq.ResCreateJPPaypalOrder\x12\x41\n\x0f\x63reateJPAuOrder\x12\x16.lq.ReqCreateJPAuOrder\x1a\x16.lq.ResCreateJPAuOrder\x12M\n\x13\x63reateJPDocomoOrder\x12\x1a.lq.ReqCreateJPDocomoOrder\x1a\x1a.lq.ResCreateJPDocomoOrder\x12S\n\x15\x63reateJPWebMoneyOrder\x12\x1c.lq.ReqCreateJPWebMoneyOrder\x1a\x1c.lq.ResCreateJPWebMoneyOrder\x12S\n\x15\x63reateJPSoftbankOrder\x12\x1c.lq.ReqCreateJPSoftbankOrder\x1a\x1c.lq.ResCreateJPSoftbankOrder\x12M\n\x13\x63reateENPaypalOrder\x12\x1a.lq.ReqCreateENPaypalOrder\x1a\x1a.lq.ResCreateENPaypalOrder\x12Y\n\x17\x63reateENMasterCardOrder\x12\x1e.lq.ReqCreateENMasterCardOrder\x1a\x1e.lq.ResCreateENMasterCardOrder\x12G\n\x11\x63reateENVisaOrder\x12\x18.lq.ReqCreateENVisaOrder\x1a\x18.lq.ResCreateENVisaOrder\x12\x44\n\x10\x63reateENJCBOrder\x12\x17.lq.ReqCreateENJCBOrder\x1a\x17.lq.ResCreateENJCBOrder\x12M\n\x13\x63reateENAlipayOrder\x12\x1a.lq.ReqCreateENAlipayOrder\x1a\x1a.lq.ResCreateENAlipayOrder\x12>\n\x0e\x63reateDMMOrder\x12\x15.lq.ReqCreateDMMOrder\x1a\x15.lq.ResCreateDmmOrder\x12>\n\x0e\x63reateIAPOrder\x12\x15.lq.ReqCreateIAPOrder\x1a\x15.lq.ResCreateIAPOrder\x12\x44\n\x10\x63reateSteamOrder\x12\x17.lq.ReqCreateSteamOrder\x1a\x17.lq.ResCreateSteamOrder\x12:\n\x10verifySteamOrder\x12\x17.lq.ReqVerifySteamOrder\x1a\r.lq.ResCommon\x12N\n\x18\x63reateMyCardAndroidOrder\x12\x18.lq.ReqCreateMyCardOrder\x1a\x18.lq.ResCreateMyCardOrder\x12J\n\x14\x63reateMyCardWebOrder\x12\x18.lq.ReqCreateMyCardOrder\x1a\x18.lq.ResCreateMyCardOrder\x12G\n\x11\x63reatePaypalOrder\x12\x18.lq.ReqCreatePaypalOrder\x1a\x18.lq.ResCreatePaypalOrder\x12G\n\x11\x63reateXsollaOrder\x12\x18.lq.ReqCreateXsollaOrder\x1a\x18.lq.ResCreateXsollaOrder\x12<\n\x11verifyMyCardOrder\x12\x18.lq.ReqVerifyMyCardOrder\x1a\r.lq.ResCommon\x12P\n\x14verificationIAPOrder\x12\x1b.lq.ReqVerificationIAPOrder\x1a\x1b.lq.ResVerificationIAPOrder\x12J\n\x14\x63reateYostarSDKOrder\x12\x18.lq.ReqCreateYostarOrder\x1a\x18.lq.ResCreateYostarOrder\x12J\n\x12\x63reateBillingOrder\x12\x19.lq.ReqCreateBillingOrder\x1a\x19.lq.ResCreateBillingOrder\x12\x42\n\x14solveGooglePlayOrder\x12\x1b.lq.ReqSolveGooglePlayOrder\x1a\r.lq.ResCommon\x12\x45\n\x15solveGooglePayOrderV3\x12\x1d.lq.ReqSolveGooglePlayOrderV3\x1a\r.lq.ResCommon\x12\'\n\tfetchMisc\x12\r.lq.ReqCommon\x1a\x0b.lq.ResMisc\x12\x38\n\x0fmodifySignature\x12\x16.lq.ReqModifySignature\x1a\r.lq.ResCommon\x12\x33\n\x0f\x66\x65tchIDCardInfo\x12\r.lq.ReqCommon\x1a\x11.lq.ResIDCardInfo\x12:\n\x10updateIDCardInfo\x12\x17.lq.ReqUpdateIDCardInfo\x1a\r.lq.ResCommon\x12\x31\n\x0e\x66\x65tchVipReward\x12\r.lq.ReqCommon\x1a\x10.lq.ResVipReward\x12\x34\n\rgainVipReward\x12\x14.lq.ReqGainVipReward\x1a\r.lq.ResCommon\x12\x62\n\x1a\x66\x65tchCustomizedContestList\x12!.lq.ReqFetchCustomizedContestList\x1a!.lq.ResFetchCustomizedContestList\x12t\n fetchCustomizedContestExtendInfo\x12\'.lq.ReqFetchCustomizedContestExtendInfo\x1a\'.lq.ResFetchCustomizedContestExtendInfo\x12n\n\x1e\x66\x65tchCustomizedContestAuthInfo\x12%.lq.ReqFetchCustomizedContestAuthInfo\x1a%.lq.ResFetchCustomizedContestAuthInfo\x12V\n\x16\x65nterCustomizedContest\x12\x1d.lq.ReqEnterCustomizedContest\x1a\x1d.lq.ResEnterCustomizedContest\x12\x36\n\x16leaveCustomizedContest\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12t\n fetchCustomizedContestOnlineInfo\x12\'.lq.ReqFetchCustomizedContestOnlineInfo\x1a\'.lq.ResFetchCustomizedContestOnlineInfo\x12w\n!fetchCustomizedContestByContestId\x12(.lq.ReqFetchCustomizedContestByContestId\x1a(.lq.ResFetchCustomizedContestByContestId\x12\x46\n\x16startCustomizedContest\x12\x1d.lq.ReqStartCustomizedContest\x1a\r.lq.ResCommon\x12\x35\n\x15stopCustomizedContest\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12k\n\x1djoinCustomizedContestChatRoom\x12$.lq.ReqJoinCustomizedContestChatRoom\x1a$.lq.ResJoinCustomizedContestChatRoom\x12>\n\x1eleaveCustomizedContestChatRoom\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x36\n\x0esayChatMessage\x12\x15.lq.ReqSayChatMessage\x1a\r.lq.ResCommon\x12w\n!fetchCustomizedContestGameRecords\x12(.lq.ReqFetchCustomizedContestGameRecords\x1a(.lq.ResFetchCustomizedContestGameRecords\x12z\n\"fetchCustomizedContestGameLiveList\x12).lq.ReqFetchCustomizedContestGameLiveList\x1a).lq.ResFetchCustomizedContestGameLiveList\x12H\n\x17\x66ollowCustomizedContest\x12\x1e.lq.ReqTargetCustomizedContest\x1a\r.lq.ResCommon\x12J\n\x19unfollowCustomizedContest\x12\x1e.lq.ReqTargetCustomizedContest\x1a\r.lq.ResCommon\x12\x37\n\x11\x66\x65tchActivityList\x12\r.lq.ReqCommon\x1a\x13.lq.ResActivityList\x12\x45\n\x18\x66\x65tchAccountActivityData\x12\r.lq.ReqCommon\x1a\x1a.lq.ResAccountActivityData\x12P\n\x14\x65xchangeActivityItem\x12\x1b.lq.ReqExchangeActivityItem\x1a\x1b.lq.ResExchangeActivityItem\x12\x42\n\x14\x63ompleteActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12\x46\n\x18\x63ompleteActivityFlipTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12H\n\x1a\x63ompletePeriodActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12H\n\x1a\x63ompleteRandomActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12Y\n\x17receiveActivityFlipTask\x12\x1e.lq.ReqReceiveActivityFlipTask\x1a\x1e.lq.ResReceiveActivityFlipTask\x12S\n\x15\x66\x65tchActivityFlipInfo\x12\x1c.lq.ReqFetchActivityFlipInfo\x1a\x1c.lq.ResFetchActivityFlipInfo\x12^\n\"gainAccumulatedPointActivityReward\x12).lq.ReqGainAccumulatedPointActivityReward\x1a\r.lq.ResCommon\x12R\n\x1cgainMultiPointActivityReward\x12#.lq.ReqGainMultiPointActivityReward\x1a\r.lq.ResCommon\x12_\n\x19\x66\x65tchRankPointLeaderboard\x12 .lq.ReqFetchRankPointLeaderboard\x1a .lq.ResFetchRankPointLeaderboard\x12@\n\x13gainRankPointReward\x12\x1a.lq.ReqGainRankPointReward\x1a\r.lq.ResCommon\x12I\n\x17richmanActivityNextMove\x12\x16.lq.ReqRichmanNextMove\x1a\x16.lq.ResRichmanNextMove\x12P\n\x1brichmanAcitivitySpecialMove\x12\x19.lq.ReqRichmanSpecialMove\x1a\x16.lq.ResRichmanNextMove\x12L\n\x18richmanActivityChestInfo\x12\x17.lq.ReqRichmanChestInfo\x1a\x17.lq.ResRichmanChestInfo\x12S\n\x15\x63reateGameObserveAuth\x12\x1c.lq.ReqCreateGameObserveAuth\x1a\x1c.lq.ResCreateGameObserveAuth\x12V\n\x16refreshGameObserveAuth\x12\x1d.lq.ReqRefreshGameObserveAuth\x1a\x1d.lq.ResRefreshGameObserveAuth\x12\x37\n\x11\x66\x65tchActivityBuff\x12\r.lq.ReqCommon\x1a\x13.lq.ResActivityBuff\x12\x46\n\x13upgradeActivityBuff\x12\x1a.lq.ReqUpgradeActivityBuff\x1a\x13.lq.ResActivityBuff\x12:\n\x10upgradeChallenge\x12\r.lq.ReqCommon\x1a\x17.lq.ResUpgradeChallenge\x12:\n\x10refreshChallenge\x12\r.lq.ReqCommon\x1a\x17.lq.ResRefreshChallenge\x12>\n\x12\x66\x65tchChallengeInfo\x12\r.lq.ReqCommon\x1a\x19.lq.ResFetchChallengeInfo\x12N\n\x1a\x66orceCompleteChallengeTask\x12!.lq.ReqForceCompleteChallengeTask\x1a\r.lq.ResCommon\x12\x41\n\x14\x66\x65tchChallengeSeason\x12\r.lq.ReqCommon\x1a\x1a.lq.ResChallengeSeasonInfo\x12\x62\n\x1areceiveChallengeRankReward\x12!.lq.ReqReceiveChallengeRankReward\x1a!.lq.ResReceiveChallengeRankReward\x12\x36\n\x10\x66\x65tchABMatchInfo\x12\r.lq.ReqCommon\x1a\x13.lq.ResFetchABMatch\x12\x32\n\x0c\x62uyInABMatch\x12\x13.lq.ReqBuyInABMatch\x1a\r.lq.ResCommon\x12\x34\n\x14receiveABMatchReward\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12+\n\x0bquitABMatch\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12<\n\x11startUnifiedMatch\x12\x18.lq.ReqStartUnifiedMatch\x1a\r.lq.ResCommon\x12>\n\x12\x63\x61ncelUnifiedMatch\x12\x19.lq.ReqCancelUnifiedMatch\x1a\r.lq.ResCommon\x12@\n\x12\x66\x65tchGamePointRank\x12\x14.lq.ReqGamePointRank\x1a\x14.lq.ResGamePointRank\x12M\n\x16\x66\x65tchSelfGamePointRank\x12\x14.lq.ReqGamePointRank\x1a\x1d.lq.ResFetchSelfGamePointRank2\xf5\x06\n\x08\x46\x61stTest\x12,\n\x08\x61uthGame\x12\x0f.lq.ReqAuthGame\x1a\x0f.lq.ResAuthGame\x12,\n\tenterGame\x12\r.lq.ReqCommon\x1a\x10.lq.ResEnterGame\x12,\n\x08syncGame\x12\x0f.lq.ReqSyncGame\x1a\x0f.lq.ResSyncGame\x12.\n\x0e\x66inishSyncGame\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\rterminateGame\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x35\n\x0einputOperation\x12\x14.lq.ReqSelfOperation\x1a\r.lq.ResCommon\x12\x35\n\x10inputChiPengGang\x12\x12.lq.ReqChiPengGang\x1a\r.lq.ResCommon\x12/\n\x0f\x63onfirmNewRound\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x38\n\x0f\x62roadcastInGame\x12\x16.lq.ReqBroadcastInGame\x1a\r.lq.ResCommon\x12=\n\x12inputGameGMCommand\x12\x18.lq.ReqGMCommandInGaming\x1a\r.lq.ResCommon\x12=\n\x14\x66\x65tchGamePlayerState\x12\r.lq.ReqCommon\x1a\x16.lq.ResGamePlayerState\x12\x31\n\x11\x63heckNetworkDelay\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12,\n\x0c\x63learLeaving\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x35\n\x0bvoteGameEnd\x12\x12.lq.ReqVoteGameEnd\x1a\x12.lq.ResGameEndVote\x12\x30\n\x0b\x61uthObserve\x12\x12.lq.ReqAuthObserve\x1a\r.lq.ResCommon\x12\x32\n\x0cstartObserve\x12\r.lq.ReqCommon\x1a\x13.lq.ResStartObserve\x12+\n\x0bstopObserve\x12\r.lq.ReqCommon\x1a\r.lq.ResCommonb\x06proto3')
+  serialized_pb=_b('\n\x0eprotocol.proto\x12\x02lq\"c\n\x13NotifyRoomGameStart\x12\x10\n\x08game_url\x18\x01 \x01(\t\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\"{\n\x14NotifyMatchGameStart\x12\x10\n\x08game_url\x18\x01 \x01(\t\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x15\n\rmatch_mode_id\x18\x04 \x01(\r\x12\x10\n\x08location\x18\x05 \x01(\t\"\xc2\x01\n\x15NotifyRoomPlayerReady\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05ready\x18\x02 \x01(\x08\x12\x41\n\x0c\x61\x63\x63ount_list\x18\x03 \x01(\x0b\x32+.lq.NotifyRoomPlayerReady.AccountReadyState\x12\x0b\n\x03seq\x18\x04 \x01(\r\x1a\x36\n\x11\x41\x63\x63ountReadyState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05ready\x18\x02 \x01(\x08\"\xd4\x01\n\x18NotifyRoomPlayerDressing\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08\x64ressing\x18\x02 \x01(\x08\x12G\n\x0c\x61\x63\x63ount_list\x18\x03 \x01(\x0b\x32\x31.lq.NotifyRoomPlayerDressing.AccountDressingState\x12\x0b\n\x03seq\x18\x04 \x01(\r\x1a<\n\x14\x41\x63\x63ountDressingState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08\x64ressing\x18\x02 \x01(\x08\"\xb3\x01\n\x16NotifyRoomPlayerUpdate\x12\'\n\x0bupdate_list\x18\x01 \x03(\x0b\x32\x12.lq.PlayerBaseView\x12\x13\n\x0bremove_list\x18\x02 \x03(\r\x12\x10\n\x08owner_id\x18\x03 \x01(\r\x12\x13\n\x0brobot_count\x18\x04 \x01(\r\x12\'\n\x0bplayer_list\x18\x05 \x03(\x0b\x32\x12.lq.PlayerBaseView\x12\x0b\n\x03seq\x18\x06 \x01(\r\"\x13\n\x11NotifyRoomKickOut\"Z\n\x17NotifyFriendStateChange\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12,\n\x0c\x61\x63tive_state\x18\x02 \x01(\x0b\x32\x16.lq.AccountActiveState\"M\n\x16NotifyFriendViewChange\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12 \n\x04\x62\x61se\x18\x02 \x01(\x0b\x32\x12.lq.PlayerBaseView\"R\n\x12NotifyFriendChange\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x1a\n\x06\x66riend\x18\x03 \x01(\x0b\x32\n.lq.Friend\"R\n\x14NotifyNewFriendApply\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\napply_time\x18\x02 \x01(\r\x12\x12\n\nremoved_id\x18\x03 \x01(\r\"X\n\x13NotifyClientMessage\x12\"\n\x06sender\x18\x01 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"8\n\x13NotifyAccountUpdate\x12!\n\x06update\x18\x01 \x01(\x0b\x32\x11.lq.AccountUpdate\"\x14\n\x12NotifyAnotherLogin\"\x15\n\x13NotifyAccountLogout\"_\n\x18NotifyAnnouncementUpdate\x12\'\n\rannouncements\x18\x01 \x03(\x0b\x32\x10.lq.Announcement\x12\x0c\n\x04sort\x18\x02 \x03(\r\x12\x0c\n\x04lang\x18\x03 \x01(\t\"\'\n\rNotifyNewMail\x12\x16\n\x04mail\x18\x01 \x01(\x0b\x32\x08.lq.Mail\"(\n\x10NotifyDeleteMail\x12\x14\n\x0cmail_id_list\x18\x01 \x03(\r\",\n\x16NotifyReviveCoinUpdate\x12\x12\n\nhas_gained\x18\x01 \x01(\x08\"r\n\x15NotifyDailyTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x1c\n\x14max_daily_task_count\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\"@\n\x18NotifyActivityTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"F\n\x1eNotifyActivityPeriodTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"E\n\x1dNotifyAccountRandomTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\"\xaf\x01\n NotifyAccountChallengeTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\r\n\x05level\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\x13\n\x0bmatch_count\x18\x04 \x01(\r\x12\x11\n\tticket_id\x18\x05 \x01(\r\x12\x17\n\x0frewarded_season\x18\x06 \x03(\r\"\x12\n\x10NotifyNewComment\"8\n\x13NotifyRollingNotice\x12!\n\x06notice\x18\x01 \x01(\x0b\x32\x11.lq.RollingNotice\"\x17\n\x15NotifyGiftSendRefresh\"3\n\x10NotifyShopUpdate\x12\x1f\n\tshop_info\x18\x01 \x01(\x0b\x32\x0c.lq.ShopInfo\"\xb7\x01\n\x14NotifyVipLevelChange\x12\x12\n\ngift_limit\x18\x01 \x01(\r\x12\x18\n\x10\x66riend_max_count\x18\x02 \x01(\r\x12\x1e\n\x16zhp_free_refresh_limit\x18\x03 \x01(\r\x12\x1e\n\x16zhp_cost_refresh_limit\x18\x04 \x01(\r\x12\x13\n\x0b\x62uddy_bonus\x18\x05 \x01(\x02\x12\x1c\n\x14record_collect_limit\x18\x06 \x01(\r\";\n\x13NotifyServerSetting\x12$\n\x08settings\x18\x01 \x01(\x0b\x32\x12.lq.ServerSettings\"\xdc\x01\n\x0fNotifyPayResult\x12\x12\n\npay_result\x18\x01 \x01(\r\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x10\n\x08goods_id\x18\x03 \x01(\r\x12\x18\n\x10new_month_ticket\x18\x04 \x01(\r\x12;\n\x0fresource_modify\x18\x05 \x03(\x0b\x32\".lq.NotifyPayResult.ResourceModify\x1a:\n\x0eResourceModify\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\"y\n\x1dNotifyCustomContestAccountMsg\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x0e\n\x06sender\x18\x03 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12\x10\n\x08verified\x18\x05 \x01(\r\"\xb1\x01\n\x1cNotifyCustomContestSystemMsg\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x32\n\ngame_start\x18\x04 \x01(\x0b\x32\x1e.lq.CustomizedContestGameStart\x12.\n\x08game_end\x18\x05 \x01(\x0b\x32\x1c.lq.CustomizedContestGameEnd\"!\n\x12NotifyMatchTimeout\x12\x0b\n\x03sid\x18\x01 \x01(\t\"<\n\x18NotifyCustomContestState\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\"T\n\x14NotifyActivityChange\x12$\n\x0enew_activities\x18\x01 \x03(\x0b\x32\x0c.lq.Activity\x12\x16\n\x0e\x65nd_activities\x18\x02 \x03(\r\"H\n\x0fNotifyAFKResult\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x62\x61n_end_time\x18\x02 \x01(\r\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\"Q\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x12\n\nu32_params\x18\x02 \x03(\r\x12\x12\n\nstr_params\x18\x03 \x03(\t\x12\x12\n\njson_param\x18\x04 \x01(\t\"%\n\x07Wrapper\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"@\n\x0fNetworkEndpoint\x12\x0e\n\x06\x66\x61mily\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x0b\n\tReqCommon\"%\n\tResCommon\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"O\n\x10ResAccountUpdate\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x06update\x18\x02 \x01(\x0b\x32\x11.lq.AccountUpdate\"(\n\rAntiAddiction\x12\x17\n\x0fonline_duration\x18\x01 \x01(\r\"\xcf\x07\n\x17\x41\x63\x63ountMahjongStatistic\x12\x1d\n\x15\x66inal_position_counts\x18\x01 \x03(\r\x12>\n\x0crecent_round\x18\x02 \x01(\x0b\x32(.lq.AccountMahjongStatistic.RoundSummary\x12\x38\n\trecent_hu\x18\x03 \x01(\x0b\x32%.lq.AccountMahjongStatistic.HuSummary\x12?\n\nhighest_hu\x18\x04 \x01(\x0b\x32+.lq.AccountMahjongStatistic.HighestHuRecord\x12G\n\x14recent_20_hu_summary\x18\x06 \x01(\x0b\x32).lq.AccountMahjongStatistic.Liqi20Summary\x12G\n\x14recent_10_hu_summary\x18\x07 \x01(\x0b\x32).lq.AccountMahjongStatistic.LiQi10Summary\x12\x45\n\x15recent_10_game_result\x18\x08 \x03(\x0b\x32&.lq.AccountMahjongStatistic.GameResult\x1a\x64\n\x0cRoundSummary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x12\n\nrong_count\x18\x02 \x01(\r\x12\x12\n\nzimo_count\x18\x03 \x01(\r\x12\x17\n\x0f\x66\x61ngchong_count\x18\x04 \x01(\r\x1aM\n\tHuSummary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x18\n\x10\x64ora_round_count\x18\x02 \x01(\r\x12\x11\n\ttotal_fan\x18\x03 \x01(\r\x1a\x7f\n\x0fHighestHuRecord\x12\x0e\n\x06\x66\x61nshu\x18\x01 \x01(\r\x12\x0f\n\x07\x64oranum\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\t\x12\r\n\x05hands\x18\x04 \x03(\t\x12\x0c\n\x04ming\x18\x05 \x03(\t\x12\r\n\x05hupai\x18\x06 \x01(\t\x12\x10\n\x08title_id\x18\x07 \x01(\r\x1aZ\n\rLiqi20Summary\x12\x13\n\x0btotal_count\x18\x01 \x01(\r\x12\x1a\n\x12total_lidora_count\x18\x02 \x01(\r\x12\x18\n\x10\x61verage_hu_point\x18\x03 \x01(\r\x1a>\n\rLiQi10Summary\x12\x17\n\x0ftotal_xuanshang\x18\x01 \x01(\r\x12\x14\n\x0ctotal_fanshu\x18\x02 \x01(\r\x1a/\n\nGameResult\x12\x0c\n\x04rank\x18\x01 \x01(\r\x12\x13\n\x0b\x66inal_point\x18\x02 \x01(\x05\"\x8a\x01\n\x14\x41\x63\x63ountStatisticData\x12\x18\n\x10mahjong_category\x18\x01 \x01(\r\x12\x15\n\rgame_category\x18\x02 \x01(\r\x12.\n\tstatistic\x18\x03 \x01(\x0b\x32\x1b.lq.AccountMahjongStatistic\x12\x11\n\tgame_type\x18\x04 \x01(\r\")\n\x0c\x41\x63\x63ountLevel\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\r\")\n\x08ViewSlot\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\x0f\n\x07item_id\x18\x02 \x01(\r\"\x84\x07\n\x07\x41\x63\x63ount\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x12\n\nlogin_time\x18\x03 \x01(\r\x12\x13\n\x0blogout_time\x18\x04 \x01(\r\x12\x0f\n\x07room_id\x18\x05 \x01(\r\x12)\n\x0e\x61nti_addiction\x18\x06 \x01(\x0b\x32\x11.lq.AntiAddiction\x12\r\n\x05title\x18\x07 \x01(\r\x12\x11\n\tsignature\x18\x08 \x01(\t\x12\r\n\x05\x65mail\x18\t \x01(\t\x12\x14\n\x0c\x65mail_verify\x18\n \x01(\r\x12\x0c\n\x04gold\x18\x0b \x01(\r\x12\x0f\n\x07\x64iamond\x18\x0c \x01(\r\x12\x11\n\tavatar_id\x18\r \x01(\r\x12\x0b\n\x03vip\x18\x0e \x01(\r\x12\x10\n\x08\x62irthday\x18\x0f \x01(\x05\x12\r\n\x05phone\x18\x10 \x01(\t\x12\x14\n\x0cphone_verify\x18\x11 \x01(\r\x12\x35\n\x10platform_diamond\x18\x12 \x03(\x0b\x32\x1b.lq.Account.PlatformDiamond\x12\x1f\n\x05level\x18\x15 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x16 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x17 \x01(\r\x12\x13\n\x0bskin_ticket\x18\x18 \x01(\r\x12<\n\x14platform_skin_ticket\x18\x19 \x03(\x0b\x32\x1e.lq.Account.PlatformSkinTicket\x12\x10\n\x08verified\x18\x1a \x01(\r\x12\x34\n\x10\x63hallenge_levels\x18\x1b \x03(\x0b\x32\x1a.lq.Account.ChallengeLevel\x12\x37\n\x11\x61\x63hievement_count\x18\x1c \x03(\x0b\x32\x1c.lq.Account.AchievementCount\x1a,\n\x0fPlatformDiamond\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x1a/\n\x12PlatformSkinTicket\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x1a=\n\x0e\x43hallengeLevel\x12\x0e\n\x06season\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0c\n\x04rank\x18\x03 \x01(\r\x1a/\n\x10\x41\x63hievementCount\x12\x0c\n\x04rare\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"-\n\x10\x41\x63\x63ountOwnerData\x12\x19\n\x11unlock_characters\x18\x01 \x03(\r\"\xde\x0c\n\rAccountUpdate\x12\x34\n\tnumerical\x18\x01 \x03(\x0b\x32!.lq.AccountUpdate.NumericalUpdate\x12\x34\n\tcharacter\x18\x02 \x01(\x0b\x32!.lq.AccountUpdate.CharacterUpdate\x12\x1a\n\x03\x62\x61g\x18\x03 \x01(\x0b\x32\r.lq.BagUpdate\x12\x38\n\x0b\x61\x63hievement\x18\x04 \x01(\x0b\x32#.lq.AccountUpdate.AchievementUpdate\x12#\n\x07shilian\x18\x05 \x01(\x0b\x32\x12.lq.AccountShiLian\x12\x35\n\ndaily_task\x18\x06 \x01(\x0b\x32!.lq.AccountUpdate.DailyTaskUpdate\x12,\n\x05title\x18\x07 \x01(\x0b\x32\x1d.lq.AccountUpdate.TitleUpdate\x12\x1a\n\x12new_recharged_list\x18\x08 \x03(\r\x12\x33\n\ractivity_task\x18\t \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12\x38\n\x12\x61\x63tivity_flip_task\x18\n \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12:\n\x14\x61\x63tivity_period_task\x18\x0b \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12:\n\x14\x61\x63tivity_random_task\x18\x0c \x01(\x0b\x32\x1c.lq.AccountUpdate.TaskUpdate\x12;\n\tchallenge\x18\r \x01(\x0b\x32(.lq.AccountUpdate.AccountChallengeUpdate\x12\x38\n\x08\x61\x62_match\x18\x0e \x01(\x0b\x32&.lq.AccountUpdate.AccountABMatchUpdate\x1a,\n\x0fNumericalUpdate\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\x1aw\n\x0f\x43haracterUpdate\x12!\n\ncharacters\x18\x02 \x03(\x0b\x32\r.lq.Character\x12\r\n\x05skins\x18\x03 \x03(\r\x12\x18\n\x10\x66inished_endings\x18\x04 \x03(\r\x12\x18\n\x10rewarded_endings\x18\x05 \x03(\r\x1aX\n\x11\x41\x63hievementUpdate\x12+\n\nprogresses\x18\x01 \x03(\x0b\x32\x17.lq.AchievementProgress\x12\x16\n\x0erewarded_group\x18\x02 \x03(\r\x1aJ\n\x0f\x44\x61ilyTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x11\n\ttask_list\x18\x02 \x03(\r\x1a\x38\n\x0bTitleUpdate\x12\x12\n\nnew_titles\x18\x01 \x03(\r\x12\x15\n\rremove_titles\x18\x02 \x03(\r\x1a\x45\n\nTaskUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x11\n\ttask_list\x18\x02 \x03(\r\x1a\xb8\x01\n\x16\x41\x63\x63ountChallengeUpdate\x12$\n\nprogresses\x18\x01 \x03(\x0b\x32\x10.lq.TaskProgress\x12\r\n\x05level\x18\x02 \x01(\r\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\x13\n\x0bmatch_count\x18\x04 \x01(\r\x12\x11\n\tticket_id\x18\x05 \x01(\r\x12\x11\n\ttask_list\x18\x06 \x03(\r\x12\x17\n\x0frewarded_season\x18\x07 \x03(\r\x1a\xfd\x01\n\x14\x41\x63\x63ountABMatchUpdate\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\x13\n\x0bmatch_count\x18\x02 \x01(\r\x12\x14\n\x0c\x62uy_in_count\x18\x03 \x01(\r\x12\r\n\x05point\x18\x04 \x01(\r\x12\x10\n\x08rewarded\x18\x05 \x01(\x08\x12J\n\x0fmatch_max_point\x18\x06 \x03(\x0b\x32\x31.lq.AccountUpdate.AccountABMatchUpdate.MatchPoint\x12\x0c\n\x04quit\x18\x07 \x01(\x08\x1a-\n\nMatchPoint\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"E\n\x0cGameMetaData\x12\x0f\n\x07room_id\x18\x01 \x01(\r\x12\x0f\n\x07mode_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63ontest_uid\x18\x03 \x01(\r\"Y\n\x12\x41\x63\x63ountPlayingGame\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\r\x12\x1e\n\x04meta\x18\x03 \x01(\x0b\x32\x10.lq.GameMetaData\"\xa2\x03\n\x10\x41\x63\x63ountCacheView\x12\x15\n\rcache_version\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x12\n\nlogin_time\x18\x04 \x01(\r\x12\x13\n\x0blogout_time\x18\x05 \x01(\r\x12\x11\n\tis_online\x18\x06 \x01(\x08\x12\x0f\n\x07room_id\x18\x07 \x01(\r\x12\r\n\x05title\x18\x08 \x01(\r\x12\x11\n\tavatar_id\x18\t \x01(\r\x12\x0b\n\x03vip\x18\n \x01(\r\x12\x1f\n\x05level\x18\x0b \x01(\x0b\x32\x10.lq.AccountLevel\x12,\n\x0cplaying_game\x18\x0c \x01(\x0b\x32\x16.lq.AccountPlayingGame\x12 \n\x06level3\x18\r \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x0e \x01(\r\x12\x10\n\x08verified\x18\x0f \x01(\r\x12\x14\n\x0c\x62\x61n_deadline\x18\x10 \x01(\r\x12\x13\n\x0b\x63omment_ban\x18\x11 \x01(\r\x12\x11\n\tban_state\x18\x12 \x01(\r\"\xd6\x01\n\x0ePlayerBaseView\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x11\n\tavatar_id\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\r\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x1f\n\x05level\x18\x05 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x06 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x07 \x01(\r\x12\x10\n\x08verified\x18\x08 \x01(\r\x12\x11\n\tis_banned\x18\t \x01(\r\"\x82\x02\n\x0ePlayerGameView\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x11\n\tavatar_id\x18\x02 \x01(\r\x12\r\n\x05title\x18\x03 \x01(\r\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x1f\n\x05level\x18\x05 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\tcharacter\x18\x06 \x01(\x0b\x32\r.lq.Character\x12 \n\x06level3\x18\x07 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\x08 \x01(\r\x12\x10\n\x08verified\x18\t \x01(\r\x12\x1b\n\x05views\x18\n \x03(\x0b\x32\x0c.lq.ViewSlot\"#\n\x0bGameSetting\x12\x14\n\x0c\x65moji_switch\x18\x01 \x01(\r\"\xc4\x01\n\x08GameMode\x12\x0c\n\x04mode\x18\x01 \x01(\r\x12\n\n\x02\x61i\x18\x04 \x01(\x08\x12\x12\n\nextendinfo\x18\x05 \x01(\t\x12\'\n\x0b\x64\x65tail_rule\x18\x06 \x01(\x0b\x32\x12.lq.GameDetailRule\x12:\n\x13testing_environment\x18\x07 \x01(\x0b\x32\x1d.lq.GameTestingEnvironmentSet\x12%\n\x0cgame_setting\x18\x08 \x01(\x0b\x32\x0f.lq.GameSetting\"@\n\x19GameTestingEnvironmentSet\x12\x0f\n\x07paixing\x18\x01 \x01(\r\x12\x12\n\nleft_count\x18\x02 \x01(\r\"\xb7\t\n\x0eGameDetailRule\x12\x12\n\ntime_fixed\x18\x01 \x01(\r\x12\x10\n\x08time_add\x18\x02 \x01(\r\x12\x12\n\ndora_count\x18\x03 \x01(\r\x12\x0f\n\x07shiduan\x18\x04 \x01(\r\x12\x12\n\ninit_point\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61ndian\x18\x06 \x01(\r\x12\x11\n\tcan_jifei\x18\x07 \x01(\x08\x12\x16\n\x0etianbian_value\x18\x08 \x01(\r\x12\x16\n\x0eliqibang_value\x18\t \x01(\r\x12\x17\n\x0f\x63hangbang_value\x18\n \x01(\r\x12\x15\n\rnoting_fafu_1\x18\x0b \x01(\r\x12\x15\n\rnoting_fafu_2\x18\x0c \x01(\r\x12\x15\n\rnoting_fafu_3\x18\r \x01(\r\x12\x19\n\x11have_liujumanguan\x18\x0e \x01(\x08\x12\x1c\n\x14have_qieshangmanguan\x18\x0f \x01(\x08\x12\x16\n\x0ehave_biao_dora\x18\x10 \x01(\x08\x12\x1b\n\x13have_gang_biao_dora\x18\x11 \x01(\x08\x12\"\n\x1aming_dora_immediately_open\x18\x12 \x01(\x08\x12\x14\n\x0chave_li_dora\x18\x13 \x01(\x08\x12\x19\n\x11have_gang_li_dora\x18\x14 \x01(\x08\x12\x19\n\x11have_sifenglianda\x18\x15 \x01(\x08\x12\x18\n\x10have_sigangsanle\x18\x16 \x01(\x08\x12\x17\n\x0fhave_sijializhi\x18\x17 \x01(\x08\x12\x1b\n\x13have_jiuzhongjiupai\x18\x18 \x01(\x08\x12\x17\n\x0fhave_sanjiahele\x18\x19 \x01(\x08\x12\x14\n\x0chave_toutiao\x18\x1a \x01(\x08\x12\x1b\n\x13have_helelianzhuang\x18\x1b \x01(\x08\x12\x18\n\x10have_helezhongju\x18\x1c \x01(\x08\x12\x1e\n\x16have_tingpailianzhuang\x18\x1d \x01(\x08\x12\x1b\n\x13have_tingpaizhongju\x18\x1e \x01(\x08\x12\x11\n\thave_yifa\x18\x1f \x01(\x08\x12\x16\n\x0ehave_nanruxiru\x18  \x01(\x08\x12\x18\n\x10jingsuanyuandian\x18! \x01(\r\x12\x13\n\x0bshunweima_2\x18\" \x01(\x05\x12\x13\n\x0bshunweima_3\x18# \x01(\x05\x12\x13\n\x0bshunweima_4\x18$ \x01(\x05\x12\x14\n\x0c\x62ianjietishi\x18% \x01(\x08\x12\x10\n\x08\x61i_level\x18& \x01(\r\x12\x14\n\x0chave_zimosun\x18\' \x01(\x08\x12\x1d\n\x15\x64isable_multi_yukaman\x18( \x01(\x08\x12\r\n\x05\x66\x61nfu\x18) \x01(\r\x12\x11\n\tguyi_mode\x18* \x01(\r\x12\x12\n\ndora3_mode\x18+ \x01(\r\x12\x17\n\x0f\x62\x65gin_open_mode\x18, \x01(\r\x12\x14\n\x0cjiuchao_mode\x18- \x01(\r\x12\x11\n\tmuyu_mode\x18. \x01(\r\x12\x11\n\topen_hand\x18/ \x01(\r\x12\x14\n\x0cxuezhandaodi\x18\x30 \x01(\r\x12\x14\n\x0chuansanzhang\x18\x31 \x01(\r\x12\x0f\n\x07\x63huanma\x18\x32 \x01(\r\x12\x1a\n\x12\x64isable_leijiyiman\x18< \x01(\x08\"\xfa\x01\n\x04Room\x12\x0f\n\x07room_id\x18\x01 \x01(\r\x12\x10\n\x08owner_id\x18\x02 \x01(\r\x12\x1a\n\x04mode\x18\x03 \x01(\x0b\x32\x0c.lq.GameMode\x12\x18\n\x10max_player_count\x18\x04 \x01(\r\x12#\n\x07persons\x18\x05 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x12\n\nready_list\x18\x06 \x03(\r\x12\x12\n\nis_playing\x18\x07 \x01(\x08\x12\x13\n\x0bpublic_live\x18\x08 \x01(\x08\x12\x13\n\x0brobot_count\x18\t \x01(\r\x12\x15\n\rtournament_id\x18\n \x01(\r\x12\x0b\n\x03seq\x18\x0b \x01(\r\"\xc1\x01\n\rGameEndResult\x12-\n\x07players\x18\x01 \x03(\x0b\x32\x1c.lq.GameEndResult.PlayerItem\x1a\x80\x01\n\nPlayerItem\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x13\n\x0btotal_point\x18\x02 \x01(\x05\x12\x14\n\x0cpart_point_1\x18\x03 \x01(\x05\x12\x14\n\x0cpart_point_2\x18\x04 \x01(\x05\x12\x15\n\rgrading_score\x18\x05 \x01(\x05\x12\x0c\n\x04gold\x18\x06 \x01(\x05\"M\n\x0fGameConnectInfo\x12\x15\n\rconnect_token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\"0\n\x0eItemGainRecord\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"d\n\x0fItemGainRecords\x12\x13\n\x0brecord_time\x18\x01 \x01(\r\x12\x17\n\x0flimit_source_id\x18\x02 \x01(\r\x12#\n\x07records\x18\x03 \x03(\x0b\x32\x12.lq.ItemGainRecord\"&\n\x04Item\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05stack\x18\x02 \x01(\r\"N\n\x03\x42\x61g\x12\x17\n\x05items\x18\x01 \x03(\x0b\x32\x08.lq.Item\x12.\n\x11\x64\x61ily_gain_record\x18\x02 \x03(\x0b\x32\x13.lq.ItemGainRecords\"b\n\tBagUpdate\x12\x1e\n\x0cupdate_items\x18\x01 \x03(\x0b\x32\x08.lq.Item\x12\x35\n\x18update_daily_gain_record\x18\x02 \x03(\x0b\x32\x13.lq.ItemGainRecords\"\'\n\nRewardSlot\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"M\n\nOpenResult\x12\x1e\n\x06reward\x18\x01 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x1f\n\x07replace\x18\x02 \x01(\x0b\x32\x0e.lq.RewardSlot\"\x97\x01\n\x10RewardPlusResult\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12/\n\x08\x65xchange\x18\x03 \x01(\x0b\x32\x1d.lq.RewardPlusResult.Exchange\x1a\x37\n\x08\x45xchange\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x10\n\x08\x65xchange\x18\x03 \x01(\r\"g\n\rExecuteReward\x12\x1e\n\x06reward\x18\x01 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x1f\n\x07replace\x18\x02 \x01(\x0b\x32\x0e.lq.RewardSlot\x12\x15\n\rreplace_count\x18\x03 \x01(\r\"\xc8\x02\n\x04Mail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\x12\x17\n\x0ftake_attachment\x18\x03 \x01(\x08\x12\r\n\x05title\x18\x04 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x05 \x01(\t\x12#\n\x0b\x61ttachments\x18\x06 \x03(\x0b\x32\x0e.lq.RewardSlot\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\r\x12\x13\n\x0b\x65xpire_time\x18\x08 \x01(\r\x12\x14\n\x0creference_id\x18\t \x01(\r\x12(\n\ntitle_i18n\x18\n \x03(\x0b\x32\x14.lq.Mail.I18nContext\x12*\n\x0c\x63ontent_i18n\x18\x0b \x03(\x0b\x32\x14.lq.Mail.I18nContext\x1a,\n\x0bI18nContext\x12\x0c\n\x04lang\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontext\x18\x02 \x01(\t\"m\n\x13\x41\x63hievementProgress\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ounter\x18\x02 \x01(\r\x12\x10\n\x08\x61\x63hieved\x18\x03 \x01(\x08\x12\x10\n\x08rewarded\x18\x04 \x01(\x08\x12\x15\n\rachieved_time\x18\x05 \x01(\r\"\x97\x04\n\x1a\x41\x63\x63ountStatisticByGameMode\x12\x0c\n\x04mode\x18\x01 \x01(\r\x12\x16\n\x0egame_count_sum\x18\x02 \x01(\r\x12\x1b\n\x13game_final_position\x18\x03 \x03(\r\x12\x11\n\tfly_count\x18\x04 \x01(\r\x12\x15\n\rgold_earn_sum\x18\x05 \x01(\x02\x12\x17\n\x0fround_count_sum\x18\x06 \x01(\r\x12\x12\n\ndadian_sum\x18\x07 \x01(\x02\x12>\n\tround_end\x18\x08 \x03(\x0b\x32+.lq.AccountStatisticByGameMode.RoundEndData\x12\x16\n\x0eming_count_sum\x18\t \x01(\r\x12\x16\n\x0eliqi_count_sum\x18\n \x01(\r\x12\x15\n\rxun_count_sum\x18\x0b \x01(\r\x12\x1a\n\x12highest_lianzhuang\x18\x0c \x01(\r\x12\x16\n\x0escore_earn_sum\x18\r \x01(\r\x12<\n\nrank_score\x18\x0e \x03(\x0b\x32(.lq.AccountStatisticByGameMode.RankScore\x1a)\n\x0cRoundEndData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0b\n\x03sum\x18\x02 \x01(\r\x1a;\n\tRankScore\x12\x0c\n\x04rank\x18\x01 \x01(\r\x12\x11\n\tscore_sum\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"4\n\x15\x41\x63\x63ountStatisticByFan\x12\x0e\n\x06\x66\x61n_id\x18\x01 \x01(\r\x12\x0b\n\x03sum\x18\x02 \x01(\r\"l\n\x12\x41\x63\x63ountFanAchieved\x12\x18\n\x10mahjong_category\x18\x01 \x01(\r\x12&\n\x03\x66\x61n\x18\x02 \x03(\x0b\x32\x19.lq.AccountStatisticByFan\x12\x14\n\x0cliujumanguan\x18\x03 \x01(\r\"\xb7\x01\n\x16\x41\x63\x63ountDetailStatistic\x12\x31\n\tgame_mode\x18\x01 \x03(\x0b\x32\x1e.lq.AccountStatisticByGameMode\x12&\n\x03\x66\x61n\x18\x02 \x03(\x0b\x32\x19.lq.AccountStatisticByFan\x12\x14\n\x0cliujumanguan\x18\x03 \x01(\r\x12,\n\x0c\x66\x61n_achieved\x18\x04 \x03(\x0b\x32\x16.lq.AccountFanAchieved\"j\n AccountDetailStatisticByCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\r\x12\x34\n\x10\x64\x65tail_statistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\"\xd1\n\n\x18\x41\x63\x63ountDetailStatisticV2\x12\x39\n\x15\x66riend_room_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x42\n\x0erank_statistic\x18\x02 \x01(\x0b\x32*.lq.AccountDetailStatisticV2.RankStatistic\x12]\n\x1c\x63ustomized_contest_statistic\x18\x03 \x01(\x0b\x32\x37.lq.AccountDetailStatisticV2.CustomizedContestStatistic\x12;\n\x17leisure_match_statistic\x18\x04 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12R\n\x19\x63hallenge_match_statistic\x18\x05 \x01(\x0b\x32/.lq.AccountDetailStatisticV2.ChallengeStatistic\x12<\n\x18\x61\x63tivity_match_statistic\x18\x06 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x36\n\x12\x61\x62_match_statistic\x18\x07 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x1a\xbd\x03\n\rRankStatistic\x12L\n\x0ftotal_statistic\x18\x01 \x01(\x0b\x32\x33.lq.AccountDetailStatisticV2.RankStatistic.RankData\x12L\n\x0fmonth_statistic\x18\x02 \x01(\x0b\x32\x33.lq.AccountDetailStatisticV2.RankStatistic.RankData\x12\x1a\n\x12month_refresh_time\x18\x03 \x01(\r\x1a\xf3\x01\n\x08RankData\x12\x37\n\x13\x61ll_level_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12Z\n\x0flevel_data_list\x18\x02 \x03(\x0b\x32\x41.lq.AccountDetailStatisticV2.RankStatistic.RankData.RankLevelData\x1aR\n\rRankLevelData\x12\x12\n\nrank_level\x18\x01 \x01(\r\x12-\n\tstatistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x1a\xa2\x01\n\x1a\x43ustomizedContestStatistic\x12\x33\n\x0ftotal_statistic\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x33\n\x0fmonth_statistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12\x1a\n\x12month_refresh_time\x18\x03 \x01(\r\x1a\xea\x01\n\x12\x43hallengeStatistic\x12.\n\nall_season\x18\x01 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\x12T\n\x10season_data_list\x18\x02 \x03(\x0b\x32:.lq.AccountDetailStatisticV2.ChallengeStatistic.SeasonData\x1aN\n\nSeasonData\x12\x11\n\tseason_id\x18\x01 \x01(\r\x12-\n\tstatistic\x18\x02 \x01(\x0b\x32\x1a.lq.AccountDetailStatistic\"-\n\x0e\x41\x63\x63ountShiLian\x12\x0c\n\x04step\x18\x01 \x01(\r\x12\r\n\x05state\x18\x02 \x01(\r\"\xc2\x01\n\x10\x43lientDeviceInfo\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x10\n\x08hardware\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x12\n\nos_version\x18\x04 \x01(\t\x12\x12\n\nis_browser\x18\x05 \x01(\x08\x12\x10\n\x08software\x18\x06 \x01(\t\x12\x15\n\rsale_platform\x18\x07 \x01(\t\x12\x17\n\x0fhardware_vendor\x18\x08 \x01(\t\x12\x14\n\x0cmodel_number\x18\t \x01(\t\"6\n\x11\x43lientVersionInfo\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\x0f\n\x07package\x18\x02 \x01(\t\":\n\x0c\x41nnouncement\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"_\n\x0cTaskProgress\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ounter\x18\x02 \x01(\r\x12\x10\n\x08\x61\x63hieved\x18\x03 \x01(\x08\x12\x10\n\x08rewarded\x18\x04 \x01(\x08\x12\x0e\n\x06\x66\x61iled\x18\x05 \x01(\x08\"Z\n\nGameConfig\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\r\x12\x1a\n\x04mode\x18\x02 \x01(\x0b\x32\x0c.lq.GameMode\x12\x1e\n\x04meta\x18\x03 \x01(\x0b\x32\x10.lq.GameMetaData\"\x8d\x01\n\x12\x41\x63\x63ountActiveState\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\nlogin_time\x18\x02 \x01(\r\x12\x13\n\x0blogout_time\x18\x03 \x01(\r\x12\x11\n\tis_online\x18\x04 \x01(\x08\x12\'\n\x07playing\x18\x05 \x01(\x0b\x32\x16.lq.AccountPlayingGame\"Q\n\x06\x46riend\x12 \n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12%\n\x05state\x18\x02 \x01(\x0b\x32\x16.lq.AccountActiveState\"O\n\x0cGameLiveUnit\x12\x11\n\ttimestamp\x18\x01 \x01(\r\x12\x17\n\x0f\x61\x63tion_category\x18\x02 \x01(\r\x12\x13\n\x0b\x61\x63tion_data\x18\x03 \x01(\x0c\"4\n\x0fGameLiveSegment\x12!\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x10.lq.GameLiveUnit\"=\n\x12GameLiveSegmentUri\x12\x12\n\nsegment_id\x18\x01 \x01(\r\x12\x13\n\x0bsegment_uri\x18\x02 \x01(\t\"\x8d\x01\n\x0cGameLiveHead\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12#\n\x0bgame_config\x18\x03 \x01(\x0b\x32\x0e.lq.GameConfig\x12#\n\x07players\x18\x04 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x11\n\tseat_list\x18\x05 \x03(\r\"(\n\x11GameNewRoundState\x12\x13\n\x0bseat_states\x18\x01 \x03(\r\"\x1e\n\rGameEndAction\x12\r\n\x05state\x18\x01 \x01(\r\"\x10\n\x0eGameNoopAction\"\x7f\n\x0b\x43ommentItem\x12\x12\n\ncomment_id\x18\x01 \x01(\r\x12\x11\n\ttimestamp\x18\x02 \x01(\r\x12%\n\tcommenter\x18\x03 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12\x11\n\tis_banned\x18\x05 \x01(\r\"y\n\rRollingNotice\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\x12\x17\n\x0frepeat_interval\x18\x05 \x01(\r\x12\x0c\n\x04lang\x18\x06 \x01(\t\"q\n\x0c\x42illingGoods\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\x13\n\x0bresource_id\x18\x05 \x01(\r\x12\x16\n\x0eresource_count\x18\x06 \x01(\r\"<\n\x0c\x42illShortcut\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tdealPrice\x18\x03 \x01(\r\"u\n\x0e\x42illingProduct\x12\x1f\n\x05goods\x18\x01 \x01(\x0b\x32\x10.lq.BillingGoods\x12\x15\n\rcurrency_code\x18\x02 \x01(\t\x12\x16\n\x0e\x63urrency_price\x18\x03 \x01(\r\x12\x13\n\x0bsort_weight\x18\x04 \x01(\r\"\x8c\x01\n\tCharacter\x12\x0e\n\x06\x63harid\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0b\n\x03\x65xp\x18\x03 \x01(\r\x12\x1b\n\x05views\x18\x04 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\x0c\n\x04skin\x18\x05 \x01(\r\x12\x13\n\x0bis_upgraded\x18\x06 \x01(\x08\x12\x13\n\x0b\x65xtra_emoji\x18\x07 \x03(\r\"&\n\tBuyRecord\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\xca\x01\n\x07ZHPShop\x12\r\n\x05goods\x18\x01 \x03(\r\x12\"\n\x0b\x62uy_records\x18\x02 \x03(\x0b\x32\r.lq.BuyRecord\x12.\n\x0c\x66ree_refresh\x18\x03 \x01(\x0b\x32\x18.lq.ZHPShop.RefreshCount\x12.\n\x0c\x63ost_refresh\x18\x04 \x01(\x0b\x32\x18.lq.ZHPShop.RefreshCount\x1a,\n\x0cRefreshCount\x12\r\n\x05\x63ount\x18\x01 \x01(\r\x12\r\n\x05limit\x18\x02 \x01(\r\"F\n\x0fMonthTicketInfo\x12\n\n\x02id\x18\x01 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\r\x12\x15\n\rlast_pay_time\x18\x03 \x01(\r\"c\n\x08ShopInfo\x12\x18\n\x03zhp\x18\x01 \x01(\x0b\x32\x0b.lq.ZHPShop\x12\"\n\x0b\x62uy_records\x18\x02 \x03(\x0b\x32\r.lq.BuyRecord\x12\x19\n\x11last_refresh_time\x18\x03 \x01(\r\">\n\x14\x43hangeNicknameRecord\x12\x0c\n\x04\x66rom\x18\x01 \x01(\t\x12\n\n\x02to\x18\x02 \x01(\t\x12\x0c\n\x04time\x18\x03 \x01(\r\"o\n\x0eServerSettings\x12+\n\x0fpayment_setting\x18\x03 \x01(\x0b\x32\x12.lq.PaymentSetting\x12\x30\n\x12payment_setting_v2\x18\x04 \x01(\x0b\x32\x14.lq.PaymentSettingV2\"\x83\x03\n\x10PaymentSettingV2\x12\x14\n\x0copen_payment\x18\x01 \x01(\r\x12\x42\n\x11payment_platforms\x18\x02 \x03(\x0b\x32\'.lq.PaymentSettingV2.PaymentSettingUnit\x1am\n\x0fPaymentMaintain\x12\x12\n\nstart_time\x18\x01 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\r\x12\x1a\n\x12goods_click_action\x18\x03 \x01(\r\x12\x18\n\x10goods_click_text\x18\x04 \x01(\t\x1a\xa5\x01\n\x12PaymentSettingUnit\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0f\n\x07is_show\x18\x02 \x01(\x08\x12\x1a\n\x12goods_click_action\x18\x03 \x01(\r\x12\x18\n\x10goods_click_text\x18\x04 \x01(\t\x12\x36\n\x08maintain\x18\x05 \x01(\x0b\x32$.lq.PaymentSettingV2.PaymentMaintain\"\xdf\x02\n\x0ePaymentSetting\x12\x14\n\x0copen_payment\x18\x01 \x01(\r\x12\x1e\n\x16payment_info_show_type\x18\x02 \x01(\r\x12\x14\n\x0cpayment_info\x18\x03 \x01(\t\x12-\n\x06wechat\x18\x04 \x01(\x0b\x32\x1d.lq.PaymentSetting.WechatData\x12-\n\x06\x61lipay\x18\x05 \x01(\x0b\x32\x1d.lq.PaymentSetting.AlipayData\x1a\\\n\nWechatData\x12\x16\n\x0e\x64isable_create\x18\x01 \x01(\x08\x12\x1f\n\x17payment_source_platform\x18\x02 \x01(\r\x12\x15\n\renable_credit\x18\x03 \x01(\x08\x1a\x45\n\nAlipayData\x12\x16\n\x0e\x64isable_create\x18\x01 \x01(\x08\x12\x1f\n\x17payment_source_platform\x18\x02 \x01(\r\",\n\x0e\x41\x63\x63ountSetting\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"h\n\tChestData\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x18\n\x10\x66\x61\x63\x65_black_count\x18\x04 \x01(\r\"S\n\x0b\x43hestDataV2\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x18\n\x10\x66\x61\x63\x65_black_count\x18\x03 \x01(\r\"d\n\tFaithData\x12\x10\n\x08\x66\x61ith_id\x18\x01 \x01(\r\x12\x18\n\x10total_open_count\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x14\n\x0cmodify_count\x18\x04 \x01(\x05\"\xd9\x01\n\x15\x43ustomizedContestBase\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x14\n\x0c\x63ontest_type\x18\n \x01(\r\"C\n\x17\x43ustomizedContestExtend\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x15\n\rpublic_notice\x18\x02 \x01(\t\"\xde\x01\n\x19\x43ustomizedContestAbstract\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x15\n\rpublic_notice\x18\n \x01(\t\"\xc0\x02\n\x17\x43ustomizedContestDetail\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\ncontest_id\x18\x02 \x01(\r\x12\x14\n\x0c\x63ontest_name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\r\x12\x12\n\ncreator_id\x18\x05 \x01(\r\x12\x13\n\x0b\x63reate_time\x18\x06 \x01(\r\x12\x12\n\nstart_time\x18\x07 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\x08 \x01(\r\x12\x0c\n\x04open\x18\t \x01(\x08\x12\x11\n\trank_rule\x18\n \x01(\r\x12\x1f\n\tgame_mode\x18\x0b \x01(\x0b\x32\x0c.lq.GameMode\x12\x16\n\x0eprivate_notice\x18\x0c \x01(\t\x12\x17\n\x0fobserver_switch\x18\r \x01(\r\x12\x14\n\x0c\x65moji_switch\x18\x0e \x01(\r\"}\n\x1d\x43ustomizedContestPlayerReport\x12\x11\n\trank_rule\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12\r\n\x05point\x18\x03 \x01(\x05\x12\x12\n\ngame_ranks\x18\x04 \x03(\r\x12\x18\n\x10total_game_count\x18\x05 \x01(\r\"\xc1\x03\n\nRecordGame\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\x1e\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x0e.lq.GameConfig\x12,\n\x08\x61\x63\x63ounts\x18\x0b \x03(\x0b\x32\x1a.lq.RecordGame.AccountInfo\x12!\n\x06result\x18\x0c \x01(\x0b\x32\x11.lq.GameEndResult\x1a\x8d\x02\n\x0b\x41\x63\x63ountInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04seat\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x11\n\tavatar_id\x18\x04 \x01(\r\x12 \n\tcharacter\x18\x05 \x01(\x0b\x32\r.lq.Character\x12\r\n\x05title\x18\x06 \x01(\r\x12\x1f\n\x05level\x18\x07 \x01(\x0b\x32\x10.lq.AccountLevel\x12 \n\x06level3\x18\x08 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x14\n\x0c\x61vatar_frame\x18\t \x01(\r\x12\x10\n\x08verified\x18\n \x01(\r\x12\x1b\n\x05views\x18\x0b \x03(\x0b\x32\x0c.lq.ViewSlot\"\x80\x01\n\x1a\x43ustomizedContestGameStart\x12\x34\n\x07players\x18\x01 \x03(\x0b\x32#.lq.CustomizedContestGameStart.Item\x1a,\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x91\x01\n\x18\x43ustomizedContestGameEnd\x12\x32\n\x07players\x18\x01 \x03(\x0b\x32!.lq.CustomizedContestGameEnd.Item\x1a\x41\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x13\n\x0btotal_point\x18\x03 \x01(\x05\"S\n\x08\x41\x63tivity\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\x0c\n\x04type\x18\x04 \x01(\t\"4\n\x0e\x45xchangeRecord\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"^\n\x1c\x41\x63tivityAccumulatedPointData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\x05\x12\x1a\n\x12gained_reward_list\x18\x03 \x03(\r\"l\n\x15\x41\x63tivityRankPointData\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\x05\x12\x15\n\rgained_reward\x18\x03 \x01(\x08\x12\x15\n\rgainable_time\x18\x04 \x01(\r\"\xa1\x03\n\x0fGameRoundHuData\x12(\n\x05hupai\x18\x01 \x01(\x0b\x32\x19.lq.GameRoundHuData.HuPai\x12%\n\x04\x66\x61ns\x18\x02 \x03(\x0b\x32\x17.lq.GameRoundHuData.Fan\x12\r\n\x05score\x18\x03 \x01(\r\x12\x0b\n\x03xun\x18\x04 \x01(\r\x12\x10\n\x08title_id\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61n_sum\x18\x06 \x01(\r\x12\x0e\n\x06\x66u_sum\x18\x07 \x01(\r\x12\x15\n\ryakuman_count\x18\x08 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\t \x01(\r\x12\x16\n\x0ered_dora_count\x18\n \x01(\r\x12\x15\n\rli_dora_count\x18\x0b \x01(\r\x12\x13\n\x0b\x62\x61\x62\x65i_count\x18\x0c \x01(\r\x12\x18\n\x10xuan_shang_count\x18\r \x01(\r\x1a\x31\n\x05HuPai\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0c\n\x04seat\x18\x02 \x01(\r\x12\x0c\n\x04liqi\x18\x03 \x01(\r\x1a-\n\x03\x46\x61n\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x0b\n\x03\x66\x61n\x18\x03 \x01(\r\"\xb5\x01\n\x15GameRoundPlayerResult\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05hands\x18\x02 \x03(\t\x12\x0c\n\x04ming\x18\x03 \x03(\t\x12\x11\n\tliqi_type\x18\x04 \x01(\r\x12\x0f\n\x07is_fulu\x18\x05 \x01(\x08\x12\x17\n\x0fis_liujumanguan\x18\x06 \x01(\x08\x12\x13\n\x0blian_zhuang\x18\x07 \x01(\r\x12\x1f\n\x02hu\x18\x08 \x01(\x0b\x32\x13.lq.GameRoundHuData\"Y\n\x0fGameRoundPlayer\x12\r\n\x05score\x18\x01 \x01(\x05\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12)\n\x06result\x18\x03 \x01(\x0b\x32\x19.lq.GameRoundPlayerResult\"R\n\x11GameRoundSnapshot\x12\n\n\x02ju\x18\x01 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x02 \x01(\r\x12$\n\x07players\x18\x03 \x03(\x0b\x32\x13.lq.GameRoundPlayer\"\x92\x07\n\x11GameFinalSnapshot\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\r\x12\x10\n\x08\x63\x61tegory\x18\x03 \x01(\r\x12\x1a\n\x04mode\x18\x04 \x01(\x0b\x32\x0c.lq.GameMode\x12\x1e\n\x04meta\x18\x05 \x01(\x0b\x32\x10.lq.GameMetaData\x12=\n\x0f\x63\x61lculate_param\x18\x06 \x01(\x0b\x32$.lq.GameFinalSnapshot.CalculateParam\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\r\x12\x12\n\nstart_time\x18\x08 \x01(\r\x12\x13\n\x0b\x66inish_time\x18\t \x01(\r\x12-\n\x05seats\x18\n \x03(\x0b\x32\x1e.lq.GameFinalSnapshot.GameSeat\x12%\n\x06rounds\x18\x0b \x03(\x0b\x32\x15.lq.GameRoundSnapshot\x12)\n\raccount_views\x18\x0c \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x38\n\rfinal_players\x18\r \x03(\x0b\x32!.lq.GameFinalSnapshot.FinalPlayer\x12/\n\x08\x61\x66k_info\x18\x0e \x03(\x0b\x32\x1d.lq.GameFinalSnapshot.AFKInfo\x1aS\n\x0e\x43\x61lculateParam\x12\x12\n\ninit_point\x18\x01 \x01(\r\x12\x18\n\x10jingsuanyuandian\x18\x02 \x01(\r\x12\x13\n\x0brank_points\x18\x03 \x03(\x05\x1a\x88\x01\n\x08GameSeat\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12,\n\x0fnotify_endpoint\x18\x03 \x01(\x0b\x32\x13.lq.NetworkEndpoint\x12\x16\n\x0e\x63lient_address\x18\x04 \x01(\t\x12\x14\n\x0cis_connected\x18\x05 \x01(\x08\x1a\x81\x01\n\x0b\x46inalPlayer\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x13\n\x0btotal_point\x18\x02 \x01(\x05\x12\x14\n\x0cpart_point_1\x18\x03 \x01(\x05\x12\x14\n\x0cpart_point_2\x18\x04 \x01(\x05\x12\x15\n\rgrading_score\x18\x05 \x01(\x05\x12\x0c\n\x04gold\x18\x06 \x01(\x05\x1a\x45\n\x07\x41\x46KInfo\x12\x17\n\x0f\x64\x65\x61l_tile_count\x18\x01 \x01(\r\x12\x13\n\x0bmoqie_count\x18\x02 \x01(\r\x12\x0c\n\x04seat\x18\x03 \x01(\r\"Z\n\x13RecordCollectedData\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\"\xba\x07\n\x11\x43ontestDetailRule\x12\x12\n\ninit_point\x18\x05 \x01(\r\x12\x0f\n\x07\x66\x61ndian\x18\x06 \x01(\r\x12\x11\n\tcan_jifei\x18\x07 \x01(\x08\x12\x16\n\x0etianbian_value\x18\x08 \x01(\r\x12\x16\n\x0eliqibang_value\x18\t \x01(\r\x12\x17\n\x0f\x63hangbang_value\x18\n \x01(\r\x12\x15\n\rnoting_fafu_1\x18\x0b \x01(\r\x12\x15\n\rnoting_fafu_2\x18\x0c \x01(\r\x12\x15\n\rnoting_fafu_3\x18\r \x01(\r\x12\x19\n\x11have_liujumanguan\x18\x0e \x01(\x08\x12\x1c\n\x14have_qieshangmanguan\x18\x0f \x01(\x08\x12\x16\n\x0ehave_biao_dora\x18\x10 \x01(\x08\x12\x1b\n\x13have_gang_biao_dora\x18\x11 \x01(\x08\x12\"\n\x1aming_dora_immediately_open\x18\x12 \x01(\x08\x12\x14\n\x0chave_li_dora\x18\x13 \x01(\x08\x12\x19\n\x11have_gang_li_dora\x18\x14 \x01(\x08\x12\x19\n\x11have_sifenglianda\x18\x15 \x01(\x08\x12\x18\n\x10have_sigangsanle\x18\x16 \x01(\x08\x12\x17\n\x0fhave_sijializhi\x18\x17 \x01(\x08\x12\x1b\n\x13have_jiuzhongjiupai\x18\x18 \x01(\x08\x12\x17\n\x0fhave_sanjiahele\x18\x19 \x01(\x08\x12\x14\n\x0chave_toutiao\x18\x1a \x01(\x08\x12\x1b\n\x13have_helelianzhuang\x18\x1b \x01(\x08\x12\x18\n\x10have_helezhongju\x18\x1c \x01(\x08\x12\x1e\n\x16have_tingpailianzhuang\x18\x1d \x01(\x08\x12\x1b\n\x13have_tingpaizhongju\x18\x1e \x01(\x08\x12\x11\n\thave_yifa\x18\x1f \x01(\x08\x12\x16\n\x0ehave_nanruxiru\x18  \x01(\x08\x12\x18\n\x10jingsuanyuandian\x18! \x01(\r\x12\x13\n\x0bshunweima_2\x18\" \x01(\x05\x12\x13\n\x0bshunweima_3\x18# \x01(\x05\x12\x13\n\x0bshunweima_4\x18$ \x01(\x05\x12\x14\n\x0c\x62ianjietishi\x18% \x01(\x08\x12\x10\n\x08\x61i_level\x18& \x01(\r\x12\x14\n\x0chave_zimosun\x18\' \x01(\x08\x12\x1d\n\x15\x64isable_multi_yukaman\x18( \x01(\x08\x12\x11\n\tguyi_mode\x18) \x01(\r\x12\x1a\n\x12\x64isable_leijiyiman\x18* \x01(\x08\"\xb3\x01\n\x13\x43ontestDetailRuleV2\x12(\n\tgame_rule\x18\x01 \x01(\x0b\x32\x15.lq.ContestDetailRule\x12\x35\n\nextra_rule\x18\x02 \x01(\x0b\x32!.lq.ContestDetailRuleV2.ExtraRule\x1a;\n\tExtraRule\x12\x16\n\x0erequired_level\x18\x01 \x01(\r\x12\x16\n\x0emax_game_count\x18\x02 \x01(\r\"\xab\x01\n\x0fGameRuleSetting\x12\x12\n\nround_type\x18\x01 \x01(\r\x12\x0f\n\x07shiduan\x18\x02 \x01(\x08\x12\x12\n\ndora_count\x18\x03 \x01(\r\x12\x15\n\rthinking_type\x18\x04 \x01(\r\x12\x17\n\x0fuse_detail_rule\x18\x05 \x01(\x08\x12/\n\x0e\x64\x65tail_rule_v2\x18\x06 \x01(\x0b\x32\x17.lq.ContestDetailRuleV2\"\xad\x01\n\x11RecordTingPaiInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0e\n\x06haveyi\x18\x02 \x01(\x08\x12\r\n\x05yiman\x18\x03 \x01(\x08\x12\r\n\x05\x63ount\x18\x04 \x01(\r\x12\n\n\x02\x66u\x18\x05 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\x06 \x01(\r\x12\x12\n\nyiman_zimo\x18\x07 \x01(\x08\x12\x12\n\ncount_zimo\x18\x08 \x01(\r\x12\x0f\n\x07\x66u_zimo\x18\t \x01(\r\"m\n\x16RecordNoTilePlayerInfo\x12\x0f\n\x07tingpai\x18\x03 \x01(\x08\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12$\n\x05tings\x18\x05 \x03(\x0b\x32\x15.lq.RecordTingPaiInfo\x12\x0e\n\x06liuman\x18\x06 \x01(\x08\"\xb8\x03\n\x0eRecordHuleInfo\x12\x0c\n\x04hand\x18\x01 \x03(\t\x12\x0c\n\x04ming\x18\x02 \x03(\t\x12\x0f\n\x07hu_tile\x18\x03 \x01(\t\x12\x0c\n\x04seat\x18\x04 \x01(\r\x12\x0c\n\x04zimo\x18\x05 \x01(\x08\x12\x0e\n\x06qinjia\x18\x06 \x01(\x08\x12\x0c\n\x04liqi\x18\x07 \x01(\x08\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08li_doras\x18\t \x03(\t\x12\r\n\x05yiman\x18\n \x01(\x08\x12\r\n\x05\x63ount\x18\x0b \x01(\r\x12.\n\x04\x66\x61ns\x18\x0c \x03(\x0b\x32 .lq.RecordHuleInfo.RecordFanInfo\x12\n\n\x02\x66u\x18\r \x01(\r\x12\x16\n\x0epoint_zimo_qin\x18\x0e \x01(\r\x12\x17\n\x0fpoint_zimo_xian\x18\x0f \x01(\r\x12\x10\n\x08title_id\x18\x10 \x01(\r\x12\x11\n\tpoint_sum\x18\x11 \x01(\r\x12\x0e\n\x06\x64\x61\x64ian\x18\x12 \x01(\r\x12\x14\n\x0cis_jue_zhang\x18\x13 \x01(\x08\x12\x0b\n\x03xun\x18\x14 \x01(\r\x12\x11\n\tting_type\x18\x15 \x01(\r\x1a(\n\rRecordFanInfo\x12\x0b\n\x03val\x18\x01 \x01(\r\x12\n\n\x02id\x18\x02 \x01(\r\"B\n\x0fRecordHulesInfo\x12\x0c\n\x04seat\x18\x01 \x01(\x05\x12!\n\x05hules\x18\x02 \x03(\x0b\x32\x12.lq.RecordHuleInfo\"-\n\x0fRecordLiujuInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\"U\n\x10RecordNoTileInfo\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12+\n\x07players\x18\x02 \x03(\x0b\x32\x1a.lq.RecordNoTilePlayerInfo\"r\n\x0eRecordLiqiInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\r\x12\x0c\n\x04is_w\x18\x03 \x01(\x08\x12\x14\n\x0cis_zhen_ting\x18\x04 \x01(\x08\x12\x0b\n\x03xun\x18\x05 \x01(\r\x12\x12\n\nis_success\x18\x06 \x01(\x08\"W\n\x0eRecordGangInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0b\n\x03pai\x18\x03 \x01(\t\x12\x0f\n\x07is_dora\x18\x04 \x01(\x08\x12\x0b\n\x03xun\x18\x05 \x01(\r\"S\n\x0fRecordBaBeiInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x10\n\x08is_zi_mo\x18\x02 \x01(\x08\x12\x10\n\x08is_chong\x18\x03 \x01(\x08\x12\x0e\n\x06is_bei\x18\x04 \x01(\x08\"O\n\x10RecordPeiPaiInfo\x12\x12\n\ndora_count\x18\x01 \x01(\r\x12\x14\n\x0cr_dora_count\x18\x02 \x01(\r\x12\x11\n\tbei_count\x18\x03 \x01(\r\"\xfb\x02\n\x0fRecordRoundInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63hang\x18\x02 \x01(\r\x12\n\n\x02ju\x18\x03 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\r\x12&\n\nliqi_infos\x18\x07 \x03(\x0b\x32\x12.lq.RecordLiqiInfo\x12&\n\ngang_infos\x18\x08 \x03(\x0b\x32\x12.lq.RecordGangInfo\x12*\n\x0cpeipai_infos\x18\t \x03(\x0b\x32\x14.lq.RecordPeiPaiInfo\x12(\n\x0b\x62\x61\x62\x61i_infos\x18\n \x03(\x0b\x32\x13.lq.RecordBaBeiInfo\x12\'\n\nhules_info\x18\x0b \x01(\x0b\x32\x13.lq.RecordHulesInfo\x12\'\n\nliuju_info\x18\x0c \x01(\x0b\x32\x13.lq.RecordLiujuInfo\x12*\n\x0cno_tile_info\x18\r \x01(\x0b\x32\x14.lq.RecordNoTileInfo\"@\n\x14RecordAnalysisedData\x12(\n\x0bround_infos\x18\x01 \x03(\x0b\x32\x13.lq.RecordRoundInfo\"[\n\x11ResConnectionInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x0f\x63lient_endpoint\x18\x02 \x01(\x0b\x32\x13.lq.NetworkEndpoint\"w\n\x10ReqSignupAccount\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\r\x12$\n\x06\x64\x65vice\x18\x05 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\",\n\x10ResSignupAccount\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"\xfe\x01\n\x08ReqLogin\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\x12\x0c\n\x04type\x18\t \x01(\r\x12\x0f\n\x07version\x18\n \x01(\r\"\xa9\x02\n\x08ResLogin\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x1c\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.lq.Account\x12&\n\tgame_info\x18\x04 \x01(\x0b\x32\x13.lq.GameConnectInfo\x12\x1f\n\x17has_unread_announcement\x18\x05 \x01(\x08\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x06 \x01(\t\x12\x13\n\x0bsignup_time\x18\x07 \x01(\r\x12\x19\n\x11is_id_card_authed\x18\x08 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\t \x01(\t\x12\x17\n\x0flogined_version\x18\n \x03(\r\x12\x18\n\x10rewarded_version\x18\x0b \x03(\r\"\xcb\x01\n\rReqEmailLogin\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12\x16\n\x0e\x63lient_version\x18\x06 \x01(\t\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\"3\n\x0eReqBindAccount\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"8\n\x18ReqCreatePhoneVerifyCode\x12\r\n\x05phone\x18\x01 \x01(\t\x12\r\n\x05usage\x18\x02 \x01(\r\"8\n\x18ReqCreateEmailVerifyCode\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\r\n\x05usage\x18\x02 \x01(\r\"9\n\x16ReqVerifyCodeForSecure\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\r\"H\n\x16ResVerfiyCodeForSecure\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0csecure_token\x18\x02 \x01(\t\"_\n\x12ReqBindPhoneNumber\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05phone\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1a\n\x12multi_bind_version\x18\x04 \x01(\x08\"E\n\x14ReqUnbindPhoneNumber\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05phone\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"G\n\x16ResFetchPhoneLoginBind\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bphone_login\x18\x02 \x01(\r\"+\n\x17ReqCreatePhoneLoginBind\x12\x10\n\x08password\x18\x01 \x01(\t\"=\n\x0cReqBindEmail\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"U\n\x11ReqModifyPassword\x12\x14\n\x0cnew_password\x18\x01 \x01(\t\x12\x14\n\x0cold_password\x18\x02 \x01(\t\x12\x14\n\x0csecure_token\x18\x03 \x01(\t\"8\n\rReqOauth2Auth\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03uid\x18\x03 \x01(\t\"?\n\rResOauth2Auth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\"4\n\x0eReqOauth2Check\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\"?\n\x0eResOauth2Check\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bhas_account\x18\x02 \x01(\x08\"\xb0\x01\n\x0fReqOauth2Signup\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x15\n\radvertise_str\x18\x04 \x01(\t\x12$\n\x06\x64\x65vice\x18\x05 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\"+\n\x0fResOauth2Signup\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"\xf7\x01\n\x0eReqOauth2Login\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x11\n\treconnect\x18\x03 \x01(\x08\x12$\n\x06\x64\x65vice\x18\x04 \x01(\x0b\x32\x14.lq.ClientDeviceInfo\x12\x12\n\nrandom_key\x18\x05 \x01(\t\x12-\n\x0e\x63lient_version\x18\x06 \x01(\x0b\x32\x15.lq.ClientVersionInfo\x12\x18\n\x10gen_access_token\x18\x07 \x01(\x08\x12\x1a\n\x12\x63urrency_platforms\x18\x08 \x03(\r\x12\x0f\n\x07version\x18\t \x01(\r\"$\n\x0eReqDMMPreLogin\x12\x12\n\nfinish_url\x18\x01 \x01(\t\"#\n\x0eResDMMPreLogin\x12\x11\n\tparameter\x18\x01 \x01(\t\"\x0b\n\tReqLogout\"%\n\tResLogout\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"+\n\x0bReqHeatBeat\x12\x1c\n\x14no_operation_counter\x18\x01 \x01(\r\" \n\x0cReqLoginBeat\x12\x10\n\x08\x63ontract\x18\x01 \x01(\t\"\'\n\x11ReqJoinMatchQueue\x12\x12\n\nmatch_mode\x18\x01 \x01(\r\")\n\x13ReqCancelMatchQueue\x12\x12\n\nmatch_mode\x18\x01 \x01(\r\"$\n\x0eReqAccountInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\"`\n\x0eResAccountInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1c\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.lq.Account\x12\x16\n\x04room\x18\x03 \x01(\x0b\x32\x08.lq.Room\"<\n\x11ReqCreateNickname\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x15\n\radvertise_str\x18\x02 \x01(\t\":\n\x11ReqModifyNickname\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x13\n\x0buse_item_id\x18\x02 \x01(\r\"%\n\x11ReqModifyBirthday\x12\x10\n\x08\x62irthday\x18\x01 \x01(\x05\"?\n\x0bResSelfRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"V\n\rReqCreateRoom\x12\x14\n\x0cplayer_count\x18\x01 \x01(\r\x12\x1a\n\x04mode\x18\x02 \x01(\x0b\x32\x0c.lq.GameMode\x12\x13\n\x0bpublic_live\x18\x03 \x01(\x08\"A\n\rResCreateRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"\x1e\n\x0bReqJoinRoom\x12\x0f\n\x07room_id\x18\x01 \x01(\r\"?\n\x0bResJoinRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x04room\x18\x02 \x01(\x0b\x32\x08.lq.Room\"\x1d\n\x0cReqRoomReady\x12\r\n\x05ready\x18\x01 \x01(\x08\"#\n\x0fReqRoomDressing\x12\x10\n\x08\x64ressing\x18\x01 \x01(\x08\"\x0e\n\x0cReqRoomStart\"!\n\x0bReqRoomKick\x12\x12\n\naccount_id\x18\x01 \x01(\r\"$\n\rReqModifyRoom\x12\x13\n\x0brobot_count\x18\x01 \x01(\r\"$\n\x0fReqChangeAvatar\x12\x11\n\tavatar_id\x18\x01 \x01(\r\"-\n\x17ReqAccountStatisticInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\"\x98\x01\n\x17ResAccountStatisticInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0estatistic_data\x18\x02 \x03(\x0b\x32\x18.lq.AccountStatisticData\x12\x31\n\x0b\x64\x65tail_data\x18\x03 \x01(\x0b\x32\x1c.lq.AccountDetailStatisticV2\"\xb9\x01\n\x1bResAccountChallengeRankInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x42\n\x0bseason_info\x18\x02 \x03(\x0b\x32-.lq.ResAccountChallengeRankInfo.ChallengeRank\x1a<\n\rChallengeRank\x12\x0e\n\x06season\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12\r\n\x05level\x18\x03 \x01(\r\".\n\x17ResAccountCharacterInfo\x12\x13\n\x0bunlock_list\x18\x01 \x03(\r\"+\n\x0fReqShopPurchase\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\r\"N\n\x0fResShopPurchase\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x06update\x18\x02 \x01(\x0b\x32\x11.lq.AccountUpdate\"\"\n\rReqGameRecord\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"g\n\rResGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1c\n\x04head\x18\x03 \x01(\x0b\x32\x0e.lq.RecordGame\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x10\n\x08\x64\x61ta_url\x18\x05 \x01(\t\"?\n\x11ReqGameRecordList\x12\r\n\x05start\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x0c\n\x04type\x18\x03 \x01(\r\"g\n\x11ResGameRecordList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0btotal_count\x18\x02 \x01(\r\x12#\n\x0brecord_list\x18\x03 \x03(\x0b\x32\x0e.lq.RecordGame\"\x82\x01\n\x1aResCollectedGameRecordList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x0brecord_list\x18\x02 \x03(\x0b\x32\x17.lq.RecordCollectedData\x12\x1c\n\x14record_collect_limit\x18\x03 \x01(\r\")\n\x14ReqGameRecordsDetail\x12\x11\n\tuuid_list\x18\x01 \x03(\t\"U\n\x14ResGameRecordsDetail\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x0brecord_list\x18\x02 \x03(\x0b\x32\x0e.lq.RecordGame\"`\n\x19ReqAddCollectedGameRecord\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\r\"5\n\x19ResAddCollectedGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\",\n\x1cReqRemoveCollectedGameRecord\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"8\n\x1cResRemoveCollectedGameRecord\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"D\n#ReqChangeCollectedGameRecordRemarks\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07remarks\x18\x02 \x01(\t\"?\n#ResChangeCollectedGameRecordRemarks\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"#\n\x13ReqLevelLeaderboard\x12\x0c\n\x04type\x18\x01 \x01(\r\"\xac\x01\n\x13ResLevelLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x05items\x18\x02 \x03(\x0b\x32\x1c.lq.ResLevelLeaderboard.Item\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a;\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x1f\n\x05level\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\")\n\x17ReqChallangeLeaderboard\x12\x0e\n\x06season\x18\x01 \x01(\r\"\xb4\x01\n\x17ResChallengeLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12/\n\x05items\x18\x02 \x03(\x0b\x32 .lq.ResChallengeLeaderboard.Item\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a;\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\x12\x10\n\x08nickname\x18\x03 \x01(\t\"@\n\x15ReqMutiChallengeLevel\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\x12\x0e\n\x06season\x18\x02 \x01(\r\"\x8b\x01\n\x15ResMutiChallengeLevel\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12-\n\x05items\x18\x02 \x03(\x0b\x32\x1e.lq.ResMutiChallengeLevel.Item\x1a)\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\",\n\x11ReqMultiAccountId\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\"U\n\x14ResMultiAccountBrief\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x07players\x18\x02 \x03(\x0b\x32\x12.lq.PlayerBaseView\"v\n\rResFriendList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1b\n\x07\x66riends\x18\x02 \x03(\x0b\x32\n.lq.Friend\x12\x18\n\x10\x66riend_max_count\x18\x03 \x01(\r\x12\x14\n\x0c\x66riend_count\x18\x04 \x01(\r\"\x9a\x01\n\x12ResFriendApplyList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x07\x61pplies\x18\x02 \x03(\x0b\x32\".lq.ResFriendApplyList.FriendApply\x1a\x35\n\x0b\x46riendApply\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x12\n\napply_time\x18\x02 \x01(\r\"#\n\x0eReqApplyFriend\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"9\n\x14ReqHandleFriendApply\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0e\n\x06method\x18\x02 \x01(\r\"$\n\x0fReqRemoveFriend\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"A\n\x19ReqSearchAccountByPattern\x12\x13\n\x0bsearch_next\x18\x01 \x01(\x08\x12\x0f\n\x07pattern\x18\x02 \x01(\t\"u\n\x19ResSearchAccountByPattern\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bis_finished\x18\x02 \x01(\x08\x12\x16\n\x0ematch_accounts\x18\x03 \x03(\r\x12\x11\n\tdecode_id\x18\x04 \x01(\r\")\n\x0eReqAccountList\x12\x17\n\x0f\x61\x63\x63ount_id_list\x18\x01 \x03(\r\"T\n\x10ResAccountStates\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12&\n\x06states\x18\x02 \x03(\x0b\x32\x16.lq.AccountActiveState\"*\n\x14ReqSearchAccountById\x12\x12\n\naccount_id\x18\x01 \x01(\r\"T\n\x14ResSearchAccountById\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x06player\x18\x02 \x01(\x0b\x32\x12.lq.PlayerBaseView\"<\n\nResBagInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x03\x62\x61g\x18\x02 \x01(\x0b\x32\x07.lq.Bag\" \n\rReqUseBagItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"F\n\x11ReqOpenManualItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tselect_id\x18\x03 \x01(\r\"*\n\x17ReqOpenRandomRewardItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"T\n\x17ResOpenRandomRewardItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\"\'\n\x14ReqOpenAllRewardItem\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"Q\n\x14ResOpenAllRewardItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\"\"\n\x0fReqComposeShard\x12\x0f\n\x07item_id\x18\x01 \x01(\r\"$\n\x14ReqFetchAnnouncement\x12\x0c\n\x04lang\x18\x01 \x01(\t\"u\n\x0fResAnnouncement\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rannouncements\x18\x02 \x03(\x0b\x32\x10.lq.Announcement\x12\x0c\n\x04sort\x18\x03 \x03(\r\x12\x11\n\tread_list\x18\x04 \x03(\r\"@\n\x0bResMailInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x17\n\x05mails\x18\x02 \x03(\x0b\x32\x08.lq.Mail\"\x1e\n\x0bReqReadMail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\" \n\rReqDeleteMail\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\"$\n\x11ReqTakeAttachment\x12\x0f\n\x07mail_id\x18\x01 \x01(\r\"4\n ReqReceiveAchievementGroupReward\x12\x10\n\x08group_id\x18\x01 \x01(\r\"g\n ResReceiveAchievementGroupReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"5\n\x1bReqReceiveAchievementReward\x12\x16\n\x0e\x61\x63hievement_id\x18\x01 \x01(\r\"b\n\x1bResReceiveAchievementReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"\x81\x01\n\x17ResFetchAchievementRate\x12\x39\n\x04rate\x18\x01 \x03(\x0b\x32+.lq.ResFetchAchievementRate.AchievementRate\x1a+\n\x0f\x41\x63hievementRate\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04rate\x18\x02 \x01(\r\"o\n\x0eResAchievement\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\nprogresses\x18\x02 \x03(\x0b\x32\x17.lq.AchievementProgress\x12\x16\n\x0erewarded_group\x18\x03 \x03(\r\"<\n\x0cResTitleList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\ntitle_list\x18\x02 \x03(\r\"\x1c\n\x0bReqUseTitle\x12\r\n\x05title\x18\x01 \x01(\r\"\x1d\n\rReqBuyShiLian\x12\x0c\n\x04type\x18\x01 \x01(\r\"2\n\x14ReqUpdateClientValue\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"w\n\x0eResClientValue\x12\'\n\x05\x64\x61tas\x18\x01 \x03(\x0b\x32\x18.lq.ResClientValue.Value\x12\x17\n\x0frecharged_count\x18\x02 \x01(\r\x1a#\n\x05Value\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"6\n\x10ReqClientMessage\x12\x11\n\ttimestamp\x18\x01 \x01(\r\x12\x0f\n\x07message\x18\x02 \x01(\t\"(\n\x13ReqCurrentMatchInfo\x12\x11\n\tmode_list\x18\x01 \x03(\r\"\xa6\x01\n\x13ResCurrentMatchInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x39\n\x07matches\x18\x02 \x03(\x0b\x32(.lq.ResCurrentMatchInfo.CurrentMatchInfo\x1a:\n\x10\x43urrentMatchInfo\x12\x0f\n\x07mode_id\x18\x01 \x01(\r\x12\x15\n\rplaying_count\x18\x02 \x01(\r\"2\n\x0fReqUserComplain\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\".\n\x13ReqReadAnnouncement\x12\x17\n\x0f\x61nnouncement_id\x18\x01 \x01(\r\"A\n\x11ResReviveCoinInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nhas_gained\x18\x02 \x01(\x08\"\x9e\x01\n\x0cResDailyTask\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\nprogresses\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x19\n\x11has_refresh_count\x18\x03 \x01(\x08\x12\x1c\n\x14max_daily_task_count\x18\x04 \x01(\r\x12\x15\n\rrefresh_count\x18\x05 \x01(\r\"&\n\x13ReqRefreshDailyTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"j\n\x13ResRefreshDailyTask\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x08progress\x18\x02 \x01(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\"\x1e\n\x0eReqUseGiftCode\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"K\n\x0eResUseGiftCode\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07rewards\x18\x06 \x03(\x0b\x32\x0e.lq.RewardSlot\"U\n\x15ResUseSpecialGiftCode\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\"\n\x07rewards\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"H\n\x14ReqSendClientMessage\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\"$\n\x0fReqGameLiveInfo\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"\xaf\x01\n\x0fResGameLiveInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1a\n\x12left_start_seconds\x18\x02 \x01(\r\x12#\n\tlive_head\x18\x03 \x01(\x0b\x32\x10.lq.GameLiveHead\x12(\n\x08segments\x18\x04 \x03(\x0b\x32\x16.lq.GameLiveSegmentUri\x12\x17\n\x0fnow_millisecond\x18\x05 \x01(\r\"D\n\x16ReqGameLiveLeftSegment\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x17\n\x0flast_segment_id\x18\x02 \x01(\r\"\xaa\x01\n\x16ResGameLiveLeftSegment\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nlive_state\x18\x02 \x01(\r\x12(\n\x08segments\x18\x04 \x03(\x0b\x32\x16.lq.GameLiveSegmentUri\x12\x17\n\x0fnow_millisecond\x18\x05 \x01(\r\x12\x1f\n\x17segment_end_millisecond\x18\x06 \x01(\r\"$\n\x0fReqGameLiveList\x12\x11\n\tfilter_id\x18\x01 \x01(\r\"P\n\x0fResGameLiveList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\tlive_list\x18\x02 \x03(\x0b\x32\x10.lq.GameLiveHead\"D\n\x11ResCommentSetting\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rcomment_allow\x18\x02 \x01(\r\"0\n\x17ReqUpdateCommentSetting\x12\x15\n\rcomment_allow\x18\x01 \x01(\r\"(\n\x13ReqFetchCommentList\x12\x11\n\ttarget_id\x18\x01 \x01(\r\"u\n\x13ResFetchCommentList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rcomment_allow\x18\x02 \x01(\r\x12\x17\n\x0f\x63omment_id_list\x18\x03 \x03(\r\x12\x14\n\x0clast_read_id\x18\x04 \x01(\r\"D\n\x16ReqFetchCommentContent\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x17\n\x0f\x63omment_id_list\x18\x02 \x03(\r\"U\n\x16ResFetchCommentContent\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\x08\x63omments\x18\x02 \x03(\x0b\x32\x0f.lq.CommentItem\"5\n\x0fReqLeaveComment\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\":\n\x10ReqDeleteComment\x12\x11\n\ttarget_id\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65lete_list\x18\x02 \x03(\r\"\'\n\x14ReqUpdateReadComment\x12\x0f\n\x07read_id\x18\x01 \x01(\r\"5\n\x10ReqRollingNotice\x12!\n\x06notice\x18\x01 \x03(\x0b\x32\x11.lq.RollingNotice\"$\n\rResServerTime\x12\x13\n\x0bserver_time\x18\x01 \x01(\r\"0\n\x1aReqPlatformBillingProducts\x12\x12\n\nshelves_id\x18\x01 \x01(\r\"\\\n\x1aResPlatformBillingProducts\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\x08products\x18\x02 \x03(\x0b\x32\x12.lq.BillingProduct\"l\n\x15ReqCreateBillingOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x18\n\x10payment_platform\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\x12\x12\n\naccount_id\x18\x04 \x01(\r\"C\n\x15ResCreateBillingOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"T\n\x17ReqSolveGooglePlayOrder\x12\x1b\n\x13inapp_purchase_data\x18\x02 \x01(\t\x12\x1c\n\x14inapp_data_signature\x18\x03 \x01(\t\"h\n\x19ReqSolveGooglePlayOrderV3\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x16\n\x0etransaction_id\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\r\",\n\x18ReqCancelGooglePlayOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\"k\n\x1aReqCreateWechatNativeOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\naccount_ip\x18\x04 \x01(\t\"_\n\x1aResCreateWechatNativeOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rqrcode_buffer\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\"h\n\x17ReqCreateWechatAppOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\naccount_ip\x18\x04 \x01(\t\"\x91\x02\n\x17ResCreateWechatAppOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12M\n\x15\x63\x61ll_wechat_app_param\x18\x02 \x01(\x0b\x32..lq.ResCreateWechatAppOrder.CallWechatAppParam\x1a\x8c\x01\n\x12\x43\x61llWechatAppParam\x12\r\n\x05\x61ppid\x18\x01 \x01(\t\x12\x11\n\tpartnerid\x18\x02 \x01(\t\x12\x10\n\x08prepayid\x18\x03 \x01(\t\x12\x0f\n\x07package\x18\x04 \x01(\t\x12\x10\n\x08noncestr\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04sign\x18\x07 \x01(\t\"\x80\x01\n\x14ReqCreateAlipayOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x19\n\x11\x61lipay_trade_type\x18\x04 \x01(\t\x12\x12\n\nreturn_url\x18\x05 \x01(\t\"D\n\x14ResCreateAlipayOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nalipay_url\x18\x02 \x01(\t\"U\n\x18ReqCreateAlipayScanOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"n\n\x18ResCreateAlipayScanOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\rqrcode_buffer\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\x12\x0f\n\x07qr_code\x18\x04 \x01(\t\"T\n\x17ReqCreateAlipayAppOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"G\n\x17ResCreateAlipayAppOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nalipay_url\x18\x02 \x01(\t\"\x81\x01\n\x1aReqCreateJPCreditCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"H\n\x1aResCreateJPCreditCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateJPPaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateJPPaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"y\n\x12ReqCreateJPAuOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"@\n\x12ResCreateJPAuOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateJPDocomoOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateJPDocomoOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x7f\n\x18ReqCreateJPWebMoneyOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"F\n\x18ResCreateJPWebMoneyOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x7f\n\x18ReqCreateJPSoftbankOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"F\n\x18ResCreateJPSoftbankOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"e\n\x14ReqCreateYostarOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\norder_type\x18\x04 \x01(\r\"B\n\x14ResCreateYostarOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateENPaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateENPaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"z\n\x13ReqCreateENJCBOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"A\n\x13ResCreateENJCBOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"\x81\x01\n\x1aReqCreateENMasterCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"H\n\x1aResCreateENMasterCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"{\n\x14ReqCreateENVisaOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"B\n\x14ResCreateENVisaOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"}\n\x16ReqCreateENAlipayOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x12\n\nreturn_url\x18\x04 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\t\"D\n\x16ResCreateENAlipayOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"N\n\x11ReqCreateDMMOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\"\xbb\x01\n\x11ResCreateDmmOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x16\n\x0etransaction_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64mm_user_id\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x06 \x01(\t\x12\x14\n\x0crequest_time\x18\t \x01(\t\x12\x12\n\ndmm_app_id\x18\n \x01(\t\"d\n\x11ReqCreateIAPOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\t\"?\n\x11ResCreateIAPOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\"m\n\x17ReqVerificationIAPOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x16\n\x0etransaction_id\x18\x02 \x01(\t\x12\x14\n\x0creceipt_data\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\r\"3\n\x17ResVerificationIAPOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\"t\n\x13ReqCreateSteamOrder\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x03 \x01(\r\x12\x10\n\x08goods_id\x18\x04 \x01(\r\x12\x10\n\x08steam_id\x18\x05 \x01(\t\"\\\n\x13ResCreateSteamOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x19\n\x11platform_order_id\x18\x03 \x01(\t\";\n\x13ReqVerifySteamOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\"Q\n\x14ReqCreateMyCardOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"U\n\x14ResCreateMyCardOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tauth_code\x18\x02 \x01(\t\x12\x10\n\x08order_id\x18\x03 \x01(\t\"<\n\x14ReqVerifyMyCardOrder\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\r\"Q\n\x14ReqCreatePaypalOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\"O\n\x14ResCreatePaypalOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"i\n\x14ReqCreateXsollaOrder\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\x13\n\x0b\x63lient_type\x18\x02 \x01(\r\x12\x12\n\naccount_id\x18\x03 \x01(\r\x12\x16\n\x0epayment_method\x18\x04 \x01(\r\"O\n\x14ResCreateXsollaOrder\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"C\n\x0cReqOpenChest\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x12\n\nuse_ticket\x18\x03 \x01(\x08\"\xee\x01\n\x0cResOpenChest\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07results\x18\x02 \x03(\x0b\x32\x0e.lq.OpenResult\x12\x18\n\x10total_open_count\x18\x03 \x01(\r\x12\x13\n\x0b\x66\x61ith_count\x18\x04 \x01(\r\x12@\n\x10\x63hest_replace_up\x18\x05 \x03(\x0b\x32&.lq.ResOpenChest.ChestReplaceCountData\x1a\x32\n\x15\x43hestReplaceCountData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"6\n\x13ReqBuyFromChestShop\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"m\n\x13ResBuyFromChestShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08\x63hest_id\x18\x02 \x01(\r\x12\x15\n\rconsume_count\x18\x03 \x01(\r\x12\x13\n\x0b\x66\x61ith_count\x18\x04 \x01(\r\"D\n\x12ResDailySignInInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0csign_in_days\x18\x02 \x01(\r\"*\n\x13ReqDoActivitySignIn\x12\x13\n\x0b\x61\x63tivity_id\x18\x02 \x01(\r\"\xad\x01\n\x13ResDoActivitySignIn\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x07rewards\x18\x02 \x03(\x0b\x32\".lq.ResDoActivitySignIn.RewardData\x12\x15\n\rsign_in_count\x18\x03 \x01(\r\x1a\x30\n\nRewardData\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\xf7\x01\n\x10ResCharacterInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12!\n\ncharacters\x18\x02 \x03(\x0b\x32\r.lq.Character\x12\r\n\x05skins\x18\x03 \x03(\r\x12\x19\n\x11main_character_id\x18\x04 \x01(\r\x12\x17\n\x0fsend_gift_count\x18\x05 \x01(\r\x12\x17\n\x0fsend_gift_limit\x18\x06 \x01(\r\x12\x18\n\x10\x66inished_endings\x18\x07 \x03(\r\x12\x18\n\x10rewarded_endings\x18\x08 \x03(\r\x12\x16\n\x0e\x63haracter_sort\x18\t \x03(\r\"&\n\x16ReqUpdateCharacterSort\x12\x0c\n\x04sort\x18\x01 \x03(\r\".\n\x16ReqChangeMainCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\"<\n\x16ReqChangeCharacterSkin\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x0c\n\x04skin\x18\x02 \x01(\r\"M\n\x16ReqChangeCharacterView\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x0c\n\x04slot\x18\x02 \x01(\r\x12\x0f\n\x07item_id\x18\x03 \x01(\r\"\x86\x01\n\x16ReqSendGiftToCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12.\n\x05gifts\x18\x02 \x03(\x0b\x32\x1f.lq.ReqSendGiftToCharacter.Gift\x1a&\n\x04Gift\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"N\n\x16ResSendGiftToCharacter\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\r\n\x05level\x18\x02 \x01(\r\x12\x0b\n\x03\x65xp\x18\x03 \x01(\r\"Z\n\x0bReqSellItem\x12#\n\x05sells\x18\x01 \x03(\x0b\x32\x14.lq.ReqSellItem.Item\x1a&\n\x04Item\x12\x0f\n\x07item_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"u\n\rResCommonView\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12%\n\x05slots\x18\x02 \x03(\x0b\x32\x16.lq.ResCommonView.Slot\x1a#\n\x04Slot\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"2\n\x13ReqChangeCommonView\x12\x0c\n\x04slot\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\r\"U\n\x12ReqSaveCommonViews\x12\x1b\n\x05views\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\x12\n\nsave_index\x18\x02 \x01(\r\x12\x0e\n\x06is_use\x18\x03 \x01(\r\"\x1f\n\x0eReqCommonViews\x12\r\n\x05index\x18\x01 \x01(\r\"-\n\x0eResCommonViews\x12\x1b\n\x05views\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\"\x9c\x01\n\x11ResAllcommonViews\x12*\n\x05views\x18\x01 \x03(\x0b\x32\x1b.lq.ResAllcommonViews.Views\x12\x0b\n\x03use\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\x1a\x34\n\x05Views\x12\x1c\n\x06values\x18\x01 \x03(\x0b\x32\x0c.lq.ViewSlot\x12\r\n\x05index\x18\x02 \x01(\r\"!\n\x10ReqUseCommonView\x12\r\n\x05index\x18\x03 \x01(\r\"+\n\x13ReqUpgradeCharacter\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\"Q\n\x13ResUpgradeCharacter\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12 \n\tcharacter\x18\x02 \x01(\x0b\x32\r.lq.Character\"N\n\x11ReqFinishedEnding\x12\x14\n\x0c\x63haracter_id\x18\x01 \x01(\r\x12\x10\n\x08story_id\x18\x02 \x01(\r\x12\x11\n\tending_id\x18\x03 \x01(\r\"\x1f\n\x0cReqGMCommand\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"H\n\x0bResShopInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\tshop_info\x18\x02 \x01(\x0b\x32\x0c.lq.ShopInfo\"o\n\x0eReqBuyFromShop\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12(\n\x0e\x62ill_short_cut\x18\x03 \x03(\x0b\x32\x10.lq.BillShortcut\x12\x12\n\ndeal_price\x18\x04 \x01(\r\"K\n\x0eResBuyFromShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x1f\n\x07rewards\x18\x02 \x03(\x0b\x32\x0e.lq.RewardSlot\"0\n\rReqBuyFromZHP\x12\x10\n\x08goods_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"&\n\x11ReqPayMonthTicket\x12\x11\n\tticket_id\x18\x01 \x01(\r\"Z\n\x11ResPayMonthTicket\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x13\n\x0bresource_id\x18\x02 \x01(\r\x12\x16\n\x0eresource_count\x18\x03 \x01(\r\"<\n\x0eReqReshZHPShop\x12\x14\n\x0c\x66ree_refresh\x18\x01 \x01(\r\x12\x14\n\x0c\x63ost_refresh\x18\x02 \x01(\r\"G\n\x11ResRefreshZHPShop\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x18\n\x03zhp\x18\x02 \x01(\x0b\x32\x0b.lq.ZHPShop\"D\n\x12ResMonthTicketInfo\x12.\n\x11month_ticket_info\x18\x01 \x03(\x0b\x32\x13.lq.MonthTicketInfo\"0\n\x13ReqExchangeCurrency\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"9\n\x11ResServerSettings\x12$\n\x08settings\x18\x01 \x01(\x0b\x32\x12.lq.ServerSettings\"T\n\x12ResAccountSettings\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12$\n\x08settings\x18\x02 \x03(\x0b\x32\x12.lq.AccountSetting\"?\n\x18ReqUpdateAccountSettings\x12#\n\x07setting\x18\x01 \x01(\x0b\x32\x12.lq.AccountSetting\"+\n\x12ResModNicknameTime\x12\x15\n\rlast_mod_time\x18\x01 \x01(\r\"\x98\x01\n\x07ResMisc\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x0erecharged_list\x18\x02 \x03(\r\x12)\n\x06\x66\x61iths\x18\x03 \x03(\x0b\x32\x19.lq.ResMisc.MiscFaithData\x1a\x30\n\rMiscFaithData\x12\x10\n\x08\x66\x61ith_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\'\n\x12ReqModifySignature\x12\x11\n\tsignature\x18\x01 \x01(\t\"M\n\rResIDCardInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tis_authed\x18\x02 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\"8\n\x13ReqUpdateIDCardInfo\x12\x10\n\x08\x66ullname\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61rd_no\x18\x02 \x01(\t\"C\n\x0cResVipReward\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x19\n\x11gained_vip_levels\x18\x02 \x03(\r\"%\n\x10ReqGainVipReward\x12\x11\n\tvip_level\x18\x01 \x01(\r\"=\n\x1dReqFetchCustomizedContestList\x12\r\n\x05start\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"\x9a\x01\n\x1dResFetchCustomizedContestList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x08\x63ontests\x18\x02 \x03(\x0b\x32\x19.lq.CustomizedContestBase\x12\x32\n\x0f\x66ollow_contests\x18\x03 \x03(\x0b\x32\x19.lq.CustomizedContestBase\"7\n#ReqFetchCustomizedContestExtendInfo\x12\x10\n\x08uid_list\x18\x01 \x03(\r\"q\n#ResFetchCustomizedContestExtendInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0b\x65xtend_list\x18\x02 \x03(\x0b\x32\x1b.lq.CustomizedContestExtend\"6\n!ReqFetchCustomizedContestAuthInfo\x12\x11\n\tunique_id\x18\x01 \x01(\r\"U\n!ResFetchCustomizedContestAuthInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x16\n\x0eobserver_level\x18\x02 \x01(\r\".\n\x19ReqEnterCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"\xb6\x01\n\x19ResEnterCustomizedContest\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x30\n\x0b\x64\x65tail_info\x18\x02 \x01(\x0b\x32\x1b.lq.CustomizedContestDetail\x12\x38\n\rplayer_report\x18\x03 \x01(\x0b\x32!.lq.CustomizedContestPlayerReport\x12\x13\n\x0bis_followed\x18\x04 \x01(\x08\"8\n#ReqFetchCustomizedContestOnlineInfo\x12\x11\n\tunique_id\x18\x01 \x01(\r\"V\n#ResFetchCustomizedContestOnlineInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x15\n\ronline_player\x18\x02 \x01(\r\":\n$ReqFetchCustomizedContestByContestId\x12\x12\n\ncontest_id\x18\x01 \x01(\r\"u\n$ResFetchCustomizedContestByContestId\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x33\n\x0c\x63ontest_info\x18\x02 \x01(\x0b\x32\x1d.lq.CustomizedContestAbstract\".\n\x19ReqStartCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"5\n ReqJoinCustomizedContestChatRoom\x12\x11\n\tunique_id\x18\x01 \x01(\r\"R\n ResJoinCustomizedContestChatRoom\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x14\n\x0c\x63hat_history\x18\x02 \x03(\x0c\"$\n\x11ReqSayChatMessage\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\":\n%ReqFetchCustomizedContestGameLiveList\x12\x11\n\tunique_id\x18\x01 \x01(\r\"f\n%ResFetchCustomizedContestGameLiveList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\tlive_list\x18\x02 \x03(\x0b\x32\x10.lq.GameLiveHead\"M\n$ReqFetchCustomizedContestGameRecords\x12\x11\n\tunique_id\x18\x01 \x01(\r\x12\x12\n\nlast_index\x18\x02 \x01(\r\"y\n$ResFetchCustomizedContestGameRecords\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x12\n\nnext_index\x18\x02 \x01(\r\x12#\n\x0brecord_list\x18\x03 \x03(\x0b\x32\x0e.lq.RecordGame\"/\n\x1aReqTargetCustomizedContest\x12\x11\n\tunique_id\x18\x01 \x01(\r\"M\n\x0fResActivityList\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12 \n\nactivities\x18\x02 \x03(\x0b\x32\x0c.lq.Activity\"\xed\x07\n\x16ResAccountActivityData\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12,\n\x10\x65xchange_records\x18\x02 \x03(\x0b\x32\x12.lq.ExchangeRecord\x12,\n\x12task_progress_list\x18\x03 \x03(\x0b\x32\x10.lq.TaskProgress\x12@\n\x16\x61\x63\x63umulated_point_list\x18\x04 \x03(\x0b\x32 .lq.ActivityAccumulatedPointData\x12\x31\n\x0erank_data_list\x18\x05 \x03(\x0b\x32\x19.lq.ActivityRankPointData\x12\x31\n\x17\x66lip_task_progress_list\x18\x06 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x43\n\x0csign_in_data\x18\x07 \x03(\x0b\x32-.lq.ResAccountActivityData.ActivitySignInData\x12\x44\n\x0crichman_data\x18\x08 \x03(\x0b\x32..lq.ResAccountActivityData.ActivityRichmanData\x12\x33\n\x19period_task_progress_list\x18\t \x03(\x0b\x32\x10.lq.TaskProgress\x12\x33\n\x19random_task_progress_list\x18\n \x03(\x0b\x32\x10.lq.TaskProgress\x12=\n\rchest_up_data\x18\x0b \x03(\x0b\x32&.lq.ResAccountActivityData.ChestUpData\x1a[\n\x12\x41\x63tivitySignInData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x15\n\rsign_in_count\x18\x02 \x01(\r\x12\x19\n\x11last_sign_in_time\x18\x03 \x01(\r\x1a\x38\n\x08\x42uffData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0e\n\x06remain\x18\x02 \x01(\r\x12\x0e\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\r\x1a\xbf\x01\n\x13\x41\x63tivityRichmanData\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x10\n\x08location\x18\x02 \x01(\r\x12\x16\n\x0e\x66inished_count\x18\x03 \x01(\r\x12\x16\n\x0e\x63hest_position\x18\x04 \x01(\r\x12\x11\n\tbank_save\x18\x05 \x01(\r\x12\x0b\n\x03\x65xp\x18\x06 \x01(\r\x12\x31\n\x04\x62uff\x18\x07 \x03(\x0b\x32#.lq.ResAccountActivityData.BuffData\x1a(\n\x0b\x43hestUpData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"=\n\x17ReqExchangeActivityItem\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"^\n\x17ResExchangeActivityItem\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12)\n\x0e\x65xecute_reward\x18\x02 \x03(\x0b\x32\x11.lq.ExecuteReward\"*\n\x17ReqCompleteActivityTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"-\n\x1aReqReceiveActivityFlipTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"E\n\x1aResReceiveActivityFlipTask\x12\r\n\x05\x63ount\x18\x01 \x01(\r\x12\x18\n\x05\x65rror\x18\x02 \x01(\x0b\x32\t.lq.Error\"/\n\x18ReqFetchActivityFlipInfo\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"T\n\x18ResFetchActivityFlipInfo\x12\x0f\n\x07rewards\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\"O\n%ReqGainAccumulatedPointActivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x11\n\treward_id\x18\x02 \x01(\r\"N\n\x1fReqGainMultiPointActivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x16\n\x0ereward_id_list\x18\x02 \x03(\r\"6\n\x1cReqFetchRankPointLeaderboard\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\"\xe4\x01\n\x1cResFetchRankPointLeaderboard\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x34\n\x05items\x18\x02 \x03(\x0b\x32%.lq.ResFetchRankPointLeaderboard.Item\x12\x19\n\x11last_refresh_time\x18\x03 \x01(\r\x1aY\n\x04Item\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0c\n\x04rank\x18\x02 \x01(\r\x12 \n\x04view\x18\x03 \x01(\x0b\x32\x12.lq.PlayerBaseView\x12\r\n\x05point\x18\x04 \x01(\r\"E\n\x16ReqGainRankPointReward\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\x13\n\x0b\x61\x63tivity_id\x18\x02 \x01(\r\")\n\x12ReqRichmanNextMove\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x94\x04\n\x12ResRichmanNextMove\x12.\n\x05paths\x18\x01 \x03(\x0b\x32\x1f.lq.ResRichmanNextMove.PathData\x12\x0c\n\x04\x64ice\x18\x02 \x01(\r\x12\x10\n\x08location\x18\x03 \x01(\r\x12\x16\n\x0e\x66inished_count\x18\x04 \x01(\r\x12\x0c\n\x04step\x18\x05 \x01(\r\x12-\n\x04\x62uff\x18\x06 \x03(\x0b\x32\x1f.lq.ResRichmanNextMove.BuffData\x12\x11\n\tbank_save\x18\x07 \x01(\r\x12\x16\n\x0e\x63hest_position\x18\x08 \x01(\r\x12\x0b\n\x03\x65xp\x18\t \x01(\r\x12\x15\n\rbank_save_add\x18\n \x01(\r\x12\x18\n\x05\x65rror\x18\x0b \x01(\x0b\x32\t.lq.Error\x1aT\n\nRewardData\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x14\n\x0corigin_count\x18\x03 \x01(\r\x12\x0c\n\x04type\x18\x05 \x01(\r\x1a`\n\x08PathData\x12\x10\n\x08location\x18\x01 \x01(\r\x12\x32\n\x07rewards\x18\x02 \x03(\x0b\x32!.lq.ResRichmanNextMove.RewardData\x12\x0e\n\x06\x65vents\x18\x03 \x03(\r\x1a\x38\n\x08\x42uffData\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0e\n\x06remain\x18\x02 \x01(\r\x12\x0e\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\r\":\n\x15ReqRichmanSpecialMove\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x0c\n\x04step\x18\x02 \x01(\r\"*\n\x13ReqRichmanChestInfo\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x87\x01\n\x13ResRichmanChestInfo\x12/\n\x05items\x18\x01 \x03(\x0b\x32 .lq.ResRichmanChestInfo.ItemData\x12\x18\n\x05\x65rror\x18\x02 \x01(\x0b\x32\t.lq.Error\x1a%\n\x08ItemData\x12\n\n\x02id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"-\n\x18ReqCreateGameObserveAuth\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\"U\n\x18ResCreateGameObserveAuth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\"*\n\x19ReqRefreshGameObserveAuth\x12\r\n\x05token\x18\x01 \x01(\t\"B\n\x19ResRefreshGameObserveAuth\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0b\n\x03ttl\x18\x02 \x01(\r\"\x98\x01\n\x0fResActivityBuff\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x37\n\tbuff_list\x18\x02 \x03(\x0b\x32$.lq.ResActivityBuff.ActivityBuffData\x1a\x32\n\x10\x41\x63tivityBuffData\x12\x0f\n\x07\x62uff_id\x18\x01 \x01(\r\x12\r\n\x05level\x18\x02 \x01(\r\")\n\x16ReqUpgradeActivityBuff\x12\x0f\n\x07\x62uff_id\x18\x01 \x01(\r\"\xa6\x01\n\x13ResUpgradeChallenge\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\"\xa6\x01\n\x13ResRefreshChallenge\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\"\xc1\x01\n\x15ResFetchChallengeInfo\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\rtask_progress\x18\x02 \x03(\x0b\x32\x10.lq.TaskProgress\x12\x15\n\rrefresh_count\x18\x03 \x01(\r\x12\r\n\x05level\x18\x04 \x01(\r\x12\x13\n\x0bmatch_count\x18\x05 \x01(\r\x12\x11\n\tticket_id\x18\x06 \x01(\r\x12\x17\n\x0frewarded_season\x18\x07 \x03(\r\"0\n\x1dReqForceCompleteChallengeTask\x12\x0f\n\x07task_id\x18\x01 \x01(\r\"\xff\x01\n\x0fResFetchABMatch\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x10\n\x08match_id\x18\x02 \x01(\r\x12\x13\n\x0bmatch_count\x18\x03 \x01(\r\x12\x14\n\x0c\x62uy_in_count\x18\x04 \x01(\r\x12\r\n\x05point\x18\x05 \x01(\r\x12\x10\n\x08rewarded\x18\x06 \x01(\x08\x12\x37\n\x0fmatch_max_point\x18\x07 \x03(\x0b\x32\x1e.lq.ResFetchABMatch.MatchPoint\x12\x0c\n\x04quit\x18\x08 \x01(\x08\x1a-\n\nMatchPoint\x12\x10\n\x08match_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\")\n\x14ReqStartUnifiedMatch\x12\x11\n\tmatch_sid\x18\x01 \x01(\t\"*\n\x15ReqCancelUnifiedMatch\x12\x11\n\tmatch_sid\x18\x01 \x01(\t\"\xba\x01\n\x16ResChallengeSeasonInfo\x12G\n\x15\x63hallenge_season_list\x18\x01 \x03(\x0b\x32(.lq.ResChallengeSeasonInfo.ChallengeInfo\x1aW\n\rChallengeInfo\x12\x11\n\tseason_id\x18\x01 \x01(\r\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\x12\r\n\x05state\x18\x04 \x01(\r\"2\n\x1dReqReceiveChallengeRankReward\x12\x11\n\tseason_id\x18\x01 \x01(\r\"\x88\x01\n\x1dResReceiveChallengeRankReward\x12\x39\n\x07rewards\x18\x01 \x03(\x0b\x32(.lq.ResReceiveChallengeRankReward.Reward\x1a,\n\x06Reward\x12\x13\n\x0bresource_id\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"#\n\x0fReqBuyInABMatch\x12\x10\n\x08match_id\x18\x01 \x01(\r\"\'\n\x10ReqGamePointRank\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\"\x9b\x01\n\x10ResGamePointRank\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12+\n\x04rank\x18\x02 \x03(\x0b\x32\x1d.lq.ResGamePointRank.RankInfo\x12\x11\n\tself_rank\x18\x03 \x01(\r\x1a-\n\x08RankInfo\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"H\n\x19ResFetchSelfGamePointRank\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x11\n\tself_rate\x18\x02 \x01(\r\"\x0f\n\rActionMJStart\"A\n\x13NewRoundOpenedTiles\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05tiles\x18\x02 \x03(\t\x12\r\n\x05\x63ount\x18\x03 \x03(\r\"F\n\x08MuyuInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x11\n\tcount_max\x18\x03 \x01(\r\x12\n\n\x02id\x18\x04 \x01(\r\"\x8a\x01\n\x0b\x43huanmaGang\x12\x12\n\nold_scores\x18\x01 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x02 \x03(\x05\x12\x0e\n\x06scores\x18\x03 \x03(\x05\x12\x1c\n\x07gameend\x18\x04 \x01(\x0b\x32\x0b.lq.GameEnd\x12#\n\rhules_history\x18\x05 \x03(\x0b\x32\x0c.lq.HuleInfo\"\x8b\x03\n\x0e\x41\x63tionNewRound\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x0c\n\x04\x64ora\x18\x05 \x01(\t\x12\x0e\n\x06scores\x18\x06 \x03(\x05\x12,\n\toperation\x18\x07 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x10\n\x08liqibang\x18\x08 \x01(\r\x12)\n\ttingpais0\x18\t \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\"\n\ttingpais1\x18\n \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\n\n\x02\x61l\x18\x0b \x01(\x08\x12\x0b\n\x03md5\x18\x0c \x01(\t\x12\x17\n\x0fleft_tile_count\x18\r \x01(\r\x12\r\n\x05\x64oras\x18\x0e \x03(\t\x12&\n\x05opens\x18\x0f \x03(\x0b\x32\x17.lq.NewRoundOpenedTiles\x12\x1a\n\x04muyu\x18\x10 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x10\n\x08ju_count\x18\x11 \x01(\r\"\x8b\x04\n\x0eRecordNewRound\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\x0c\n\x04\x64ora\x18\x04 \x01(\t\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x10\n\x08liqibang\x18\x06 \x01(\r\x12\x0e\n\x06tiles0\x18\x07 \x03(\t\x12\x0e\n\x06tiles1\x18\x08 \x03(\t\x12\x0e\n\x06tiles2\x18\t \x03(\t\x12\x0e\n\x06tiles3\x18\n \x03(\t\x12+\n\x07tingpai\x18\x0b \x03(\x0b\x32\x1a.lq.RecordNewRound.TingPai\x12,\n\toperation\x18\x0c \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x0b\n\x03md5\x18\r \x01(\t\x12\x0f\n\x07paishan\x18\x0e \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x0f \x01(\r\x12\r\n\x05\x64oras\x18\x10 \x03(\t\x12&\n\x05opens\x18\x11 \x03(\x0b\x32\x17.lq.NewRoundOpenedTiles\x12\x1a\n\x04muyu\x18\x12 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12-\n\noperations\x18\x13 \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\x10\n\x08ju_count\x18\x14 \x01(\r\x1a;\n\x07TingPai\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\ttingpais1\x18\x02 \x03(\x0b\x32\x0f.lq.TingPaiInfo\"\x99\x03\n\x0cGameSnapshot\x12\r\n\x05\x63hang\x18\x01 \x01(\r\x12\n\n\x02ju\x18\x02 \x01(\r\x12\x0b\n\x03\x62\x65n\x18\x03 \x01(\r\x12\x14\n\x0cindex_player\x18\x04 \x01(\r\x12\x17\n\x0fleft_tile_count\x18\x05 \x01(\r\x12\r\n\x05hands\x18\x06 \x03(\t\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x10\n\x08liqibang\x18\x08 \x01(\r\x12\x30\n\x07players\x18\t \x03(\x0b\x32\x1f.lq.GameSnapshot.PlayerSnapshot\x12\x10\n\x08zhenting\x18\n \x01(\x08\x1a\xbd\x01\n\x0ePlayerSnapshot\x12\r\n\x05score\x18\x01 \x01(\x05\x12\x14\n\x0cliqiposition\x18\x02 \x01(\x05\x12\x0f\n\x07tilenum\x18\x03 \x01(\r\x12\x0e\n\x06qipais\x18\x04 \x03(\t\x12\x33\n\x05mings\x18\x05 \x03(\x0b\x32$.lq.GameSnapshot.PlayerSnapshot.Fulu\x1a\x30\n\x04\x46ulu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x03(\t\x12\x0c\n\x04\x66rom\x18\x03 \x03(\r\";\n\x0f\x41\x63tionPrototype\x12\x0c\n\x04step\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"$\n\x11GameDetailRecords\x12\x0f\n\x07records\x18\x01 \x03(\x0c\"z\n\x11OptionalOperation\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x13\n\x0b\x63ombination\x18\x02 \x03(\t\x12\x14\n\x0c\x63hange_tiles\x18\x03 \x03(\t\x12\x1a\n\x12\x63hange_tile_states\x18\x04 \x03(\x05\x12\x10\n\x08gap_type\x18\x05 \x01(\r\"z\n\x15OptionalOperationList\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12-\n\x0eoperation_list\x18\x02 \x03(\x0b\x32\x15.lq.OptionalOperation\x12\x10\n\x08time_add\x18\x04 \x01(\r\x12\x12\n\ntime_fixed\x18\x05 \x01(\r\"L\n\x0bLiQiSuccess\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05score\x18\x02 \x01(\x05\x12\x10\n\x08liqibang\x18\x03 \x01(\r\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\"0\n\x07\x46\x61nInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03val\x18\x02 \x01(\r\x12\n\n\x02id\x18\x03 \x01(\r\"\xe0\x02\n\x08HuleInfo\x12\x0c\n\x04hand\x18\x01 \x03(\t\x12\x0c\n\x04ming\x18\x02 \x03(\t\x12\x0f\n\x07hu_tile\x18\x03 \x01(\t\x12\x0c\n\x04seat\x18\x04 \x01(\r\x12\x0c\n\x04zimo\x18\x05 \x01(\x08\x12\x0e\n\x06qinjia\x18\x06 \x01(\x08\x12\x0c\n\x04liqi\x18\x07 \x01(\x08\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08li_doras\x18\t \x03(\t\x12\r\n\x05yiman\x18\n \x01(\x08\x12\r\n\x05\x63ount\x18\x0b \x01(\r\x12\x19\n\x04\x66\x61ns\x18\x0c \x03(\x0b\x32\x0b.lq.FanInfo\x12\n\n\x02\x66u\x18\r \x01(\r\x12\r\n\x05title\x18\x0e \x01(\t\x12\x12\n\npoint_rong\x18\x0f \x01(\r\x12\x16\n\x0epoint_zimo_qin\x18\x10 \x01(\r\x12\x17\n\x0fpoint_zimo_xian\x18\x11 \x01(\r\x12\x10\n\x08title_id\x18\x12 \x01(\r\x12\x11\n\tpoint_sum\x18\x13 \x01(\r\x12\x0e\n\x06\x64\x61\x64ian\x18\x14 \x01(\r\"\xa7\x01\n\x0bTingPaiInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x0e\n\x06haveyi\x18\x02 \x01(\x08\x12\r\n\x05yiman\x18\x03 \x01(\x08\x12\r\n\x05\x63ount\x18\x04 \x01(\r\x12\n\n\x02\x66u\x18\x05 \x01(\r\x12\x17\n\x0f\x62iao_dora_count\x18\x06 \x01(\r\x12\x12\n\nyiman_zimo\x18\x07 \x01(\x08\x12\x12\n\ncount_zimo\x18\x08 \x01(\r\x12\x0f\n\x07\x66u_zimo\x18\t \x01(\r\"T\n\x12TingPaiDiscardInfo\x12\x0c\n\x04tile\x18\x01 \x01(\t\x12\x10\n\x08zhenting\x18\x02 \x01(\x08\x12\x1e\n\x05infos\x18\x03 \x03(\x0b\x32\x0f.lq.TingPaiInfo\"\x19\n\x07GameEnd\x12\x0e\n\x06scores\x18\x01 \x03(\x05\"\xa1\x01\n\x0f\x41\x63tionSelectGap\x12\x11\n\tgap_types\x18\x01 \x03(\r\x12)\n\ttingpais0\x18\x02 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\"\n\ttingpais1\x18\x03 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\"\xbd\x01\n\x0fRecordSelectGap\x12\x11\n\tgap_types\x18\x01 \x03(\r\x12,\n\x07tingpai\x18\x02 \x03(\x0b\x32\x1b.lq.RecordSelectGap.TingPai\x12,\n\toperation\x18\x03 \x01(\x0b\x32\x19.lq.OptionalOperationList\x1a;\n\x07TingPai\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\ttingpais1\x18\x02 \x03(\x0b\x32\x0f.lq.TingPaiInfo\"\x89\x02\n\x10\x41\x63tionChangeTile\x12\x10\n\x08in_tiles\x18\x01 \x03(\t\x12\x16\n\x0ein_tile_states\x18\x02 \x03(\x05\x12\x11\n\tout_tiles\x18\x03 \x03(\t\x12\x17\n\x0fout_tile_states\x18\x04 \x03(\x05\x12\r\n\x05\x64oras\x18\x05 \x03(\t\x12)\n\ttingpais0\x18\x06 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\"\n\ttingpais1\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0b\x63hange_type\x18\t \x01(\r\"\x9f\x03\n\x10RecordChangeTile\x12\r\n\x05\x64oras\x18\x01 \x03(\t\x12-\n\x07tingpai\x18\x02 \x03(\x0b\x32\x1c.lq.RecordChangeTile.TingPai\x12:\n\x11\x63hange_tile_infos\x18\x03 \x03(\x0b\x32\x1f.lq.RecordChangeTile.ChangeTile\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0b\x63hange_type\x18\x05 \x01(\r\x12-\n\noperations\x18\x06 \x03(\x0b\x32\x19.lq.OptionalOperationList\x1a;\n\x07TingPai\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\ttingpais1\x18\x02 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x1a\x62\n\nChangeTile\x12\x10\n\x08in_tiles\x18\x01 \x03(\t\x12\x16\n\x0ein_tile_states\x18\x02 \x03(\x05\x12\x11\n\tout_tiles\x18\x03 \x03(\t\x12\x17\n\x0fout_tile_states\x18\x04 \x03(\x05\"\x83\x02\n\x11\x41\x63tionDiscardTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x0f\n\x07is_liqi\x18\x03 \x01(\x08\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x10\n\x08zhenting\x18\x06 \x01(\x08\x12!\n\x08tingpais\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08is_wliqi\x18\t \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x84\x02\n\x11RecordDiscardTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x0f\n\x07is_liqi\x18\x03 \x01(\x08\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x10\n\x08zhenting\x18\x06 \x03(\x08\x12!\n\x08tingpais\x18\x07 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05\x64oras\x18\x08 \x03(\t\x12\x10\n\x08is_wliqi\x18\t \x01(\x08\x12-\n\noperations\x18\n \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\x12\n\ntile_state\x18\x0b \x01(\r\x12\x1a\n\x04muyu\x18\x0c \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x8d\x02\n\x0e\x41\x63tionDealTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x03 \x01(\r\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12(\n\x08tingpais\x18\x08 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\x12\n\ntile_state\x18\t \x01(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xe3\x01\n\x0eRecordDealTile\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04tile\x18\x02 \x01(\t\x12\x17\n\x0fleft_tile_count\x18\x03 \x01(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x03(\x08\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x12\n\ntile_state\x18\t \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x87\x02\n\x11\x41\x63tionChiPengGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x03(\t\x12\r\n\x05\x66roms\x18\x04 \x03(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12,\n\toperation\x18\x06 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12(\n\x08tingpais\x18\x08 \x03(\x0b\x32\x16.lq.TingPaiDiscardInfo\x12\x13\n\x0btile_states\x18\t \x03(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xdd\x01\n\x11RecordChiPengGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x03(\t\x12\r\n\x05\x66roms\x18\x04 \x03(\r\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\x07 \x03(\x08\x12,\n\toperation\x18\x08 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\x13\n\x0btile_states\x18\t \x03(\r\x12\x1a\n\x04muyu\x18\n \x01(\x0b\x32\x0c.lq.MuyuInfo\"7\n\x10\x41\x63tionGangResult\x12#\n\ngang_infos\x18\x01 \x01(\x0b\x32\x0f.lq.ChuanmaGang\"7\n\x10RecordGangResult\x12#\n\ngang_infos\x18\x01 \x01(\x0b\x32\x0f.lq.ChuanmaGang\":\n\x13\x41\x63tionGangResultEnd\x12#\n\ngang_infos\x18\x01 \x01(\x0b\x32\x0f.lq.ChuanmaGang\":\n\x13RecordGangResultEnd\x12#\n\ngang_infos\x18\x01 \x01(\x0b\x32\x0f.lq.ChuanmaGang\"\xce\x01\n\x13\x41\x63tionAnGangAddGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x01(\t\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12!\n\x08tingpais\x18\x08 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\x1a\n\x04muyu\x18\t \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x9a\x01\n\x13RecordAnGangAddGang\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05tiles\x18\x03 \x01(\t\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12-\n\noperations\x18\x07 \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xcc\x01\n\x0b\x41\x63tionBaBei\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12,\n\toperation\x18\x04 \x01(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\x10\n\x08zhenting\x18\x07 \x01(\x08\x12!\n\x08tingpais\x18\x08 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\r\n\x05moqie\x18\t \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\x98\x01\n\x0bRecordBaBei\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12-\n\noperations\x18\x07 \x03(\x0b\x32\x19.lq.OptionalOperationList\x12\r\n\x05moqie\x18\x08 \x01(\x08\x12\x12\n\ntile_state\x18\n \x01(\r\x12\x1a\n\x04muyu\x18\x0b \x01(\x0b\x32\x0c.lq.MuyuInfo\"\xd2\x01\n\nActionHule\x12\x1b\n\x05hules\x18\x01 \x03(\x0b\x32\x0c.lq.HuleInfo\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x0e\n\x06\x62\x61opai\x18\t \x01(\x05\"\xd2\x01\n\nRecordHule\x12\x1b\n\x05hules\x18\x01 \x03(\x0b\x32\x0c.lq.HuleInfo\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x04 \x01(\r\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x0e\n\x06\x62\x61opai\x18\t \x01(\x05\"\xc6\x01\n\x10HuInfoXueZhanMid\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x12\n\nhand_count\x18\x02 \x01(\r\x12\x0c\n\x04hand\x18\x03 \x03(\t\x12\x0c\n\x04ming\x18\x04 \x03(\t\x12\x0f\n\x07hu_tile\x18\x05 \x01(\t\x12\x0c\n\x04zimo\x18\x06 \x01(\x08\x12\r\n\x05yiman\x18\x07 \x01(\x08\x12\r\n\x05\x63ount\x18\x08 \x01(\r\x12\x19\n\x04\x66\x61ns\x18\t \x03(\x0b\x32\x0b.lq.FanInfo\x12\n\n\x02\x66u\x18\n \x01(\r\x12\x10\n\x08title_id\x18\x0b \x01(\r\"\xd1\x01\n\x14\x41\x63tionHuleXueZhanMid\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x1d\n\x04liqi\x18\t \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\n \x01(\x08\"\xd1\x01\n\x14RecordHuleXueZhanMid\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x05 \x03(\x05\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12\x1d\n\x04liqi\x18\t \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x10\n\x08zhenting\x18\n \x03(\x08\"\xf9\x01\n\x14\x41\x63tionHuleXueZhanEnd\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x04 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x05 \x01(\r\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xf9\x01\n\x14RecordHuleXueZhanEnd\x12#\n\x05hules\x18\x01 \x03(\x0b\x32\x14.lq.HuInfoXueZhanMid\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0e\n\x06scores\x18\x04 \x03(\x05\x12\x14\n\x0cwait_timeout\x18\x05 \x01(\r\x12\x1c\n\x07gameend\x18\x06 \x01(\x0b\x32\x0b.lq.GameEnd\x12\r\n\x05\x64oras\x18\x07 \x03(\t\x12\x1a\n\x04muyu\x18\x08 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xce\x01\n\x0b\x41\x63tionLiuJu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x1c\n\x07gameend\x18\x02 \x01(\x0b\x32\x0b.lq.GameEnd\x12\x0c\n\x04seat\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x16\n\x0e\x61llplayertiles\x18\x06 \x03(\t\x12\x1a\n\x04muyu\x18\x07 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xce\x01\n\x0bRecordLiuJu\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x1c\n\x07gameend\x18\x02 \x01(\x0b\x32\x0b.lq.GameEnd\x12\x0c\n\x04seat\x18\x03 \x01(\r\x12\r\n\x05tiles\x18\x04 \x03(\t\x12\x1d\n\x04liqi\x18\x05 \x01(\x0b\x32\x0f.lq.LiQiSuccess\x12\x16\n\x0e\x61llplayertiles\x18\x06 \x03(\t\x12\x1a\n\x04muyu\x18\x07 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"g\n\x10NoTilePlayerInfo\x12\x0f\n\x07tingpai\x18\x03 \x01(\x08\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12\x1e\n\x05tings\x18\x05 \x03(\x0b\x32\x0f.lq.TingPaiInfo\x12\x14\n\x0c\x61lready_hule\x18\x06 \x01(\x08\"\xa1\x01\n\x0fNoTileScoreInfo\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x12\n\nold_scores\x18\x02 \x03(\x05\x12\x14\n\x0c\x64\x65lta_scores\x18\x03 \x03(\x05\x12\x0c\n\x04hand\x18\x04 \x03(\t\x12\x0c\n\x04ming\x18\x05 \x03(\t\x12\r\n\x05\x64oras\x18\x06 \x03(\t\x12\r\n\x05score\x18\x07 \x01(\r\x12\r\n\x05taxes\x18\x08 \x03(\x05\x12\r\n\x05lines\x18\t \x03(\t\"\xc2\x01\n\x0c\x41\x63tionNoTile\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12%\n\x07players\x18\x02 \x03(\x0b\x32\x14.lq.NoTilePlayerInfo\x12#\n\x06scores\x18\x03 \x03(\x0b\x32\x13.lq.NoTileScoreInfo\x12\x0f\n\x07gameend\x18\x04 \x01(\x08\x12\x1a\n\x04muyu\x18\x05 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\xc2\x01\n\x0cRecordNoTile\x12\x14\n\x0cliujumanguan\x18\x01 \x01(\x08\x12%\n\x07players\x18\x02 \x03(\x0b\x32\x14.lq.NoTilePlayerInfo\x12#\n\x06scores\x18\x03 \x03(\x0b\x32\x13.lq.NoTileScoreInfo\x12\x0f\n\x07gameend\x18\x04 \x01(\x08\x12\x1a\n\x04muyu\x18\x05 \x01(\x0b\x32\x0c.lq.MuyuInfo\x12#\n\rhules_history\x18\t \x03(\x0b\x32\x0c.lq.HuleInfo\"\x1d\n\rPlayerLeaving\x12\x0c\n\x04seat\x18\x01 \x01(\r\"C\n\x0bReqAuthGame\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tgame_uuid\x18\x03 \x01(\t\"\xb2\x01\n\x0bResAuthGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12#\n\x07players\x18\x02 \x03(\x0b\x32\x12.lq.PlayerGameView\x12\x11\n\tseat_list\x18\x03 \x03(\r\x12\x15\n\ris_game_start\x18\x04 \x01(\x08\x12#\n\x0bgame_config\x18\x05 \x01(\x0b\x32\x0e.lq.GameConfig\x12\x15\n\rready_id_list\x18\x06 \x03(\r\"\xb8\x01\n\x0bGameRestore\x12\"\n\x08snapshot\x18\x01 \x01(\x0b\x32\x10.lq.GameSnapshot\x12$\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32\x13.lq.ActionPrototype\x12\x1b\n\x13passed_waiting_time\x18\x03 \x01(\r\x12\x12\n\ngame_state\x18\x04 \x01(\r\x12\x12\n\nstart_time\x18\x05 \x01(\r\x12\x1a\n\x12last_pause_time_ms\x18\x06 \x01(\r\"m\n\x0cResEnterGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0e\n\x06is_end\x18\x02 \x01(\x08\x12\x0c\n\x04step\x18\x03 \x01(\r\x12%\n\x0cgame_restore\x18\x04 \x01(\x0b\x32\x0f.lq.GameRestore\"-\n\x0bReqSyncGame\x12\x10\n\x08round_id\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\r\"l\n\x0bResSyncGame\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\x0e\n\x06is_end\x18\x02 \x01(\x08\x12\x0c\n\x04step\x18\x03 \x01(\r\x12%\n\x0cgame_restore\x18\x04 \x01(\x0b\x32\x0f.lq.GameRestore\"\xc8\x01\n\x10ReqSelfOperation\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05index\x18\x02 \x01(\r\x12\x0c\n\x04tile\x18\x03 \x01(\t\x12\x18\n\x10\x63\x61ncel_operation\x18\x04 \x01(\x08\x12\r\n\x05moqie\x18\x05 \x01(\x08\x12\x0f\n\x07timeuse\x18\x06 \x01(\r\x12\x12\n\ntile_state\x18\x07 \x01(\x05\x12\x14\n\x0c\x63hange_tiles\x18\x08 \x03(\t\x12\x13\n\x0btile_states\x18\t \x03(\x05\x12\x10\n\x08gap_type\x18\n \x01(\r\"X\n\x0eReqChiPengGang\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\r\n\x05index\x18\x02 \x01(\r\x12\x18\n\x10\x63\x61ncel_operation\x18\x03 \x01(\x08\x12\x0f\n\x07timeuse\x18\x06 \x01(\r\":\n\x12ReqBroadcastInGame\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\x12\x13\n\x0b\x65xcept_self\x18\x02 \x01(\x08\")\n\x14ReqGMCommandInGaming\x12\x11\n\tjson_data\x18\x01 \x01(\t\"W\n\x12ResGamePlayerState\x12\x18\n\x05\x65rror\x18\x01 \x01(\x0b\x32\t.lq.Error\x12\'\n\nstate_list\x18\x02 \x03(\x0e\x32\x13.lq.GamePlayerState\"\x1d\n\x0eReqVoteGameEnd\x12\x0b\n\x03yes\x18\x01 \x01(\x08\"U\n\x0eResGameEndVote\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x18\n\x10vote_cd_end_time\x18\x02 \x01(\r\x12\x18\n\x05\x65rror\x18\x03 \x01(\x0b\x32\t.lq.Error\"\x1f\n\x0eReqAuthObserve\x12\r\n\x05token\x18\x01 \x01(\t\"V\n\x0fResStartObserve\x12\x1e\n\x04head\x18\x01 \x01(\x0b\x32\x10.lq.GameLiveHead\x12#\n\x06passed\x18\x02 \x01(\x0b\x32\x13.lq.GameLiveSegment\"7\n\rNotifyNewGame\x12\x11\n\tgame_uuid\x18\x01 \x01(\t\x12\x13\n\x0bplayer_list\x18\x02 \x03(\t\"2\n\x19NotifyPlayerLoadGameReady\x12\x15\n\rready_id_list\x18\x01 \x03(\r\"4\n\x13NotifyGameBroadcast\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"8\n\x13NotifyGameEndResult\x12!\n\x06result\x18\x01 \x01(\x0b\x32\x11.lq.GameEndResult\"%\n\x13NotifyGameTerminate\x12\x0e\n\x06reason\x18\x01 \x01(\t\"O\n\x1bNotifyPlayerConnectionState\x12\x0c\n\x04seat\x18\x01 \x01(\r\x12\"\n\x05state\x18\x02 \x01(\x0e\x32\x13.lq.GamePlayerState\"k\n\x18NotifyAccountLevelChange\x12 \n\x06origin\x18\x01 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x1f\n\x05\x66inal\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x0c\n\x04type\x18\x03 \x01(\r\"\x84\x05\n\x16NotifyGameFinishReward\x12\x0f\n\x07mode_id\x18\x01 \x01(\r\x12<\n\x0clevel_change\x18\x02 \x01(\x0b\x32&.lq.NotifyGameFinishReward.LevelChange\x12:\n\x0bmatch_chest\x18\x03 \x01(\x0b\x32%.lq.NotifyGameFinishReward.MatchChest\x12@\n\x0emain_character\x18\x04 \x01(\x0b\x32(.lq.NotifyGameFinishReward.MainCharacter\x12@\n\x0e\x63haracter_gift\x18\x05 \x01(\x0b\x32(.lq.NotifyGameFinishReward.CharacterGift\x1a^\n\x0bLevelChange\x12 \n\x06origin\x18\x01 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x1f\n\x05\x66inal\x18\x02 \x01(\x0b\x32\x10.lq.AccountLevel\x12\x0c\n\x04type\x18\x03 \x01(\r\x1aq\n\nMatchChest\x12\x10\n\x08\x63hest_id\x18\x01 \x01(\r\x12\x0e\n\x06origin\x18\x02 \x01(\r\x12\r\n\x05\x66inal\x18\x03 \x01(\r\x12\x11\n\tis_graded\x18\x04 \x01(\x08\x12\x1f\n\x07rewards\x18\x05 \x03(\x0b\x32\x0e.lq.RewardSlot\x1a\x38\n\rMainCharacter\x12\r\n\x05level\x18\x01 \x01(\r\x12\x0b\n\x03\x65xp\x18\x02 \x01(\r\x12\x0b\n\x03\x61\x64\x64\x18\x03 \x01(\r\x1aN\n\rCharacterGift\x12\x0e\n\x06origin\x18\x01 \x01(\r\x12\r\n\x05\x66inal\x18\x02 \x01(\r\x12\x0b\n\x03\x61\x64\x64\x18\x03 \x01(\r\x12\x11\n\tis_graded\x18\x04 \x01(\x08\"\xa0\x01\n\x14NotifyActivityReward\x12@\n\x0f\x61\x63tivity_reward\x18\x01 \x03(\x0b\x32\'.lq.NotifyActivityReward.ActivityReward\x1a\x46\n\x0e\x41\x63tivityReward\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\x1f\n\x07rewards\x18\x02 \x03(\x0b\x32\x0e.lq.RewardSlot\"\x8a\x01\n\x13NotifyActivityPoint\x12>\n\x0f\x61\x63tivity_points\x18\x01 \x03(\x0b\x32%.lq.NotifyActivityPoint.ActivityPoint\x1a\x33\n\rActivityPoint\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"\x9c\x01\n\x16NotifyLeaderboardPoint\x12G\n\x12leaderboard_points\x18\x01 \x03(\x0b\x32+.lq.NotifyLeaderboardPoint.LeaderboardPoint\x1a\x39\n\x10LeaderboardPoint\x12\x16\n\x0eleaderboard_id\x18\x01 \x01(\r\x12\r\n\x05point\x18\x02 \x01(\r\"!\n\x0fNotifyGamePause\x12\x0e\n\x06paused\x18\x01 \x01(\x08\"\xa0\x01\n\x11NotifyEndGameVote\x12\x31\n\x07results\x18\x01 \x03(\x0b\x32 .lq.NotifyEndGameVote.VoteResult\x12\x12\n\nstart_time\x18\x02 \x01(\r\x12\x15\n\rduration_time\x18\x03 \x01(\r\x1a-\n\nVoteResult\x12\x12\n\naccount_id\x18\x01 \x01(\r\x12\x0b\n\x03yes\x18\x02 \x01(\x08\"3\n\x11NotifyObserveData\x12\x1e\n\x04unit\x18\x01 \x01(\x0b\x32\x10.lq.GameLiveUnit*=\n\x0fGamePlayerState\x12\x08\n\x04NULL\x10\x00\x12\x08\n\x04\x41UTH\x10\x01\x12\x0b\n\x07SYNCING\x10\x02\x12\t\n\x05READY\x10\x03\x32\xd4x\n\x05Lobby\x12;\n\x13\x66\x65tchConnectionInfo\x12\r.lq.ReqCommon\x1a\x15.lq.ResConnectionInfo\x12\x34\n\x06signup\x12\x14.lq.ReqSignupAccount\x1a\x14.lq.ResSignupAccount\x12#\n\x05login\x12\x0c.lq.ReqLogin\x1a\x0c.lq.ResLogin\x12,\n\x0cloginSuccess\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\nemailLogin\x12\x11.lq.ReqEmailLogin\x1a\x0c.lq.ResLogin\x12\x32\n\noauth2Auth\x12\x11.lq.ReqOauth2Auth\x1a\x11.lq.ResOauth2Auth\x12\x35\n\x0boauth2Check\x12\x12.lq.ReqOauth2Check\x1a\x12.lq.ResOauth2Check\x12\x38\n\x0coauth2Signup\x12\x13.lq.ReqOauth2Signup\x1a\x13.lq.ResOauth2Signup\x12/\n\x0boauth2Login\x12\x12.lq.ReqOauth2Login\x1a\x0c.lq.ResLogin\x12\x35\n\x0b\x64mmPreLogin\x12\x12.lq.ReqDMMPreLogin\x1a\x12.lq.ResDMMPreLogin\x12\x44\n\x15\x63reatePhoneVerifyCode\x12\x1c.lq.ReqCreatePhoneVerifyCode\x1a\r.lq.ResCommon\x12\x44\n\x15\x63reateEmailVerifyCode\x12\x1c.lq.ReqCreateEmailVerifyCode\x1a\r.lq.ResCommon\x12N\n\x14verfifyCodeForSecure\x12\x1a.lq.ReqVerifyCodeForSecure\x1a\x1a.lq.ResVerfiyCodeForSecure\x12\x38\n\x0f\x62indPhoneNumber\x12\x16.lq.ReqBindPhoneNumber\x1a\r.lq.ResCommon\x12<\n\x11unbindPhoneNumber\x12\x18.lq.ReqUnbindPhoneNumber\x1a\r.lq.ResCommon\x12@\n\x13\x66\x65tchPhoneLoginBind\x12\r.lq.ReqCommon\x1a\x1a.lq.ResFetchPhoneLoginBind\x12\x42\n\x14\x63reatePhoneLoginBind\x12\x1b.lq.ReqCreatePhoneLoginBind\x1a\r.lq.ResCommon\x12,\n\tbindEmail\x12\x10.lq.ReqBindEmail\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyPassword\x12\x15.lq.ReqModifyPassword\x1a\r.lq.ResCommon\x12\x30\n\x0b\x62indAccount\x12\x12.lq.ReqBindAccount\x1a\r.lq.ResCommon\x12&\n\x06logout\x12\r.lq.ReqLogout\x1a\r.lq.ResLogout\x12*\n\x08heatbeat\x12\x0f.lq.ReqHeatBeat\x1a\r.lq.ResCommon\x12,\n\tloginBeat\x12\x10.lq.ReqLoginBeat\x1a\r.lq.ResCommon\x12\x36\n\x0e\x63reateNickname\x12\x15.lq.ReqCreateNickname\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyNickname\x12\x15.lq.ReqModifyNickname\x1a\r.lq.ResCommon\x12\x36\n\x0emodifyBirthday\x12\x15.lq.ReqModifyBirthday\x1a\r.lq.ResCommon\x12+\n\tfetchRoom\x12\r.lq.ReqCommon\x1a\x0f.lq.ResSelfRoom\x12\x32\n\ncreateRoom\x12\x11.lq.ReqCreateRoom\x1a\x11.lq.ResCreateRoom\x12,\n\x08joinRoom\x12\x0f.lq.ReqJoinRoom\x1a\x0f.lq.ResJoinRoom\x12)\n\tleaveRoom\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12,\n\treadyPlay\x12\x10.lq.ReqRoomReady\x1a\r.lq.ResCommon\x12\x34\n\x0e\x64ressingStatus\x12\x13.lq.ReqRoomDressing\x1a\r.lq.ResCommon\x12,\n\tstartRoom\x12\x10.lq.ReqRoomStart\x1a\r.lq.ResCommon\x12,\n\nkickPlayer\x12\x0f.lq.ReqRoomKick\x1a\r.lq.ResCommon\x12.\n\nmodifyRoom\x12\x11.lq.ReqModifyRoom\x1a\r.lq.ResCommon\x12\x31\n\tmatchGame\x12\x15.lq.ReqJoinMatchQueue\x1a\r.lq.ResCommon\x12\x35\n\x0b\x63\x61ncelMatch\x12\x17.lq.ReqCancelMatchQueue\x1a\r.lq.ResCommon\x12:\n\x10\x66\x65tchAccountInfo\x12\x12.lq.ReqAccountInfo\x1a\x12.lq.ResAccountInfo\x12\x32\n\x0c\x63hangeAvatar\x12\x13.lq.ReqChangeAvatar\x1a\r.lq.ResCommon\x12\x34\n\x14receiveVersionReward\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12U\n\x19\x66\x65tchAccountStatisticInfo\x12\x1b.lq.ReqAccountStatisticInfo\x1a\x1b.lq.ResAccountStatisticInfo\x12T\n\x1d\x66\x65tchAccountChallengeRankInfo\x12\x12.lq.ReqAccountInfo\x1a\x1f.lq.ResAccountChallengeRankInfo\x12G\n\x19\x66\x65tchAccountCharacterInfo\x12\r.lq.ReqCommon\x1a\x1b.lq.ResAccountCharacterInfo\x12\x38\n\x0cshopPurchase\x12\x13.lq.ReqShopPurchase\x1a\x13.lq.ResShopPurchase\x12\x37\n\x0f\x66\x65tchGameRecord\x12\x11.lq.ReqGameRecord\x1a\x11.lq.ResGameRecord\x12\x32\n\x0ereadGameRecord\x12\x11.lq.ReqGameRecord\x1a\r.lq.ResCommon\x12\x43\n\x13\x66\x65tchGameRecordList\x12\x15.lq.ReqGameRecordList\x1a\x15.lq.ResGameRecordList\x12M\n\x1c\x66\x65tchCollectedGameRecordList\x12\r.lq.ReqCommon\x1a\x1e.lq.ResCollectedGameRecordList\x12L\n\x16\x66\x65tchGameRecordsDetail\x12\x18.lq.ReqGameRecordsDetail\x1a\x18.lq.ResGameRecordsDetail\x12V\n\x16\x61\x64\x64\x43ollectedGameRecord\x12\x1d.lq.ReqAddCollectedGameRecord\x1a\x1d.lq.ResAddCollectedGameRecord\x12_\n\x19removeCollectedGameRecord\x12 .lq.ReqRemoveCollectedGameRecord\x1a .lq.ResRemoveCollectedGameRecord\x12t\n changeCollectedGameRecordRemarks\x12\'.lq.ReqChangeCollectedGameRecordRemarks\x1a\'.lq.ResChangeCollectedGameRecordRemarks\x12I\n\x15\x66\x65tchLevelLeaderboard\x12\x17.lq.ReqLevelLeaderboard\x1a\x17.lq.ResLevelLeaderboard\x12U\n\x19\x66\x65tchChallengeLeaderboard\x12\x1b.lq.ReqChallangeLeaderboard\x1a\x1b.lq.ResChallengeLeaderboard\x12O\n\x17\x66\x65tchMutiChallengeLevel\x12\x19.lq.ReqMutiChallengeLevel\x1a\x19.lq.ResMutiChallengeLevel\x12I\n\x16\x66\x65tchMultiAccountBrief\x12\x15.lq.ReqMultiAccountId\x1a\x18.lq.ResMultiAccountBrief\x12\x33\n\x0f\x66\x65tchFriendList\x12\r.lq.ReqCommon\x1a\x11.lq.ResFriendList\x12=\n\x14\x66\x65tchFriendApplyList\x12\r.lq.ReqCommon\x1a\x16.lq.ResFriendApplyList\x12\x30\n\x0b\x61pplyFriend\x12\x12.lq.ReqApplyFriend\x1a\r.lq.ResCommon\x12<\n\x11handleFriendApply\x12\x18.lq.ReqHandleFriendApply\x1a\r.lq.ResCommon\x12\x32\n\x0cremoveFriend\x12\x13.lq.ReqRemoveFriend\x1a\r.lq.ResCommon\x12G\n\x11searchAccountById\x12\x18.lq.ReqSearchAccountById\x1a\x18.lq.ResSearchAccountById\x12V\n\x16searchAccountByPattern\x12\x1d.lq.ReqSearchAccountByPattern\x1a\x1d.lq.ResSearchAccountByPattern\x12=\n\x11\x66\x65tchAccountState\x12\x12.lq.ReqAccountList\x1a\x14.lq.ResAccountStates\x12-\n\x0c\x66\x65tchBagInfo\x12\r.lq.ReqCommon\x1a\x0e.lq.ResBagInfo\x12.\n\nuseBagItem\x12\x11.lq.ReqUseBagItem\x1a\r.lq.ResCommon\x12\x36\n\x0eopenManualItem\x12\x15.lq.ReqOpenManualItem\x1a\r.lq.ResCommon\x12P\n\x14openRandomRewardItem\x12\x1b.lq.ReqOpenRandomRewardItem\x1a\x1b.lq.ResOpenRandomRewardItem\x12G\n\x11openAllRewardItem\x12\x18.lq.ReqOpenAllRewardItem\x1a\x18.lq.ResOpenAllRewardItem\x12\x32\n\x0c\x63omposeShard\x12\x13.lq.ReqComposeShard\x1a\r.lq.ResCommon\x12\x42\n\x11\x66\x65tchAnnouncement\x12\x18.lq.ReqFetchAnnouncement\x1a\x13.lq.ResAnnouncement\x12:\n\x10readAnnouncement\x12\x17.lq.ReqReadAnnouncement\x1a\r.lq.ResCommon\x12/\n\rfetchMailInfo\x12\r.lq.ReqCommon\x1a\x0f.lq.ResMailInfo\x12*\n\x08readMail\x12\x0f.lq.ReqReadMail\x1a\r.lq.ResCommon\x12.\n\ndeleteMail\x12\x11.lq.ReqDeleteMail\x1a\r.lq.ResCommon\x12>\n\x16takeAttachmentFromMail\x12\x15.lq.ReqTakeAttachment\x1a\r.lq.ResCommon\x12\\\n\x18receiveAchievementReward\x12\x1f.lq.ReqReceiveAchievementReward\x1a\x1f.lq.ResReceiveAchievementReward\x12k\n\x1dreceiveAchievementGroupReward\x12$.lq.ReqReceiveAchievementGroupReward\x1a$.lq.ResReceiveAchievementGroupReward\x12\x42\n\x14\x66\x65tchAchievementRate\x12\r.lq.ReqCommon\x1a\x1b.lq.ResFetchAchievementRate\x12\x35\n\x10\x66\x65tchAchievement\x12\r.lq.ReqCommon\x1a\x12.lq.ResAchievement\x12.\n\nbuyShiLian\x12\x11.lq.ReqBuyShiLian\x1a\r.lq.ResCommon\x12,\n\x0cmatchShiLian\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\rgoNextShiLian\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12<\n\x11updateClientValue\x12\x18.lq.ReqUpdateClientValue\x1a\r.lq.ResCommon\x12\x35\n\x10\x66\x65tchClientValue\x12\r.lq.ReqCommon\x1a\x12.lq.ResClientValue\x12\x34\n\rclientMessage\x12\x14.lq.ReqClientMessage\x1a\r.lq.ResCommon\x12I\n\x15\x66\x65tchCurrentMatchInfo\x12\x17.lq.ReqCurrentMatchInfo\x1a\x17.lq.ResCurrentMatchInfo\x12\x32\n\x0cuserComplain\x12\x13.lq.ReqUserComplain\x1a\r.lq.ResCommon\x12;\n\x13\x66\x65tchReviveCoinInfo\x12\r.lq.ReqCommon\x1a\x15.lq.ResReviveCoinInfo\x12.\n\x0egainReviveCoin\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x31\n\x0e\x66\x65tchDailyTask\x12\r.lq.ReqCommon\x1a\x10.lq.ResDailyTask\x12\x44\n\x10refreshDailyTask\x12\x17.lq.ReqRefreshDailyTask\x1a\x17.lq.ResRefreshDailyTask\x12\x35\n\x0buseGiftCode\x12\x12.lq.ReqUseGiftCode\x1a\x12.lq.ResUseGiftCode\x12\x43\n\x12useSpecialGiftCode\x12\x12.lq.ReqUseGiftCode\x1a\x19.lq.ResUseSpecialGiftCode\x12\x31\n\x0e\x66\x65tchTitleList\x12\r.lq.ReqCommon\x1a\x10.lq.ResTitleList\x12*\n\x08useTitle\x12\x0f.lq.ReqUseTitle\x1a\r.lq.ResCommon\x12<\n\x11sendClientMessage\x12\x18.lq.ReqSendClientMessage\x1a\r.lq.ResCommon\x12=\n\x11\x66\x65tchGameLiveInfo\x12\x13.lq.ReqGameLiveInfo\x1a\x13.lq.ResGameLiveInfo\x12R\n\x18\x66\x65tchGameLiveLeftSegment\x12\x1a.lq.ReqGameLiveLeftSegment\x1a\x1a.lq.ResGameLiveLeftSegment\x12=\n\x11\x66\x65tchGameLiveList\x12\x13.lq.ReqGameLiveList\x1a\x13.lq.ResGameLiveList\x12;\n\x13\x66\x65tchCommentSetting\x12\r.lq.ReqCommon\x1a\x15.lq.ResCommentSetting\x12\x42\n\x14updateCommentSetting\x12\x1b.lq.ReqUpdateCommentSetting\x1a\r.lq.ResCommon\x12\x44\n\x10\x66\x65tchCommentList\x12\x17.lq.ReqFetchCommentList\x1a\x17.lq.ResFetchCommentList\x12M\n\x13\x66\x65tchCommentContent\x12\x1a.lq.ReqFetchCommentContent\x1a\x1a.lq.ResFetchCommentContent\x12\x32\n\x0cleaveComment\x12\x13.lq.ReqLeaveComment\x1a\r.lq.ResCommon\x12\x34\n\rdeleteComment\x12\x14.lq.ReqDeleteComment\x1a\r.lq.ResCommon\x12<\n\x11updateReadComment\x12\x18.lq.ReqUpdateReadComment\x1a\r.lq.ResCommon\x12\x39\n\x12\x66\x65tchRollingNotice\x12\r.lq.ReqCommon\x1a\x14.lq.ReqRollingNotice\x12\x33\n\x0f\x66\x65tchServerTime\x12\r.lq.ReqCommon\x1a\x11.lq.ResServerTime\x12W\n\x15\x66\x65tchPlatformProducts\x12\x1e.lq.ReqPlatformBillingProducts\x1a\x1e.lq.ResPlatformBillingProducts\x12\x44\n\x15\x63\x61ncelGooglePlayOrder\x12\x1c.lq.ReqCancelGooglePlayOrder\x1a\r.lq.ResCommon\x12/\n\topenChest\x12\x10.lq.ReqOpenChest\x1a\x10.lq.ResOpenChest\x12\x44\n\x10\x62uyFromChestShop\x12\x17.lq.ReqBuyFromChestShop\x1a\x17.lq.ResBuyFromChestShop\x12=\n\x14\x66\x65tchDailySignInInfo\x12\r.lq.ReqCommon\x1a\x16.lq.ResDailySignInInfo\x12-\n\rdoDailySignIn\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x44\n\x10\x64oActivitySignIn\x12\x17.lq.ReqDoActivitySignIn\x1a\x17.lq.ResDoActivitySignIn\x12\x39\n\x12\x66\x65tchCharacterInfo\x12\r.lq.ReqCommon\x1a\x14.lq.ResCharacterInfo\x12@\n\x13updateCharacterSort\x12\x1a.lq.ReqUpdateCharacterSort\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeMainCharacter\x12\x1a.lq.ReqChangeMainCharacter\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeCharacterSkin\x12\x1a.lq.ReqChangeCharacterSkin\x1a\r.lq.ResCommon\x12@\n\x13\x63hangeCharacterView\x12\x1a.lq.ReqChangeCharacterView\x1a\r.lq.ResCommon\x12M\n\x13sendGiftToCharacter\x12\x1a.lq.ReqSendGiftToCharacter\x1a\x1a.lq.ResSendGiftToCharacter\x12*\n\x08sellItem\x12\x0f.lq.ReqSellItem\x1a\r.lq.ResCommon\x12\x33\n\x0f\x66\x65tchCommonView\x12\r.lq.ReqCommon\x1a\x11.lq.ResCommonView\x12:\n\x10\x63hangeCommonView\x12\x17.lq.ReqChangeCommonView\x1a\r.lq.ResCommon\x12\x38\n\x0fsaveCommonViews\x12\x16.lq.ReqSaveCommonViews\x1a\r.lq.ResCommon\x12:\n\x10\x66\x65tchCommonViews\x12\x12.lq.ReqCommonViews\x1a\x12.lq.ResCommonViews\x12;\n\x13\x66\x65tchAllCommonViews\x12\r.lq.ReqCommon\x1a\x15.lq.ResAllcommonViews\x12\x34\n\ruseCommonView\x12\x14.lq.ReqUseCommonView\x1a\r.lq.ResCommon\x12\x44\n\x10upgradeCharacter\x12\x17.lq.ReqUpgradeCharacter\x1a\x17.lq.ResUpgradeCharacter\x12\x39\n\x11\x61\x64\x64\x46inishedEnding\x12\x15.lq.ReqFinishedEnding\x1a\r.lq.ResCommon\x12;\n\x13receiveEndingReward\x12\x15.lq.ReqFinishedEnding\x1a\r.lq.ResCommon\x12\x34\n\x11gameMasterCommand\x12\x10.lq.ReqGMCommand\x1a\r.lq.ResCommon\x12/\n\rfetchShopInfo\x12\r.lq.ReqCommon\x1a\x0f.lq.ResShopInfo\x12\x35\n\x0b\x62uyFromShop\x12\x12.lq.ReqBuyFromShop\x1a\x12.lq.ResBuyFromShop\x12.\n\nbuyFromZHP\x12\x11.lq.ReqBuyFromZHP\x1a\r.lq.ResCommon\x12;\n\x0erefreshZHPShop\x12\x12.lq.ReqReshZHPShop\x1a\x15.lq.ResRefreshZHPShop\x12=\n\x14\x66\x65tchMonthTicketInfo\x12\r.lq.ReqCommon\x1a\x16.lq.ResMonthTicketInfo\x12>\n\x0epayMonthTicket\x12\x15.lq.ReqPayMonthTicket\x1a\x15.lq.ResPayMonthTicket\x12:\n\x10\x65xchangeCurrency\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12<\n\x12\x65xchangeChestStone\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12\x39\n\x0f\x65xchangeDiamond\x12\x17.lq.ReqExchangeCurrency\x1a\r.lq.ResCommon\x12;\n\x13\x66\x65tchServerSettings\x12\r.lq.ReqCommon\x1a\x15.lq.ResServerSettings\x12=\n\x14\x66\x65tchAccountSettings\x12\r.lq.ReqCommon\x1a\x16.lq.ResAccountSettings\x12\x44\n\x15updateAccountSettings\x12\x1c.lq.ReqUpdateAccountSettings\x1a\r.lq.ResCommon\x12=\n\x14\x66\x65tchModNicknameTime\x12\r.lq.ReqCommon\x1a\x16.lq.ResModNicknameTime\x12Y\n\x17\x63reateWechatNativeOrder\x12\x1e.lq.ReqCreateWechatNativeOrder\x1a\x1e.lq.ResCreateWechatNativeOrder\x12P\n\x14\x63reateWechatAppOrder\x12\x1b.lq.ReqCreateWechatAppOrder\x1a\x1b.lq.ResCreateWechatAppOrder\x12G\n\x11\x63reateAlipayOrder\x12\x18.lq.ReqCreateAlipayOrder\x1a\x18.lq.ResCreateAlipayOrder\x12S\n\x15\x63reateAlipayScanOrder\x12\x1c.lq.ReqCreateAlipayScanOrder\x1a\x1c.lq.ResCreateAlipayScanOrder\x12P\n\x14\x63reateAlipayAppOrder\x12\x1b.lq.ReqCreateAlipayAppOrder\x1a\x1b.lq.ResCreateAlipayAppOrder\x12Y\n\x17\x63reateJPCreditCardOrder\x12\x1e.lq.ReqCreateJPCreditCardOrder\x1a\x1e.lq.ResCreateJPCreditCardOrder\x12M\n\x13\x63reateJPPaypalOrder\x12\x1a.lq.ReqCreateJPPaypalOrder\x1a\x1a.lq.ResCreateJPPaypalOrder\x12\x41\n\x0f\x63reateJPAuOrder\x12\x16.lq.ReqCreateJPAuOrder\x1a\x16.lq.ResCreateJPAuOrder\x12M\n\x13\x63reateJPDocomoOrder\x12\x1a.lq.ReqCreateJPDocomoOrder\x1a\x1a.lq.ResCreateJPDocomoOrder\x12S\n\x15\x63reateJPWebMoneyOrder\x12\x1c.lq.ReqCreateJPWebMoneyOrder\x1a\x1c.lq.ResCreateJPWebMoneyOrder\x12S\n\x15\x63reateJPSoftbankOrder\x12\x1c.lq.ReqCreateJPSoftbankOrder\x1a\x1c.lq.ResCreateJPSoftbankOrder\x12M\n\x13\x63reateENPaypalOrder\x12\x1a.lq.ReqCreateENPaypalOrder\x1a\x1a.lq.ResCreateENPaypalOrder\x12Y\n\x17\x63reateENMasterCardOrder\x12\x1e.lq.ReqCreateENMasterCardOrder\x1a\x1e.lq.ResCreateENMasterCardOrder\x12G\n\x11\x63reateENVisaOrder\x12\x18.lq.ReqCreateENVisaOrder\x1a\x18.lq.ResCreateENVisaOrder\x12\x44\n\x10\x63reateENJCBOrder\x12\x17.lq.ReqCreateENJCBOrder\x1a\x17.lq.ResCreateENJCBOrder\x12M\n\x13\x63reateENAlipayOrder\x12\x1a.lq.ReqCreateENAlipayOrder\x1a\x1a.lq.ResCreateENAlipayOrder\x12>\n\x0e\x63reateDMMOrder\x12\x15.lq.ReqCreateDMMOrder\x1a\x15.lq.ResCreateDmmOrder\x12>\n\x0e\x63reateIAPOrder\x12\x15.lq.ReqCreateIAPOrder\x1a\x15.lq.ResCreateIAPOrder\x12\x44\n\x10\x63reateSteamOrder\x12\x17.lq.ReqCreateSteamOrder\x1a\x17.lq.ResCreateSteamOrder\x12:\n\x10verifySteamOrder\x12\x17.lq.ReqVerifySteamOrder\x1a\r.lq.ResCommon\x12N\n\x18\x63reateMyCardAndroidOrder\x12\x18.lq.ReqCreateMyCardOrder\x1a\x18.lq.ResCreateMyCardOrder\x12J\n\x14\x63reateMyCardWebOrder\x12\x18.lq.ReqCreateMyCardOrder\x1a\x18.lq.ResCreateMyCardOrder\x12G\n\x11\x63reatePaypalOrder\x12\x18.lq.ReqCreatePaypalOrder\x1a\x18.lq.ResCreatePaypalOrder\x12G\n\x11\x63reateXsollaOrder\x12\x18.lq.ReqCreateXsollaOrder\x1a\x18.lq.ResCreateXsollaOrder\x12<\n\x11verifyMyCardOrder\x12\x18.lq.ReqVerifyMyCardOrder\x1a\r.lq.ResCommon\x12P\n\x14verificationIAPOrder\x12\x1b.lq.ReqVerificationIAPOrder\x1a\x1b.lq.ResVerificationIAPOrder\x12J\n\x14\x63reateYostarSDKOrder\x12\x18.lq.ReqCreateYostarOrder\x1a\x18.lq.ResCreateYostarOrder\x12J\n\x12\x63reateBillingOrder\x12\x19.lq.ReqCreateBillingOrder\x1a\x19.lq.ResCreateBillingOrder\x12\x42\n\x14solveGooglePlayOrder\x12\x1b.lq.ReqSolveGooglePlayOrder\x1a\r.lq.ResCommon\x12\x45\n\x15solveGooglePayOrderV3\x12\x1d.lq.ReqSolveGooglePlayOrderV3\x1a\r.lq.ResCommon\x12\'\n\tfetchMisc\x12\r.lq.ReqCommon\x1a\x0b.lq.ResMisc\x12\x38\n\x0fmodifySignature\x12\x16.lq.ReqModifySignature\x1a\r.lq.ResCommon\x12\x33\n\x0f\x66\x65tchIDCardInfo\x12\r.lq.ReqCommon\x1a\x11.lq.ResIDCardInfo\x12:\n\x10updateIDCardInfo\x12\x17.lq.ReqUpdateIDCardInfo\x1a\r.lq.ResCommon\x12\x31\n\x0e\x66\x65tchVipReward\x12\r.lq.ReqCommon\x1a\x10.lq.ResVipReward\x12\x34\n\rgainVipReward\x12\x14.lq.ReqGainVipReward\x1a\r.lq.ResCommon\x12\x62\n\x1a\x66\x65tchCustomizedContestList\x12!.lq.ReqFetchCustomizedContestList\x1a!.lq.ResFetchCustomizedContestList\x12t\n fetchCustomizedContestExtendInfo\x12\'.lq.ReqFetchCustomizedContestExtendInfo\x1a\'.lq.ResFetchCustomizedContestExtendInfo\x12n\n\x1e\x66\x65tchCustomizedContestAuthInfo\x12%.lq.ReqFetchCustomizedContestAuthInfo\x1a%.lq.ResFetchCustomizedContestAuthInfo\x12V\n\x16\x65nterCustomizedContest\x12\x1d.lq.ReqEnterCustomizedContest\x1a\x1d.lq.ResEnterCustomizedContest\x12\x36\n\x16leaveCustomizedContest\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12t\n fetchCustomizedContestOnlineInfo\x12\'.lq.ReqFetchCustomizedContestOnlineInfo\x1a\'.lq.ResFetchCustomizedContestOnlineInfo\x12w\n!fetchCustomizedContestByContestId\x12(.lq.ReqFetchCustomizedContestByContestId\x1a(.lq.ResFetchCustomizedContestByContestId\x12\x46\n\x16startCustomizedContest\x12\x1d.lq.ReqStartCustomizedContest\x1a\r.lq.ResCommon\x12\x35\n\x15stopCustomizedContest\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12k\n\x1djoinCustomizedContestChatRoom\x12$.lq.ReqJoinCustomizedContestChatRoom\x1a$.lq.ResJoinCustomizedContestChatRoom\x12>\n\x1eleaveCustomizedContestChatRoom\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x36\n\x0esayChatMessage\x12\x15.lq.ReqSayChatMessage\x1a\r.lq.ResCommon\x12w\n!fetchCustomizedContestGameRecords\x12(.lq.ReqFetchCustomizedContestGameRecords\x1a(.lq.ResFetchCustomizedContestGameRecords\x12z\n\"fetchCustomizedContestGameLiveList\x12).lq.ReqFetchCustomizedContestGameLiveList\x1a).lq.ResFetchCustomizedContestGameLiveList\x12H\n\x17\x66ollowCustomizedContest\x12\x1e.lq.ReqTargetCustomizedContest\x1a\r.lq.ResCommon\x12J\n\x19unfollowCustomizedContest\x12\x1e.lq.ReqTargetCustomizedContest\x1a\r.lq.ResCommon\x12\x37\n\x11\x66\x65tchActivityList\x12\r.lq.ReqCommon\x1a\x13.lq.ResActivityList\x12\x45\n\x18\x66\x65tchAccountActivityData\x12\r.lq.ReqCommon\x1a\x1a.lq.ResAccountActivityData\x12P\n\x14\x65xchangeActivityItem\x12\x1b.lq.ReqExchangeActivityItem\x1a\x1b.lq.ResExchangeActivityItem\x12\x42\n\x14\x63ompleteActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12\x46\n\x18\x63ompleteActivityFlipTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12H\n\x1a\x63ompletePeriodActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12H\n\x1a\x63ompleteRandomActivityTask\x12\x1b.lq.ReqCompleteActivityTask\x1a\r.lq.ResCommon\x12Y\n\x17receiveActivityFlipTask\x12\x1e.lq.ReqReceiveActivityFlipTask\x1a\x1e.lq.ResReceiveActivityFlipTask\x12S\n\x15\x66\x65tchActivityFlipInfo\x12\x1c.lq.ReqFetchActivityFlipInfo\x1a\x1c.lq.ResFetchActivityFlipInfo\x12^\n\"gainAccumulatedPointActivityReward\x12).lq.ReqGainAccumulatedPointActivityReward\x1a\r.lq.ResCommon\x12R\n\x1cgainMultiPointActivityReward\x12#.lq.ReqGainMultiPointActivityReward\x1a\r.lq.ResCommon\x12_\n\x19\x66\x65tchRankPointLeaderboard\x12 .lq.ReqFetchRankPointLeaderboard\x1a .lq.ResFetchRankPointLeaderboard\x12@\n\x13gainRankPointReward\x12\x1a.lq.ReqGainRankPointReward\x1a\r.lq.ResCommon\x12I\n\x17richmanActivityNextMove\x12\x16.lq.ReqRichmanNextMove\x1a\x16.lq.ResRichmanNextMove\x12P\n\x1brichmanAcitivitySpecialMove\x12\x19.lq.ReqRichmanSpecialMove\x1a\x16.lq.ResRichmanNextMove\x12L\n\x18richmanActivityChestInfo\x12\x17.lq.ReqRichmanChestInfo\x1a\x17.lq.ResRichmanChestInfo\x12S\n\x15\x63reateGameObserveAuth\x12\x1c.lq.ReqCreateGameObserveAuth\x1a\x1c.lq.ResCreateGameObserveAuth\x12V\n\x16refreshGameObserveAuth\x12\x1d.lq.ReqRefreshGameObserveAuth\x1a\x1d.lq.ResRefreshGameObserveAuth\x12\x37\n\x11\x66\x65tchActivityBuff\x12\r.lq.ReqCommon\x1a\x13.lq.ResActivityBuff\x12\x46\n\x13upgradeActivityBuff\x12\x1a.lq.ReqUpgradeActivityBuff\x1a\x13.lq.ResActivityBuff\x12:\n\x10upgradeChallenge\x12\r.lq.ReqCommon\x1a\x17.lq.ResUpgradeChallenge\x12:\n\x10refreshChallenge\x12\r.lq.ReqCommon\x1a\x17.lq.ResRefreshChallenge\x12>\n\x12\x66\x65tchChallengeInfo\x12\r.lq.ReqCommon\x1a\x19.lq.ResFetchChallengeInfo\x12N\n\x1a\x66orceCompleteChallengeTask\x12!.lq.ReqForceCompleteChallengeTask\x1a\r.lq.ResCommon\x12\x41\n\x14\x66\x65tchChallengeSeason\x12\r.lq.ReqCommon\x1a\x1a.lq.ResChallengeSeasonInfo\x12\x62\n\x1areceiveChallengeRankReward\x12!.lq.ReqReceiveChallengeRankReward\x1a!.lq.ResReceiveChallengeRankReward\x12\x36\n\x10\x66\x65tchABMatchInfo\x12\r.lq.ReqCommon\x1a\x13.lq.ResFetchABMatch\x12\x32\n\x0c\x62uyInABMatch\x12\x13.lq.ReqBuyInABMatch\x1a\r.lq.ResCommon\x12\x34\n\x14receiveABMatchReward\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12+\n\x0bquitABMatch\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12<\n\x11startUnifiedMatch\x12\x18.lq.ReqStartUnifiedMatch\x1a\r.lq.ResCommon\x12>\n\x12\x63\x61ncelUnifiedMatch\x12\x19.lq.ReqCancelUnifiedMatch\x1a\r.lq.ResCommon\x12@\n\x12\x66\x65tchGamePointRank\x12\x14.lq.ReqGamePointRank\x1a\x14.lq.ResGamePointRank\x12M\n\x16\x66\x65tchSelfGamePointRank\x12\x14.lq.ReqGamePointRank\x1a\x1d.lq.ResFetchSelfGamePointRank2\xf5\x06\n\x08\x46\x61stTest\x12,\n\x08\x61uthGame\x12\x0f.lq.ReqAuthGame\x1a\x0f.lq.ResAuthGame\x12,\n\tenterGame\x12\r.lq.ReqCommon\x1a\x10.lq.ResEnterGame\x12,\n\x08syncGame\x12\x0f.lq.ReqSyncGame\x1a\x0f.lq.ResSyncGame\x12.\n\x0e\x66inishSyncGame\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12-\n\rterminateGame\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x35\n\x0einputOperation\x12\x14.lq.ReqSelfOperation\x1a\r.lq.ResCommon\x12\x35\n\x10inputChiPengGang\x12\x12.lq.ReqChiPengGang\x1a\r.lq.ResCommon\x12/\n\x0f\x63onfirmNewRound\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x38\n\x0f\x62roadcastInGame\x12\x16.lq.ReqBroadcastInGame\x1a\r.lq.ResCommon\x12=\n\x12inputGameGMCommand\x12\x18.lq.ReqGMCommandInGaming\x1a\r.lq.ResCommon\x12=\n\x14\x66\x65tchGamePlayerState\x12\r.lq.ReqCommon\x1a\x16.lq.ResGamePlayerState\x12\x31\n\x11\x63heckNetworkDelay\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12,\n\x0c\x63learLeaving\x12\r.lq.ReqCommon\x1a\r.lq.ResCommon\x12\x35\n\x0bvoteGameEnd\x12\x12.lq.ReqVoteGameEnd\x1a\x12.lq.ResGameEndVote\x12\x30\n\x0b\x61uthObserve\x12\x12.lq.ReqAuthObserve\x1a\r.lq.ResCommon\x12\x32\n\x0cstartObserve\x12\r.lq.ReqCommon\x1a\x13.lq.ResStartObserve\x12+\n\x0bstopObserve\x12\r.lq.ReqCommon\x1a\r.lq.ResCommonb\x06proto3')
 )
 
 _GAMEPLAYERSTATE = _descriptor.EnumDescriptor(
   name='GamePlayerState',
   full_name='lq.GamePlayerState',
   filename=None,
   file=DESCRIPTOR,
@@ -44,16 +44,16 @@
     _descriptor.EnumValueDescriptor(
       name='READY', index=3, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=62405,
-  serialized_end=62466,
+  serialized_start=63334,
+  serialized_end=63395,
 )
 _sym_db.RegisterEnumDescriptor(_GAMEPLAYERSTATE)
 
 GamePlayerState = enum_type_wrapper.EnumTypeWrapper(_GAMEPLAYERSTATE)
 NULL = 0
 AUTH = 1
 SYNCING = 2
@@ -4231,15 +4231,22 @@
       name='huansanzhang', full_name='lq.GameDetailRule.huansanzhang', index=48,
       number=49, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='disable_leijiyiman', full_name='lq.GameDetailRule.disable_leijiyiman', index=49,
+      name='chuanma', full_name='lq.GameDetailRule.chuanma', index=49,
+      number=50, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='disable_leijiyiman', full_name='lq.GameDetailRule.disable_leijiyiman', index=50,
       number=60, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -4250,15 +4257,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=8825,
-  serialized_end=10015,
+  serialized_end=10032,
 )
 
 
 _ROOM = _descriptor.Descriptor(
   name='Room',
   full_name='lq.Room',
   filename=None,
@@ -4350,16 +4357,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10018,
-  serialized_end=10268,
+  serialized_start=10035,
+  serialized_end=10285,
 )
 
 
 _GAMEENDRESULT_PLAYERITEM = _descriptor.Descriptor(
   name='PlayerItem',
   full_name='lq.GameEndResult.PlayerItem',
   filename=None,
@@ -4416,16 +4423,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10336,
-  serialized_end=10464,
+  serialized_start=10353,
+  serialized_end=10481,
 )
 
 _GAMEENDRESULT = _descriptor.Descriptor(
   name='GameEndResult',
   full_name='lq.GameEndResult',
   filename=None,
   file=DESCRIPTOR,
@@ -4446,16 +4453,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10271,
-  serialized_end=10464,
+  serialized_start=10288,
+  serialized_end=10481,
 )
 
 
 _GAMECONNECTINFO = _descriptor.Descriptor(
   name='GameConnectInfo',
   full_name='lq.GameConnectInfo',
   filename=None,
@@ -4491,16 +4498,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10466,
-  serialized_end=10543,
+  serialized_start=10483,
+  serialized_end=10560,
 )
 
 
 _ITEMGAINRECORD = _descriptor.Descriptor(
   name='ItemGainRecord',
   full_name='lq.ItemGainRecord',
   filename=None,
@@ -4529,16 +4536,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10545,
-  serialized_end=10593,
+  serialized_start=10562,
+  serialized_end=10610,
 )
 
 
 _ITEMGAINRECORDS = _descriptor.Descriptor(
   name='ItemGainRecords',
   full_name='lq.ItemGainRecords',
   filename=None,
@@ -4574,16 +4581,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10595,
-  serialized_end=10695,
+  serialized_start=10612,
+  serialized_end=10712,
 )
 
 
 _ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.Item',
   filename=None,
@@ -4612,16 +4619,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10697,
-  serialized_end=10735,
+  serialized_start=10714,
+  serialized_end=10752,
 )
 
 
 _BAG = _descriptor.Descriptor(
   name='Bag',
   full_name='lq.Bag',
   filename=None,
@@ -4650,16 +4657,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10737,
-  serialized_end=10815,
+  serialized_start=10754,
+  serialized_end=10832,
 )
 
 
 _BAGUPDATE = _descriptor.Descriptor(
   name='BagUpdate',
   full_name='lq.BagUpdate',
   filename=None,
@@ -4688,16 +4695,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10817,
-  serialized_end=10915,
+  serialized_start=10834,
+  serialized_end=10932,
 )
 
 
 _REWARDSLOT = _descriptor.Descriptor(
   name='RewardSlot',
   full_name='lq.RewardSlot',
   filename=None,
@@ -4726,16 +4733,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10917,
-  serialized_end=10956,
+  serialized_start=10934,
+  serialized_end=10973,
 )
 
 
 _OPENRESULT = _descriptor.Descriptor(
   name='OpenResult',
   full_name='lq.OpenResult',
   filename=None,
@@ -4764,16 +4771,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10958,
-  serialized_end=11035,
+  serialized_start=10975,
+  serialized_end=11052,
 )
 
 
 _REWARDPLUSRESULT_EXCHANGE = _descriptor.Descriptor(
   name='Exchange',
   full_name='lq.RewardPlusResult.Exchange',
   filename=None,
@@ -4809,16 +4816,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11134,
-  serialized_end=11189,
+  serialized_start=11151,
+  serialized_end=11206,
 )
 
 _REWARDPLUSRESULT = _descriptor.Descriptor(
   name='RewardPlusResult',
   full_name='lq.RewardPlusResult',
   filename=None,
   file=DESCRIPTOR,
@@ -4853,16 +4860,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11038,
-  serialized_end=11189,
+  serialized_start=11055,
+  serialized_end=11206,
 )
 
 
 _EXECUTEREWARD = _descriptor.Descriptor(
   name='ExecuteReward',
   full_name='lq.ExecuteReward',
   filename=None,
@@ -4898,16 +4905,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11191,
-  serialized_end=11294,
+  serialized_start=11208,
+  serialized_end=11311,
 )
 
 
 _MAIL_I18NCONTEXT = _descriptor.Descriptor(
   name='I18nContext',
   full_name='lq.Mail.I18nContext',
   filename=None,
@@ -4936,16 +4943,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11581,
-  serialized_end=11625,
+  serialized_start=11598,
+  serialized_end=11642,
 )
 
 _MAIL = _descriptor.Descriptor(
   name='Mail',
   full_name='lq.Mail',
   filename=None,
   file=DESCRIPTOR,
@@ -5036,16 +5043,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11297,
-  serialized_end=11625,
+  serialized_start=11314,
+  serialized_end=11642,
 )
 
 
 _ACHIEVEMENTPROGRESS = _descriptor.Descriptor(
   name='AchievementProgress',
   full_name='lq.AchievementProgress',
   filename=None,
@@ -5095,16 +5102,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11627,
-  serialized_end=11736,
+  serialized_start=11644,
+  serialized_end=11753,
 )
 
 
 _ACCOUNTSTATISTICBYGAMEMODE_ROUNDENDDATA = _descriptor.Descriptor(
   name='RoundEndData',
   full_name='lq.AccountStatisticByGameMode.RoundEndData',
   filename=None,
@@ -5133,16 +5140,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12172,
-  serialized_end=12213,
+  serialized_start=12189,
+  serialized_end=12230,
 )
 
 _ACCOUNTSTATISTICBYGAMEMODE_RANKSCORE = _descriptor.Descriptor(
   name='RankScore',
   full_name='lq.AccountStatisticByGameMode.RankScore',
   filename=None,
   file=DESCRIPTOR,
@@ -5177,16 +5184,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12215,
-  serialized_end=12274,
+  serialized_start=12232,
+  serialized_end=12291,
 )
 
 _ACCOUNTSTATISTICBYGAMEMODE = _descriptor.Descriptor(
   name='AccountStatisticByGameMode',
   full_name='lq.AccountStatisticByGameMode',
   filename=None,
   file=DESCRIPTOR,
@@ -5298,16 +5305,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11739,
-  serialized_end=12274,
+  serialized_start=11756,
+  serialized_end=12291,
 )
 
 
 _ACCOUNTSTATISTICBYFAN = _descriptor.Descriptor(
   name='AccountStatisticByFan',
   full_name='lq.AccountStatisticByFan',
   filename=None,
@@ -5336,16 +5343,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12276,
-  serialized_end=12328,
+  serialized_start=12293,
+  serialized_end=12345,
 )
 
 
 _ACCOUNTFANACHIEVED = _descriptor.Descriptor(
   name='AccountFanAchieved',
   full_name='lq.AccountFanAchieved',
   filename=None,
@@ -5381,16 +5388,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12330,
-  serialized_end=12438,
+  serialized_start=12347,
+  serialized_end=12455,
 )
 
 
 _ACCOUNTDETAILSTATISTIC = _descriptor.Descriptor(
   name='AccountDetailStatistic',
   full_name='lq.AccountDetailStatistic',
   filename=None,
@@ -5433,16 +5440,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12441,
-  serialized_end=12624,
+  serialized_start=12458,
+  serialized_end=12641,
 )
 
 
 _ACCOUNTDETAILSTATISTICBYCATEGORY = _descriptor.Descriptor(
   name='AccountDetailStatisticByCategory',
   full_name='lq.AccountDetailStatisticByCategory',
   filename=None,
@@ -5471,16 +5478,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12626,
-  serialized_end=12732,
+  serialized_start=12643,
+  serialized_end=12749,
 )
 
 
 _ACCOUNTDETAILSTATISTICV2_RANKSTATISTIC_RANKDATA_RANKLEVELDATA = _descriptor.Descriptor(
   name='RankLevelData',
   full_name='lq.AccountDetailStatisticV2.RankStatistic.RankData.RankLevelData',
   filename=None,
@@ -5509,16 +5516,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13612,
-  serialized_end=13694,
+  serialized_start=13629,
+  serialized_end=13711,
 )
 
 _ACCOUNTDETAILSTATISTICV2_RANKSTATISTIC_RANKDATA = _descriptor.Descriptor(
   name='RankData',
   full_name='lq.AccountDetailStatisticV2.RankStatistic.RankData',
   filename=None,
   file=DESCRIPTOR,
@@ -5546,16 +5553,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13451,
-  serialized_end=13694,
+  serialized_start=13468,
+  serialized_end=13711,
 )
 
 _ACCOUNTDETAILSTATISTICV2_RANKSTATISTIC = _descriptor.Descriptor(
   name='RankStatistic',
   full_name='lq.AccountDetailStatisticV2.RankStatistic',
   filename=None,
   file=DESCRIPTOR,
@@ -5590,16 +5597,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13249,
-  serialized_end=13694,
+  serialized_start=13266,
+  serialized_end=13711,
 )
 
 _ACCOUNTDETAILSTATISTICV2_CUSTOMIZEDCONTESTSTATISTIC = _descriptor.Descriptor(
   name='CustomizedContestStatistic',
   full_name='lq.AccountDetailStatisticV2.CustomizedContestStatistic',
   filename=None,
   file=DESCRIPTOR,
@@ -5634,16 +5641,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13697,
-  serialized_end=13859,
+  serialized_start=13714,
+  serialized_end=13876,
 )
 
 _ACCOUNTDETAILSTATISTICV2_CHALLENGESTATISTIC_SEASONDATA = _descriptor.Descriptor(
   name='SeasonData',
   full_name='lq.AccountDetailStatisticV2.ChallengeStatistic.SeasonData',
   filename=None,
   file=DESCRIPTOR,
@@ -5671,16 +5678,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14018,
-  serialized_end=14096,
+  serialized_start=14035,
+  serialized_end=14113,
 )
 
 _ACCOUNTDETAILSTATISTICV2_CHALLENGESTATISTIC = _descriptor.Descriptor(
   name='ChallengeStatistic',
   full_name='lq.AccountDetailStatisticV2.ChallengeStatistic',
   filename=None,
   file=DESCRIPTOR,
@@ -5708,16 +5715,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13862,
-  serialized_end=14096,
+  serialized_start=13879,
+  serialized_end=14113,
 )
 
 _ACCOUNTDETAILSTATISTICV2 = _descriptor.Descriptor(
   name='AccountDetailStatisticV2',
   full_name='lq.AccountDetailStatisticV2',
   filename=None,
   file=DESCRIPTOR,
@@ -5780,16 +5787,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12735,
-  serialized_end=14096,
+  serialized_start=12752,
+  serialized_end=14113,
 )
 
 
 _ACCOUNTSHILIAN = _descriptor.Descriptor(
   name='AccountShiLian',
   full_name='lq.AccountShiLian',
   filename=None,
@@ -5818,16 +5825,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14098,
-  serialized_end=14143,
+  serialized_start=14115,
+  serialized_end=14160,
 )
 
 
 _CLIENTDEVICEINFO = _descriptor.Descriptor(
   name='ClientDeviceInfo',
   full_name='lq.ClientDeviceInfo',
   filename=None,
@@ -5905,16 +5912,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14146,
-  serialized_end=14340,
+  serialized_start=14163,
+  serialized_end=14357,
 )
 
 
 _CLIENTVERSIONINFO = _descriptor.Descriptor(
   name='ClientVersionInfo',
   full_name='lq.ClientVersionInfo',
   filename=None,
@@ -5943,16 +5950,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14342,
-  serialized_end=14396,
+  serialized_start=14359,
+  serialized_end=14413,
 )
 
 
 _ANNOUNCEMENT = _descriptor.Descriptor(
   name='Announcement',
   full_name='lq.Announcement',
   filename=None,
@@ -5988,16 +5995,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14398,
-  serialized_end=14456,
+  serialized_start=14415,
+  serialized_end=14473,
 )
 
 
 _TASKPROGRESS = _descriptor.Descriptor(
   name='TaskProgress',
   full_name='lq.TaskProgress',
   filename=None,
@@ -6047,16 +6054,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14458,
-  serialized_end=14553,
+  serialized_start=14475,
+  serialized_end=14570,
 )
 
 
 _GAMECONFIG = _descriptor.Descriptor(
   name='GameConfig',
   full_name='lq.GameConfig',
   filename=None,
@@ -6092,16 +6099,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14555,
-  serialized_end=14645,
+  serialized_start=14572,
+  serialized_end=14662,
 )
 
 
 _ACCOUNTACTIVESTATE = _descriptor.Descriptor(
   name='AccountActiveState',
   full_name='lq.AccountActiveState',
   filename=None,
@@ -6151,16 +6158,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14648,
-  serialized_end=14789,
+  serialized_start=14665,
+  serialized_end=14806,
 )
 
 
 _FRIEND = _descriptor.Descriptor(
   name='Friend',
   full_name='lq.Friend',
   filename=None,
@@ -6189,16 +6196,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14791,
-  serialized_end=14872,
+  serialized_start=14808,
+  serialized_end=14889,
 )
 
 
 _GAMELIVEUNIT = _descriptor.Descriptor(
   name='GameLiveUnit',
   full_name='lq.GameLiveUnit',
   filename=None,
@@ -6234,16 +6241,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14874,
-  serialized_end=14953,
+  serialized_start=14891,
+  serialized_end=14970,
 )
 
 
 _GAMELIVESEGMENT = _descriptor.Descriptor(
   name='GameLiveSegment',
   full_name='lq.GameLiveSegment',
   filename=None,
@@ -6265,16 +6272,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14955,
-  serialized_end=15007,
+  serialized_start=14972,
+  serialized_end=15024,
 )
 
 
 _GAMELIVESEGMENTURI = _descriptor.Descriptor(
   name='GameLiveSegmentUri',
   full_name='lq.GameLiveSegmentUri',
   filename=None,
@@ -6303,16 +6310,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15009,
-  serialized_end=15070,
+  serialized_start=15026,
+  serialized_end=15087,
 )
 
 
 _GAMELIVEHEAD = _descriptor.Descriptor(
   name='GameLiveHead',
   full_name='lq.GameLiveHead',
   filename=None,
@@ -6362,16 +6369,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15073,
-  serialized_end=15214,
+  serialized_start=15090,
+  serialized_end=15231,
 )
 
 
 _GAMENEWROUNDSTATE = _descriptor.Descriptor(
   name='GameNewRoundState',
   full_name='lq.GameNewRoundState',
   filename=None,
@@ -6393,16 +6400,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15216,
-  serialized_end=15256,
+  serialized_start=15233,
+  serialized_end=15273,
 )
 
 
 _GAMEENDACTION = _descriptor.Descriptor(
   name='GameEndAction',
   full_name='lq.GameEndAction',
   filename=None,
@@ -6424,16 +6431,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15258,
-  serialized_end=15288,
+  serialized_start=15275,
+  serialized_end=15305,
 )
 
 
 _GAMENOOPACTION = _descriptor.Descriptor(
   name='GameNoopAction',
   full_name='lq.GameNoopAction',
   filename=None,
@@ -6448,16 +6455,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15290,
-  serialized_end=15306,
+  serialized_start=15307,
+  serialized_end=15323,
 )
 
 
 _COMMENTITEM = _descriptor.Descriptor(
   name='CommentItem',
   full_name='lq.CommentItem',
   filename=None,
@@ -6507,16 +6514,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15308,
-  serialized_end=15435,
+  serialized_start=15325,
+  serialized_end=15452,
 )
 
 
 _ROLLINGNOTICE = _descriptor.Descriptor(
   name='RollingNotice',
   full_name='lq.RollingNotice',
   filename=None,
@@ -6573,16 +6580,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15437,
-  serialized_end=15558,
+  serialized_start=15454,
+  serialized_end=15575,
 )
 
 
 _BILLINGGOODS = _descriptor.Descriptor(
   name='BillingGoods',
   full_name='lq.BillingGoods',
   filename=None,
@@ -6639,16 +6646,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15560,
-  serialized_end=15673,
+  serialized_start=15577,
+  serialized_end=15690,
 )
 
 
 _BILLSHORTCUT = _descriptor.Descriptor(
   name='BillShortcut',
   full_name='lq.BillShortcut',
   filename=None,
@@ -6684,16 +6691,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15675,
-  serialized_end=15735,
+  serialized_start=15692,
+  serialized_end=15752,
 )
 
 
 _BILLINGPRODUCT = _descriptor.Descriptor(
   name='BillingProduct',
   full_name='lq.BillingProduct',
   filename=None,
@@ -6736,16 +6743,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15737,
-  serialized_end=15854,
+  serialized_start=15754,
+  serialized_end=15871,
 )
 
 
 _CHARACTER = _descriptor.Descriptor(
   name='Character',
   full_name='lq.Character',
   filename=None,
@@ -6809,16 +6816,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15857,
-  serialized_end=15997,
+  serialized_start=15874,
+  serialized_end=16014,
 )
 
 
 _BUYRECORD = _descriptor.Descriptor(
   name='BuyRecord',
   full_name='lq.BuyRecord',
   filename=None,
@@ -6847,16 +6854,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15999,
-  serialized_end=16037,
+  serialized_start=16016,
+  serialized_end=16054,
 )
 
 
 _ZHPSHOP_REFRESHCOUNT = _descriptor.Descriptor(
   name='RefreshCount',
   full_name='lq.ZHPShop.RefreshCount',
   filename=None,
@@ -6885,16 +6892,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16198,
-  serialized_end=16242,
+  serialized_start=16215,
+  serialized_end=16259,
 )
 
 _ZHPSHOP = _descriptor.Descriptor(
   name='ZHPShop',
   full_name='lq.ZHPShop',
   filename=None,
   file=DESCRIPTOR,
@@ -6936,16 +6943,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16040,
-  serialized_end=16242,
+  serialized_start=16057,
+  serialized_end=16259,
 )
 
 
 _MONTHTICKETINFO = _descriptor.Descriptor(
   name='MonthTicketInfo',
   full_name='lq.MonthTicketInfo',
   filename=None,
@@ -6981,16 +6988,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16244,
-  serialized_end=16314,
+  serialized_start=16261,
+  serialized_end=16331,
 )
 
 
 _SHOPINFO = _descriptor.Descriptor(
   name='ShopInfo',
   full_name='lq.ShopInfo',
   filename=None,
@@ -7026,16 +7033,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16316,
-  serialized_end=16415,
+  serialized_start=16333,
+  serialized_end=16432,
 )
 
 
 _CHANGENICKNAMERECORD = _descriptor.Descriptor(
   name='ChangeNicknameRecord',
   full_name='lq.ChangeNicknameRecord',
   filename=None,
@@ -7071,16 +7078,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16417,
-  serialized_end=16479,
+  serialized_start=16434,
+  serialized_end=16496,
 )
 
 
 _SERVERSETTINGS = _descriptor.Descriptor(
   name='ServerSettings',
   full_name='lq.ServerSettings',
   filename=None,
@@ -7109,16 +7116,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16481,
-  serialized_end=16592,
+  serialized_start=16498,
+  serialized_end=16609,
 )
 
 
 _PAYMENTSETTINGV2_PAYMENTMAINTAIN = _descriptor.Descriptor(
   name='PaymentMaintain',
   full_name='lq.PaymentSettingV2.PaymentMaintain',
   filename=None,
@@ -7161,16 +7168,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16705,
-  serialized_end=16814,
+  serialized_start=16722,
+  serialized_end=16831,
 )
 
 _PAYMENTSETTINGV2_PAYMENTSETTINGUNIT = _descriptor.Descriptor(
   name='PaymentSettingUnit',
   full_name='lq.PaymentSettingV2.PaymentSettingUnit',
   filename=None,
   file=DESCRIPTOR,
@@ -7219,16 +7226,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16817,
-  serialized_end=16982,
+  serialized_start=16834,
+  serialized_end=16999,
 )
 
 _PAYMENTSETTINGV2 = _descriptor.Descriptor(
   name='PaymentSettingV2',
   full_name='lq.PaymentSettingV2',
   filename=None,
   file=DESCRIPTOR,
@@ -7256,16 +7263,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16595,
-  serialized_end=16982,
+  serialized_start=16612,
+  serialized_end=16999,
 )
 
 
 _PAYMENTSETTING_WECHATDATA = _descriptor.Descriptor(
   name='WechatData',
   full_name='lq.PaymentSetting.WechatData',
   filename=None,
@@ -7301,16 +7308,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17173,
-  serialized_end=17265,
+  serialized_start=17190,
+  serialized_end=17282,
 )
 
 _PAYMENTSETTING_ALIPAYDATA = _descriptor.Descriptor(
   name='AlipayData',
   full_name='lq.PaymentSetting.AlipayData',
   filename=None,
   file=DESCRIPTOR,
@@ -7338,16 +7345,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17267,
-  serialized_end=17336,
+  serialized_start=17284,
+  serialized_end=17353,
 )
 
 _PAYMENTSETTING = _descriptor.Descriptor(
   name='PaymentSetting',
   full_name='lq.PaymentSetting',
   filename=None,
   file=DESCRIPTOR,
@@ -7396,16 +7403,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=16985,
-  serialized_end=17336,
+  serialized_start=17002,
+  serialized_end=17353,
 )
 
 
 _ACCOUNTSETTING = _descriptor.Descriptor(
   name='AccountSetting',
   full_name='lq.AccountSetting',
   filename=None,
@@ -7434,16 +7441,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17338,
-  serialized_end=17382,
+  serialized_start=17355,
+  serialized_end=17399,
 )
 
 
 _CHESTDATA = _descriptor.Descriptor(
   name='ChestData',
   full_name='lq.ChestData',
   filename=None,
@@ -7486,16 +7493,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17384,
-  serialized_end=17488,
+  serialized_start=17401,
+  serialized_end=17505,
 )
 
 
 _CHESTDATAV2 = _descriptor.Descriptor(
   name='ChestDataV2',
   full_name='lq.ChestDataV2',
   filename=None,
@@ -7531,16 +7538,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17490,
-  serialized_end=17573,
+  serialized_start=17507,
+  serialized_end=17590,
 )
 
 
 _FAITHDATA = _descriptor.Descriptor(
   name='FaithData',
   full_name='lq.FaithData',
   filename=None,
@@ -7583,16 +7590,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17575,
-  serialized_end=17675,
+  serialized_start=17592,
+  serialized_end=17692,
 )
 
 
 _CUSTOMIZEDCONTESTBASE = _descriptor.Descriptor(
   name='CustomizedContestBase',
   full_name='lq.CustomizedContestBase',
   filename=None,
@@ -7677,16 +7684,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17678,
-  serialized_end=17895,
+  serialized_start=17695,
+  serialized_end=17912,
 )
 
 
 _CUSTOMIZEDCONTESTEXTEND = _descriptor.Descriptor(
   name='CustomizedContestExtend',
   full_name='lq.CustomizedContestExtend',
   filename=None,
@@ -7715,16 +7722,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17897,
-  serialized_end=17964,
+  serialized_start=17914,
+  serialized_end=17981,
 )
 
 
 _CUSTOMIZEDCONTESTABSTRACT = _descriptor.Descriptor(
   name='CustomizedContestAbstract',
   full_name='lq.CustomizedContestAbstract',
   filename=None,
@@ -7809,16 +7816,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=17967,
-  serialized_end=18189,
+  serialized_start=17984,
+  serialized_end=18206,
 )
 
 
 _CUSTOMIZEDCONTESTDETAIL = _descriptor.Descriptor(
   name='CustomizedContestDetail',
   full_name='lq.CustomizedContestDetail',
   filename=None,
@@ -7931,16 +7938,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=18192,
-  serialized_end=18512,
+  serialized_start=18209,
+  serialized_end=18529,
 )
 
 
 _CUSTOMIZEDCONTESTPLAYERREPORT = _descriptor.Descriptor(
   name='CustomizedContestPlayerReport',
   full_name='lq.CustomizedContestPlayerReport',
   filename=None,
@@ -7990,16 +7997,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=18514,
-  serialized_end=18639,
+  serialized_start=18531,
+  serialized_end=18656,
 )
 
 
 _RECORDGAME_ACCOUNTINFO = _descriptor.Descriptor(
   name='AccountInfo',
   full_name='lq.RecordGame.AccountInfo',
   filename=None,
@@ -8091,16 +8098,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=18822,
-  serialized_end=19091,
+  serialized_start=18839,
+  serialized_end=19108,
 )
 
 _RECORDGAME = _descriptor.Descriptor(
   name='RecordGame',
   full_name='lq.RecordGame',
   filename=None,
   file=DESCRIPTOR,
@@ -8156,16 +8163,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=18642,
-  serialized_end=19091,
+  serialized_start=18659,
+  serialized_end=19108,
 )
 
 
 _CUSTOMIZEDCONTESTGAMESTART_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.CustomizedContestGameStart.Item',
   filename=None,
@@ -8194,16 +8201,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19178,
-  serialized_end=19222,
+  serialized_start=19195,
+  serialized_end=19239,
 )
 
 _CUSTOMIZEDCONTESTGAMESTART = _descriptor.Descriptor(
   name='CustomizedContestGameStart',
   full_name='lq.CustomizedContestGameStart',
   filename=None,
   file=DESCRIPTOR,
@@ -8224,16 +8231,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19094,
-  serialized_end=19222,
+  serialized_start=19111,
+  serialized_end=19239,
 )
 
 
 _CUSTOMIZEDCONTESTGAMEEND_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.CustomizedContestGameEnd.Item',
   filename=None,
@@ -8269,16 +8276,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19305,
-  serialized_end=19370,
+  serialized_start=19322,
+  serialized_end=19387,
 )
 
 _CUSTOMIZEDCONTESTGAMEEND = _descriptor.Descriptor(
   name='CustomizedContestGameEnd',
   full_name='lq.CustomizedContestGameEnd',
   filename=None,
   file=DESCRIPTOR,
@@ -8299,16 +8306,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19225,
-  serialized_end=19370,
+  serialized_start=19242,
+  serialized_end=19387,
 )
 
 
 _ACTIVITY = _descriptor.Descriptor(
   name='Activity',
   full_name='lq.Activity',
   filename=None,
@@ -8351,16 +8358,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19372,
-  serialized_end=19455,
+  serialized_start=19389,
+  serialized_end=19472,
 )
 
 
 _EXCHANGERECORD = _descriptor.Descriptor(
   name='ExchangeRecord',
   full_name='lq.ExchangeRecord',
   filename=None,
@@ -8389,16 +8396,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19457,
-  serialized_end=19509,
+  serialized_start=19474,
+  serialized_end=19526,
 )
 
 
 _ACTIVITYACCUMULATEDPOINTDATA = _descriptor.Descriptor(
   name='ActivityAccumulatedPointData',
   full_name='lq.ActivityAccumulatedPointData',
   filename=None,
@@ -8434,16 +8441,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19511,
-  serialized_end=19605,
+  serialized_start=19528,
+  serialized_end=19622,
 )
 
 
 _ACTIVITYRANKPOINTDATA = _descriptor.Descriptor(
   name='ActivityRankPointData',
   full_name='lq.ActivityRankPointData',
   filename=None,
@@ -8486,16 +8493,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19607,
-  serialized_end=19715,
+  serialized_start=19624,
+  serialized_end=19732,
 )
 
 
 _GAMEROUNDHUDATA_HUPAI = _descriptor.Descriptor(
   name='HuPai',
   full_name='lq.GameRoundHuData.HuPai',
   filename=None,
@@ -8531,16 +8538,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20039,
-  serialized_end=20088,
+  serialized_start=20056,
+  serialized_end=20105,
 )
 
 _GAMEROUNDHUDATA_FAN = _descriptor.Descriptor(
   name='Fan',
   full_name='lq.GameRoundHuData.Fan',
   filename=None,
   file=DESCRIPTOR,
@@ -8575,16 +8582,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20090,
-  serialized_end=20135,
+  serialized_start=20107,
+  serialized_end=20152,
 )
 
 _GAMEROUNDHUDATA = _descriptor.Descriptor(
   name='GameRoundHuData',
   full_name='lq.GameRoundHuData',
   filename=None,
   file=DESCRIPTOR,
@@ -8689,16 +8696,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=19718,
-  serialized_end=20135,
+  serialized_start=19735,
+  serialized_end=20152,
 )
 
 
 _GAMEROUNDPLAYERRESULT = _descriptor.Descriptor(
   name='GameRoundPlayerResult',
   full_name='lq.GameRoundPlayerResult',
   filename=None,
@@ -8769,16 +8776,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20138,
-  serialized_end=20319,
+  serialized_start=20155,
+  serialized_end=20336,
 )
 
 
 _GAMEROUNDPLAYER = _descriptor.Descriptor(
   name='GameRoundPlayer',
   full_name='lq.GameRoundPlayer',
   filename=None,
@@ -8814,16 +8821,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20321,
-  serialized_end=20410,
+  serialized_start=20338,
+  serialized_end=20427,
 )
 
 
 _GAMEROUNDSNAPSHOT = _descriptor.Descriptor(
   name='GameRoundSnapshot',
   full_name='lq.GameRoundSnapshot',
   filename=None,
@@ -8859,16 +8866,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20412,
-  serialized_end=20494,
+  serialized_start=20429,
+  serialized_end=20511,
 )
 
 
 _GAMEFINALSNAPSHOT_CALCULATEPARAM = _descriptor.Descriptor(
   name='CalculateParam',
   full_name='lq.GameFinalSnapshot.CalculateParam',
   filename=None,
@@ -8904,16 +8911,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20986,
-  serialized_end=21069,
+  serialized_start=21003,
+  serialized_end=21086,
 )
 
 _GAMEFINALSNAPSHOT_GAMESEAT = _descriptor.Descriptor(
   name='GameSeat',
   full_name='lq.GameFinalSnapshot.GameSeat',
   filename=None,
   file=DESCRIPTOR,
@@ -8962,16 +8969,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=21072,
-  serialized_end=21208,
+  serialized_start=21089,
+  serialized_end=21225,
 )
 
 _GAMEFINALSNAPSHOT_FINALPLAYER = _descriptor.Descriptor(
   name='FinalPlayer',
   full_name='lq.GameFinalSnapshot.FinalPlayer',
   filename=None,
   file=DESCRIPTOR,
@@ -9027,16 +9034,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=21211,
-  serialized_end=21340,
+  serialized_start=21228,
+  serialized_end=21357,
 )
 
 _GAMEFINALSNAPSHOT_AFKINFO = _descriptor.Descriptor(
   name='AFKInfo',
   full_name='lq.GameFinalSnapshot.AFKInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -9071,16 +9078,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=21342,
-  serialized_end=21411,
+  serialized_start=21359,
+  serialized_end=21428,
 )
 
 _GAMEFINALSNAPSHOT = _descriptor.Descriptor(
   name='GameFinalSnapshot',
   full_name='lq.GameFinalSnapshot',
   filename=None,
   file=DESCRIPTOR,
@@ -9192,16 +9199,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=20497,
-  serialized_end=21411,
+  serialized_start=20514,
+  serialized_end=21428,
 )
 
 
 _RECORDCOLLECTEDDATA = _descriptor.Descriptor(
   name='RecordCollectedData',
   full_name='lq.RecordCollectedData',
   filename=None,
@@ -9244,16 +9251,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=21413,
-  serialized_end=21503,
+  serialized_start=21430,
+  serialized_end=21520,
 )
 
 
 _CONTESTDETAILRULE = _descriptor.Descriptor(
   name='ContestDetailRule',
   full_name='lq.ContestDetailRule',
   filename=None,
@@ -9534,16 +9541,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=21506,
-  serialized_end=22460,
+  serialized_start=21523,
+  serialized_end=22477,
 )
 
 
 _CONTESTDETAILRULEV2_EXTRARULE = _descriptor.Descriptor(
   name='ExtraRule',
   full_name='lq.ContestDetailRuleV2.ExtraRule',
   filename=None,
@@ -9572,16 +9579,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=22583,
-  serialized_end=22642,
+  serialized_start=22600,
+  serialized_end=22659,
 )
 
 _CONTESTDETAILRULEV2 = _descriptor.Descriptor(
   name='ContestDetailRuleV2',
   full_name='lq.ContestDetailRuleV2',
   filename=None,
   file=DESCRIPTOR,
@@ -9609,16 +9616,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=22463,
-  serialized_end=22642,
+  serialized_start=22480,
+  serialized_end=22659,
 )
 
 
 _GAMERULESETTING = _descriptor.Descriptor(
   name='GameRuleSetting',
   full_name='lq.GameRuleSetting',
   filename=None,
@@ -9675,16 +9682,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=22645,
-  serialized_end=22816,
+  serialized_start=22662,
+  serialized_end=22833,
 )
 
 
 _RECORDTINGPAIINFO = _descriptor.Descriptor(
   name='RecordTingPaiInfo',
   full_name='lq.RecordTingPaiInfo',
   filename=None,
@@ -9762,16 +9769,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=22819,
-  serialized_end=22992,
+  serialized_start=22836,
+  serialized_end=23009,
 )
 
 
 _RECORDNOTILEPLAYERINFO = _descriptor.Descriptor(
   name='RecordNoTilePlayerInfo',
   full_name='lq.RecordNoTilePlayerInfo',
   filename=None,
@@ -9814,16 +9821,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=22994,
-  serialized_end=23103,
+  serialized_start=23011,
+  serialized_end=23120,
 )
 
 
 _RECORDHULEINFO_RECORDFANINFO = _descriptor.Descriptor(
   name='RecordFanInfo',
   full_name='lq.RecordHuleInfo.RecordFanInfo',
   filename=None,
@@ -9852,16 +9859,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23506,
-  serialized_end=23546,
+  serialized_start=23523,
+  serialized_end=23563,
 )
 
 _RECORDHULEINFO = _descriptor.Descriptor(
   name='RecordHuleInfo',
   full_name='lq.RecordHuleInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -10022,16 +10029,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23106,
-  serialized_end=23546,
+  serialized_start=23123,
+  serialized_end=23563,
 )
 
 
 _RECORDHULESINFO = _descriptor.Descriptor(
   name='RecordHulesInfo',
   full_name='lq.RecordHulesInfo',
   filename=None,
@@ -10060,16 +10067,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23548,
-  serialized_end=23614,
+  serialized_start=23565,
+  serialized_end=23631,
 )
 
 
 _RECORDLIUJUINFO = _descriptor.Descriptor(
   name='RecordLiujuInfo',
   full_name='lq.RecordLiujuInfo',
   filename=None,
@@ -10098,16 +10105,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23616,
-  serialized_end=23661,
+  serialized_start=23633,
+  serialized_end=23678,
 )
 
 
 _RECORDNOTILEINFO = _descriptor.Descriptor(
   name='RecordNoTileInfo',
   full_name='lq.RecordNoTileInfo',
   filename=None,
@@ -10136,16 +10143,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23663,
-  serialized_end=23748,
+  serialized_start=23680,
+  serialized_end=23765,
 )
 
 
 _RECORDLIQIINFO = _descriptor.Descriptor(
   name='RecordLiqiInfo',
   full_name='lq.RecordLiqiInfo',
   filename=None,
@@ -10202,16 +10209,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23750,
-  serialized_end=23864,
+  serialized_start=23767,
+  serialized_end=23881,
 )
 
 
 _RECORDGANGINFO = _descriptor.Descriptor(
   name='RecordGangInfo',
   full_name='lq.RecordGangInfo',
   filename=None,
@@ -10261,16 +10268,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23866,
-  serialized_end=23953,
+  serialized_start=23883,
+  serialized_end=23970,
 )
 
 
 _RECORDBABEIINFO = _descriptor.Descriptor(
   name='RecordBaBeiInfo',
   full_name='lq.RecordBaBeiInfo',
   filename=None,
@@ -10313,16 +10320,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=23955,
-  serialized_end=24038,
+  serialized_start=23972,
+  serialized_end=24055,
 )
 
 
 _RECORDPEIPAIINFO = _descriptor.Descriptor(
   name='RecordPeiPaiInfo',
   full_name='lq.RecordPeiPaiInfo',
   filename=None,
@@ -10358,16 +10365,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24040,
-  serialized_end=24119,
+  serialized_start=24057,
+  serialized_end=24136,
 )
 
 
 _RECORDROUNDINFO = _descriptor.Descriptor(
   name='RecordRoundInfo',
   full_name='lq.RecordRoundInfo',
   filename=None,
@@ -10466,16 +10473,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24122,
-  serialized_end=24501,
+  serialized_start=24139,
+  serialized_end=24518,
 )
 
 
 _RECORDANALYSISEDDATA = _descriptor.Descriptor(
   name='RecordAnalysisedData',
   full_name='lq.RecordAnalysisedData',
   filename=None,
@@ -10497,16 +10504,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24503,
-  serialized_end=24567,
+  serialized_start=24520,
+  serialized_end=24584,
 )
 
 
 _RESCONNECTIONINFO = _descriptor.Descriptor(
   name='ResConnectionInfo',
   full_name='lq.ResConnectionInfo',
   filename=None,
@@ -10535,16 +10542,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24569,
-  serialized_end=24660,
+  serialized_start=24586,
+  serialized_end=24677,
 )
 
 
 _REQSIGNUPACCOUNT = _descriptor.Descriptor(
   name='ReqSignupAccount',
   full_name='lq.ReqSignupAccount',
   filename=None,
@@ -10594,16 +10601,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24662,
-  serialized_end=24781,
+  serialized_start=24679,
+  serialized_end=24798,
 )
 
 
 _RESSIGNUPACCOUNT = _descriptor.Descriptor(
   name='ResSignupAccount',
   full_name='lq.ResSignupAccount',
   filename=None,
@@ -10625,16 +10632,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24783,
-  serialized_end=24827,
+  serialized_start=24800,
+  serialized_end=24844,
 )
 
 
 _REQLOGIN = _descriptor.Descriptor(
   name='ReqLogin',
   full_name='lq.ReqLogin',
   filename=None,
@@ -10719,16 +10726,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=24830,
-  serialized_end=25084,
+  serialized_start=24847,
+  serialized_end=25101,
 )
 
 
 _RESLOGIN = _descriptor.Descriptor(
   name='ResLogin',
   full_name='lq.ResLogin',
   filename=None,
@@ -10820,16 +10827,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25087,
-  serialized_end=25384,
+  serialized_start=25104,
+  serialized_end=25401,
 )
 
 
 _REQEMAILLOGIN = _descriptor.Descriptor(
   name='ReqEmailLogin',
   full_name='lq.ReqEmailLogin',
   filename=None,
@@ -10900,16 +10907,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25387,
-  serialized_end=25590,
+  serialized_start=25404,
+  serialized_end=25607,
 )
 
 
 _REQBINDACCOUNT = _descriptor.Descriptor(
   name='ReqBindAccount',
   full_name='lq.ReqBindAccount',
   filename=None,
@@ -10938,16 +10945,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25592,
-  serialized_end=25643,
+  serialized_start=25609,
+  serialized_end=25660,
 )
 
 
 _REQCREATEPHONEVERIFYCODE = _descriptor.Descriptor(
   name='ReqCreatePhoneVerifyCode',
   full_name='lq.ReqCreatePhoneVerifyCode',
   filename=None,
@@ -10976,16 +10983,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25645,
-  serialized_end=25701,
+  serialized_start=25662,
+  serialized_end=25718,
 )
 
 
 _REQCREATEEMAILVERIFYCODE = _descriptor.Descriptor(
   name='ReqCreateEmailVerifyCode',
   full_name='lq.ReqCreateEmailVerifyCode',
   filename=None,
@@ -11014,16 +11021,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25703,
-  serialized_end=25759,
+  serialized_start=25720,
+  serialized_end=25776,
 )
 
 
 _REQVERIFYCODEFORSECURE = _descriptor.Descriptor(
   name='ReqVerifyCodeForSecure',
   full_name='lq.ReqVerifyCodeForSecure',
   filename=None,
@@ -11052,16 +11059,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25761,
-  serialized_end=25818,
+  serialized_start=25778,
+  serialized_end=25835,
 )
 
 
 _RESVERFIYCODEFORSECURE = _descriptor.Descriptor(
   name='ResVerfiyCodeForSecure',
   full_name='lq.ResVerfiyCodeForSecure',
   filename=None,
@@ -11090,16 +11097,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25820,
-  serialized_end=25892,
+  serialized_start=25837,
+  serialized_end=25909,
 )
 
 
 _REQBINDPHONENUMBER = _descriptor.Descriptor(
   name='ReqBindPhoneNumber',
   full_name='lq.ReqBindPhoneNumber',
   filename=None,
@@ -11142,16 +11149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25894,
-  serialized_end=25989,
+  serialized_start=25911,
+  serialized_end=26006,
 )
 
 
 _REQUNBINDPHONENUMBER = _descriptor.Descriptor(
   name='ReqUnbindPhoneNumber',
   full_name='lq.ReqUnbindPhoneNumber',
   filename=None,
@@ -11187,16 +11194,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=25991,
-  serialized_end=26060,
+  serialized_start=26008,
+  serialized_end=26077,
 )
 
 
 _RESFETCHPHONELOGINBIND = _descriptor.Descriptor(
   name='ResFetchPhoneLoginBind',
   full_name='lq.ResFetchPhoneLoginBind',
   filename=None,
@@ -11225,16 +11232,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26062,
-  serialized_end=26133,
+  serialized_start=26079,
+  serialized_end=26150,
 )
 
 
 _REQCREATEPHONELOGINBIND = _descriptor.Descriptor(
   name='ReqCreatePhoneLoginBind',
   full_name='lq.ReqCreatePhoneLoginBind',
   filename=None,
@@ -11256,16 +11263,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26135,
-  serialized_end=26178,
+  serialized_start=26152,
+  serialized_end=26195,
 )
 
 
 _REQBINDEMAIL = _descriptor.Descriptor(
   name='ReqBindEmail',
   full_name='lq.ReqBindEmail',
   filename=None,
@@ -11301,16 +11308,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26180,
-  serialized_end=26241,
+  serialized_start=26197,
+  serialized_end=26258,
 )
 
 
 _REQMODIFYPASSWORD = _descriptor.Descriptor(
   name='ReqModifyPassword',
   full_name='lq.ReqModifyPassword',
   filename=None,
@@ -11346,16 +11353,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26243,
-  serialized_end=26328,
+  serialized_start=26260,
+  serialized_end=26345,
 )
 
 
 _REQOAUTH2AUTH = _descriptor.Descriptor(
   name='ReqOauth2Auth',
   full_name='lq.ReqOauth2Auth',
   filename=None,
@@ -11391,16 +11398,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26330,
-  serialized_end=26386,
+  serialized_start=26347,
+  serialized_end=26403,
 )
 
 
 _RESOAUTH2AUTH = _descriptor.Descriptor(
   name='ResOauth2Auth',
   full_name='lq.ResOauth2Auth',
   filename=None,
@@ -11429,16 +11436,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26388,
-  serialized_end=26451,
+  serialized_start=26405,
+  serialized_end=26468,
 )
 
 
 _REQOAUTH2CHECK = _descriptor.Descriptor(
   name='ReqOauth2Check',
   full_name='lq.ReqOauth2Check',
   filename=None,
@@ -11467,16 +11474,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26453,
-  serialized_end=26505,
+  serialized_start=26470,
+  serialized_end=26522,
 )
 
 
 _RESOAUTH2CHECK = _descriptor.Descriptor(
   name='ResOauth2Check',
   full_name='lq.ResOauth2Check',
   filename=None,
@@ -11505,16 +11512,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26507,
-  serialized_end=26570,
+  serialized_start=26524,
+  serialized_end=26587,
 )
 
 
 _REQOAUTH2SIGNUP = _descriptor.Descriptor(
   name='ReqOauth2Signup',
   full_name='lq.ReqOauth2Signup',
   filename=None,
@@ -11571,16 +11578,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26573,
-  serialized_end=26749,
+  serialized_start=26590,
+  serialized_end=26766,
 )
 
 
 _RESOAUTH2SIGNUP = _descriptor.Descriptor(
   name='ResOauth2Signup',
   full_name='lq.ResOauth2Signup',
   filename=None,
@@ -11602,16 +11609,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26751,
-  serialized_end=26794,
+  serialized_start=26768,
+  serialized_end=26811,
 )
 
 
 _REQOAUTH2LOGIN = _descriptor.Descriptor(
   name='ReqOauth2Login',
   full_name='lq.ReqOauth2Login',
   filename=None,
@@ -11689,16 +11696,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=26797,
-  serialized_end=27044,
+  serialized_start=26814,
+  serialized_end=27061,
 )
 
 
 _REQDMMPRELOGIN = _descriptor.Descriptor(
   name='ReqDMMPreLogin',
   full_name='lq.ReqDMMPreLogin',
   filename=None,
@@ -11720,16 +11727,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27046,
-  serialized_end=27082,
+  serialized_start=27063,
+  serialized_end=27099,
 )
 
 
 _RESDMMPRELOGIN = _descriptor.Descriptor(
   name='ResDMMPreLogin',
   full_name='lq.ResDMMPreLogin',
   filename=None,
@@ -11751,16 +11758,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27084,
-  serialized_end=27119,
+  serialized_start=27101,
+  serialized_end=27136,
 )
 
 
 _REQLOGOUT = _descriptor.Descriptor(
   name='ReqLogout',
   full_name='lq.ReqLogout',
   filename=None,
@@ -11775,16 +11782,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27121,
-  serialized_end=27132,
+  serialized_start=27138,
+  serialized_end=27149,
 )
 
 
 _RESLOGOUT = _descriptor.Descriptor(
   name='ResLogout',
   full_name='lq.ResLogout',
   filename=None,
@@ -11806,16 +11813,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27134,
-  serialized_end=27171,
+  serialized_start=27151,
+  serialized_end=27188,
 )
 
 
 _REQHEATBEAT = _descriptor.Descriptor(
   name='ReqHeatBeat',
   full_name='lq.ReqHeatBeat',
   filename=None,
@@ -11837,16 +11844,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27173,
-  serialized_end=27216,
+  serialized_start=27190,
+  serialized_end=27233,
 )
 
 
 _REQLOGINBEAT = _descriptor.Descriptor(
   name='ReqLoginBeat',
   full_name='lq.ReqLoginBeat',
   filename=None,
@@ -11868,16 +11875,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27218,
-  serialized_end=27250,
+  serialized_start=27235,
+  serialized_end=27267,
 )
 
 
 _REQJOINMATCHQUEUE = _descriptor.Descriptor(
   name='ReqJoinMatchQueue',
   full_name='lq.ReqJoinMatchQueue',
   filename=None,
@@ -11899,16 +11906,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27252,
-  serialized_end=27291,
+  serialized_start=27269,
+  serialized_end=27308,
 )
 
 
 _REQCANCELMATCHQUEUE = _descriptor.Descriptor(
   name='ReqCancelMatchQueue',
   full_name='lq.ReqCancelMatchQueue',
   filename=None,
@@ -11930,16 +11937,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27293,
-  serialized_end=27334,
+  serialized_start=27310,
+  serialized_end=27351,
 )
 
 
 _REQACCOUNTINFO = _descriptor.Descriptor(
   name='ReqAccountInfo',
   full_name='lq.ReqAccountInfo',
   filename=None,
@@ -11961,16 +11968,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27336,
-  serialized_end=27372,
+  serialized_start=27353,
+  serialized_end=27389,
 )
 
 
 _RESACCOUNTINFO = _descriptor.Descriptor(
   name='ResAccountInfo',
   full_name='lq.ResAccountInfo',
   filename=None,
@@ -12006,16 +12013,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27374,
-  serialized_end=27470,
+  serialized_start=27391,
+  serialized_end=27487,
 )
 
 
 _REQCREATENICKNAME = _descriptor.Descriptor(
   name='ReqCreateNickname',
   full_name='lq.ReqCreateNickname',
   filename=None,
@@ -12044,16 +12051,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27472,
-  serialized_end=27532,
+  serialized_start=27489,
+  serialized_end=27549,
 )
 
 
 _REQMODIFYNICKNAME = _descriptor.Descriptor(
   name='ReqModifyNickname',
   full_name='lq.ReqModifyNickname',
   filename=None,
@@ -12082,16 +12089,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27534,
-  serialized_end=27592,
+  serialized_start=27551,
+  serialized_end=27609,
 )
 
 
 _REQMODIFYBIRTHDAY = _descriptor.Descriptor(
   name='ReqModifyBirthday',
   full_name='lq.ReqModifyBirthday',
   filename=None,
@@ -12113,16 +12120,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27594,
-  serialized_end=27631,
+  serialized_start=27611,
+  serialized_end=27648,
 )
 
 
 _RESSELFROOM = _descriptor.Descriptor(
   name='ResSelfRoom',
   full_name='lq.ResSelfRoom',
   filename=None,
@@ -12151,16 +12158,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27633,
-  serialized_end=27696,
+  serialized_start=27650,
+  serialized_end=27713,
 )
 
 
 _REQCREATEROOM = _descriptor.Descriptor(
   name='ReqCreateRoom',
   full_name='lq.ReqCreateRoom',
   filename=None,
@@ -12196,16 +12203,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27698,
-  serialized_end=27784,
+  serialized_start=27715,
+  serialized_end=27801,
 )
 
 
 _RESCREATEROOM = _descriptor.Descriptor(
   name='ResCreateRoom',
   full_name='lq.ResCreateRoom',
   filename=None,
@@ -12234,16 +12241,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27786,
-  serialized_end=27851,
+  serialized_start=27803,
+  serialized_end=27868,
 )
 
 
 _REQJOINROOM = _descriptor.Descriptor(
   name='ReqJoinRoom',
   full_name='lq.ReqJoinRoom',
   filename=None,
@@ -12265,16 +12272,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27853,
-  serialized_end=27883,
+  serialized_start=27870,
+  serialized_end=27900,
 )
 
 
 _RESJOINROOM = _descriptor.Descriptor(
   name='ResJoinRoom',
   full_name='lq.ResJoinRoom',
   filename=None,
@@ -12303,16 +12310,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27885,
-  serialized_end=27948,
+  serialized_start=27902,
+  serialized_end=27965,
 )
 
 
 _REQROOMREADY = _descriptor.Descriptor(
   name='ReqRoomReady',
   full_name='lq.ReqRoomReady',
   filename=None,
@@ -12334,16 +12341,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27950,
-  serialized_end=27979,
+  serialized_start=27967,
+  serialized_end=27996,
 )
 
 
 _REQROOMDRESSING = _descriptor.Descriptor(
   name='ReqRoomDressing',
   full_name='lq.ReqRoomDressing',
   filename=None,
@@ -12365,16 +12372,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=27981,
-  serialized_end=28016,
+  serialized_start=27998,
+  serialized_end=28033,
 )
 
 
 _REQROOMSTART = _descriptor.Descriptor(
   name='ReqRoomStart',
   full_name='lq.ReqRoomStart',
   filename=None,
@@ -12389,16 +12396,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28018,
-  serialized_end=28032,
+  serialized_start=28035,
+  serialized_end=28049,
 )
 
 
 _REQROOMKICK = _descriptor.Descriptor(
   name='ReqRoomKick',
   full_name='lq.ReqRoomKick',
   filename=None,
@@ -12420,16 +12427,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28034,
-  serialized_end=28067,
+  serialized_start=28051,
+  serialized_end=28084,
 )
 
 
 _REQMODIFYROOM = _descriptor.Descriptor(
   name='ReqModifyRoom',
   full_name='lq.ReqModifyRoom',
   filename=None,
@@ -12451,16 +12458,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28069,
-  serialized_end=28105,
+  serialized_start=28086,
+  serialized_end=28122,
 )
 
 
 _REQCHANGEAVATAR = _descriptor.Descriptor(
   name='ReqChangeAvatar',
   full_name='lq.ReqChangeAvatar',
   filename=None,
@@ -12482,16 +12489,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28107,
-  serialized_end=28143,
+  serialized_start=28124,
+  serialized_end=28160,
 )
 
 
 _REQACCOUNTSTATISTICINFO = _descriptor.Descriptor(
   name='ReqAccountStatisticInfo',
   full_name='lq.ReqAccountStatisticInfo',
   filename=None,
@@ -12513,16 +12520,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28145,
-  serialized_end=28190,
+  serialized_start=28162,
+  serialized_end=28207,
 )
 
 
 _RESACCOUNTSTATISTICINFO = _descriptor.Descriptor(
   name='ResAccountStatisticInfo',
   full_name='lq.ResAccountStatisticInfo',
   filename=None,
@@ -12558,16 +12565,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28193,
-  serialized_end=28345,
+  serialized_start=28210,
+  serialized_end=28362,
 )
 
 
 _RESACCOUNTCHALLENGERANKINFO_CHALLENGERANK = _descriptor.Descriptor(
   name='ChallengeRank',
   full_name='lq.ResAccountChallengeRankInfo.ChallengeRank',
   filename=None,
@@ -12603,16 +12610,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28473,
-  serialized_end=28533,
+  serialized_start=28490,
+  serialized_end=28550,
 )
 
 _RESACCOUNTCHALLENGERANKINFO = _descriptor.Descriptor(
   name='ResAccountChallengeRankInfo',
   full_name='lq.ResAccountChallengeRankInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -12640,16 +12647,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28348,
-  serialized_end=28533,
+  serialized_start=28365,
+  serialized_end=28550,
 )
 
 
 _RESACCOUNTCHARACTERINFO = _descriptor.Descriptor(
   name='ResAccountCharacterInfo',
   full_name='lq.ResAccountCharacterInfo',
   filename=None,
@@ -12671,16 +12678,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28535,
-  serialized_end=28581,
+  serialized_start=28552,
+  serialized_end=28598,
 )
 
 
 _REQSHOPPURCHASE = _descriptor.Descriptor(
   name='ReqShopPurchase',
   full_name='lq.ReqShopPurchase',
   filename=None,
@@ -12709,16 +12716,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28583,
-  serialized_end=28626,
+  serialized_start=28600,
+  serialized_end=28643,
 )
 
 
 _RESSHOPPURCHASE = _descriptor.Descriptor(
   name='ResShopPurchase',
   full_name='lq.ResShopPurchase',
   filename=None,
@@ -12747,16 +12754,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28628,
-  serialized_end=28706,
+  serialized_start=28645,
+  serialized_end=28723,
 )
 
 
 _REQGAMERECORD = _descriptor.Descriptor(
   name='ReqGameRecord',
   full_name='lq.ReqGameRecord',
   filename=None,
@@ -12778,16 +12785,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28708,
-  serialized_end=28742,
+  serialized_start=28725,
+  serialized_end=28759,
 )
 
 
 _RESGAMERECORD = _descriptor.Descriptor(
   name='ResGameRecord',
   full_name='lq.ResGameRecord',
   filename=None,
@@ -12830,16 +12837,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28744,
-  serialized_end=28847,
+  serialized_start=28761,
+  serialized_end=28864,
 )
 
 
 _REQGAMERECORDLIST = _descriptor.Descriptor(
   name='ReqGameRecordList',
   full_name='lq.ReqGameRecordList',
   filename=None,
@@ -12875,16 +12882,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28849,
-  serialized_end=28912,
+  serialized_start=28866,
+  serialized_end=28929,
 )
 
 
 _RESGAMERECORDLIST = _descriptor.Descriptor(
   name='ResGameRecordList',
   full_name='lq.ResGameRecordList',
   filename=None,
@@ -12920,16 +12927,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28914,
-  serialized_end=29017,
+  serialized_start=28931,
+  serialized_end=29034,
 )
 
 
 _RESCOLLECTEDGAMERECORDLIST = _descriptor.Descriptor(
   name='ResCollectedGameRecordList',
   full_name='lq.ResCollectedGameRecordList',
   filename=None,
@@ -12965,16 +12972,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29020,
-  serialized_end=29150,
+  serialized_start=29037,
+  serialized_end=29167,
 )
 
 
 _REQGAMERECORDSDETAIL = _descriptor.Descriptor(
   name='ReqGameRecordsDetail',
   full_name='lq.ReqGameRecordsDetail',
   filename=None,
@@ -12996,16 +13003,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29152,
-  serialized_end=29193,
+  serialized_start=29169,
+  serialized_end=29210,
 )
 
 
 _RESGAMERECORDSDETAIL = _descriptor.Descriptor(
   name='ResGameRecordsDetail',
   full_name='lq.ResGameRecordsDetail',
   filename=None,
@@ -13034,16 +13041,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29195,
-  serialized_end=29280,
+  serialized_start=29212,
+  serialized_end=29297,
 )
 
 
 _REQADDCOLLECTEDGAMERECORD = _descriptor.Descriptor(
   name='ReqAddCollectedGameRecord',
   full_name='lq.ReqAddCollectedGameRecord',
   filename=None,
@@ -13086,16 +13093,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29282,
-  serialized_end=29378,
+  serialized_start=29299,
+  serialized_end=29395,
 )
 
 
 _RESADDCOLLECTEDGAMERECORD = _descriptor.Descriptor(
   name='ResAddCollectedGameRecord',
   full_name='lq.ResAddCollectedGameRecord',
   filename=None,
@@ -13117,16 +13124,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29380,
-  serialized_end=29433,
+  serialized_start=29397,
+  serialized_end=29450,
 )
 
 
 _REQREMOVECOLLECTEDGAMERECORD = _descriptor.Descriptor(
   name='ReqRemoveCollectedGameRecord',
   full_name='lq.ReqRemoveCollectedGameRecord',
   filename=None,
@@ -13148,16 +13155,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29435,
-  serialized_end=29479,
+  serialized_start=29452,
+  serialized_end=29496,
 )
 
 
 _RESREMOVECOLLECTEDGAMERECORD = _descriptor.Descriptor(
   name='ResRemoveCollectedGameRecord',
   full_name='lq.ResRemoveCollectedGameRecord',
   filename=None,
@@ -13179,16 +13186,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29481,
-  serialized_end=29537,
+  serialized_start=29498,
+  serialized_end=29554,
 )
 
 
 _REQCHANGECOLLECTEDGAMERECORDREMARKS = _descriptor.Descriptor(
   name='ReqChangeCollectedGameRecordRemarks',
   full_name='lq.ReqChangeCollectedGameRecordRemarks',
   filename=None,
@@ -13217,16 +13224,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29539,
-  serialized_end=29607,
+  serialized_start=29556,
+  serialized_end=29624,
 )
 
 
 _RESCHANGECOLLECTEDGAMERECORDREMARKS = _descriptor.Descriptor(
   name='ResChangeCollectedGameRecordRemarks',
   full_name='lq.ResChangeCollectedGameRecordRemarks',
   filename=None,
@@ -13248,16 +13255,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29609,
-  serialized_end=29672,
+  serialized_start=29626,
+  serialized_end=29689,
 )
 
 
 _REQLEVELLEADERBOARD = _descriptor.Descriptor(
   name='ReqLevelLeaderboard',
   full_name='lq.ReqLevelLeaderboard',
   filename=None,
@@ -13279,16 +13286,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29674,
-  serialized_end=29709,
+  serialized_start=29691,
+  serialized_end=29726,
 )
 
 
 _RESLEVELLEADERBOARD_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.ResLevelLeaderboard.Item',
   filename=None,
@@ -13317,16 +13324,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29825,
-  serialized_end=29884,
+  serialized_start=29842,
+  serialized_end=29901,
 )
 
 _RESLEVELLEADERBOARD = _descriptor.Descriptor(
   name='ResLevelLeaderboard',
   full_name='lq.ResLevelLeaderboard',
   filename=None,
   file=DESCRIPTOR,
@@ -13361,16 +13368,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29712,
-  serialized_end=29884,
+  serialized_start=29729,
+  serialized_end=29901,
 )
 
 
 _REQCHALLANGELEADERBOARD = _descriptor.Descriptor(
   name='ReqChallangeLeaderboard',
   full_name='lq.ReqChallangeLeaderboard',
   filename=None,
@@ -13392,16 +13399,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29886,
-  serialized_end=29927,
+  serialized_start=29903,
+  serialized_end=29944,
 )
 
 
 _RESCHALLENGELEADERBOARD_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.ResChallengeLeaderboard.Item',
   filename=None,
@@ -13437,16 +13444,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30051,
-  serialized_end=30110,
+  serialized_start=30068,
+  serialized_end=30127,
 )
 
 _RESCHALLENGELEADERBOARD = _descriptor.Descriptor(
   name='ResChallengeLeaderboard',
   full_name='lq.ResChallengeLeaderboard',
   filename=None,
   file=DESCRIPTOR,
@@ -13481,16 +13488,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=29930,
-  serialized_end=30110,
+  serialized_start=29947,
+  serialized_end=30127,
 )
 
 
 _REQMUTICHALLENGELEVEL = _descriptor.Descriptor(
   name='ReqMutiChallengeLevel',
   full_name='lq.ReqMutiChallengeLevel',
   filename=None,
@@ -13519,16 +13526,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30112,
-  serialized_end=30176,
+  serialized_start=30129,
+  serialized_end=30193,
 )
 
 
 _RESMUTICHALLENGELEVEL_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.ResMutiChallengeLevel.Item',
   filename=None,
@@ -13557,16 +13564,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30051,
-  serialized_end=30092,
+  serialized_start=30068,
+  serialized_end=30109,
 )
 
 _RESMUTICHALLENGELEVEL = _descriptor.Descriptor(
   name='ResMutiChallengeLevel',
   full_name='lq.ResMutiChallengeLevel',
   filename=None,
   file=DESCRIPTOR,
@@ -13594,16 +13601,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30179,
-  serialized_end=30318,
+  serialized_start=30196,
+  serialized_end=30335,
 )
 
 
 _REQMULTIACCOUNTID = _descriptor.Descriptor(
   name='ReqMultiAccountId',
   full_name='lq.ReqMultiAccountId',
   filename=None,
@@ -13625,16 +13632,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30320,
-  serialized_end=30364,
+  serialized_start=30337,
+  serialized_end=30381,
 )
 
 
 _RESMULTIACCOUNTBRIEF = _descriptor.Descriptor(
   name='ResMultiAccountBrief',
   full_name='lq.ResMultiAccountBrief',
   filename=None,
@@ -13663,16 +13670,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30366,
-  serialized_end=30451,
+  serialized_start=30383,
+  serialized_end=30468,
 )
 
 
 _RESFRIENDLIST = _descriptor.Descriptor(
   name='ResFriendList',
   full_name='lq.ResFriendList',
   filename=None,
@@ -13715,16 +13722,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30453,
-  serialized_end=30571,
+  serialized_start=30470,
+  serialized_end=30588,
 )
 
 
 _RESFRIENDAPPLYLIST_FRIENDAPPLY = _descriptor.Descriptor(
   name='FriendApply',
   full_name='lq.ResFriendApplyList.FriendApply',
   filename=None,
@@ -13753,16 +13760,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30675,
-  serialized_end=30728,
+  serialized_start=30692,
+  serialized_end=30745,
 )
 
 _RESFRIENDAPPLYLIST = _descriptor.Descriptor(
   name='ResFriendApplyList',
   full_name='lq.ResFriendApplyList',
   filename=None,
   file=DESCRIPTOR,
@@ -13790,16 +13797,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30574,
-  serialized_end=30728,
+  serialized_start=30591,
+  serialized_end=30745,
 )
 
 
 _REQAPPLYFRIEND = _descriptor.Descriptor(
   name='ReqApplyFriend',
   full_name='lq.ReqApplyFriend',
   filename=None,
@@ -13821,16 +13828,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30730,
-  serialized_end=30765,
+  serialized_start=30747,
+  serialized_end=30782,
 )
 
 
 _REQHANDLEFRIENDAPPLY = _descriptor.Descriptor(
   name='ReqHandleFriendApply',
   full_name='lq.ReqHandleFriendApply',
   filename=None,
@@ -13859,16 +13866,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30767,
-  serialized_end=30824,
+  serialized_start=30784,
+  serialized_end=30841,
 )
 
 
 _REQREMOVEFRIEND = _descriptor.Descriptor(
   name='ReqRemoveFriend',
   full_name='lq.ReqRemoveFriend',
   filename=None,
@@ -13890,16 +13897,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30826,
-  serialized_end=30862,
+  serialized_start=30843,
+  serialized_end=30879,
 )
 
 
 _REQSEARCHACCOUNTBYPATTERN = _descriptor.Descriptor(
   name='ReqSearchAccountByPattern',
   full_name='lq.ReqSearchAccountByPattern',
   filename=None,
@@ -13928,16 +13935,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30864,
-  serialized_end=30929,
+  serialized_start=30881,
+  serialized_end=30946,
 )
 
 
 _RESSEARCHACCOUNTBYPATTERN = _descriptor.Descriptor(
   name='ResSearchAccountByPattern',
   full_name='lq.ResSearchAccountByPattern',
   filename=None,
@@ -13980,16 +13987,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=30931,
-  serialized_end=31048,
+  serialized_start=30948,
+  serialized_end=31065,
 )
 
 
 _REQACCOUNTLIST = _descriptor.Descriptor(
   name='ReqAccountList',
   full_name='lq.ReqAccountList',
   filename=None,
@@ -14011,16 +14018,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31050,
-  serialized_end=31091,
+  serialized_start=31067,
+  serialized_end=31108,
 )
 
 
 _RESACCOUNTSTATES = _descriptor.Descriptor(
   name='ResAccountStates',
   full_name='lq.ResAccountStates',
   filename=None,
@@ -14049,16 +14056,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31093,
-  serialized_end=31177,
+  serialized_start=31110,
+  serialized_end=31194,
 )
 
 
 _REQSEARCHACCOUNTBYID = _descriptor.Descriptor(
   name='ReqSearchAccountById',
   full_name='lq.ReqSearchAccountById',
   filename=None,
@@ -14080,16 +14087,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31179,
-  serialized_end=31221,
+  serialized_start=31196,
+  serialized_end=31238,
 )
 
 
 _RESSEARCHACCOUNTBYID = _descriptor.Descriptor(
   name='ResSearchAccountById',
   full_name='lq.ResSearchAccountById',
   filename=None,
@@ -14118,16 +14125,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31223,
-  serialized_end=31307,
+  serialized_start=31240,
+  serialized_end=31324,
 )
 
 
 _RESBAGINFO = _descriptor.Descriptor(
   name='ResBagInfo',
   full_name='lq.ResBagInfo',
   filename=None,
@@ -14156,16 +14163,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31309,
-  serialized_end=31369,
+  serialized_start=31326,
+  serialized_end=31386,
 )
 
 
 _REQUSEBAGITEM = _descriptor.Descriptor(
   name='ReqUseBagItem',
   full_name='lq.ReqUseBagItem',
   filename=None,
@@ -14187,16 +14194,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31371,
-  serialized_end=31403,
+  serialized_start=31388,
+  serialized_end=31420,
 )
 
 
 _REQOPENMANUALITEM = _descriptor.Descriptor(
   name='ReqOpenManualItem',
   full_name='lq.ReqOpenManualItem',
   filename=None,
@@ -14232,16 +14239,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31405,
-  serialized_end=31475,
+  serialized_start=31422,
+  serialized_end=31492,
 )
 
 
 _REQOPENRANDOMREWARDITEM = _descriptor.Descriptor(
   name='ReqOpenRandomRewardItem',
   full_name='lq.ReqOpenRandomRewardItem',
   filename=None,
@@ -14263,16 +14270,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31477,
-  serialized_end=31519,
+  serialized_start=31494,
+  serialized_end=31536,
 )
 
 
 _RESOPENRANDOMREWARDITEM = _descriptor.Descriptor(
   name='ResOpenRandomRewardItem',
   full_name='lq.ResOpenRandomRewardItem',
   filename=None,
@@ -14301,16 +14308,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31521,
-  serialized_end=31605,
+  serialized_start=31538,
+  serialized_end=31622,
 )
 
 
 _REQOPENALLREWARDITEM = _descriptor.Descriptor(
   name='ReqOpenAllRewardItem',
   full_name='lq.ReqOpenAllRewardItem',
   filename=None,
@@ -14332,16 +14339,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31607,
-  serialized_end=31646,
+  serialized_start=31624,
+  serialized_end=31663,
 )
 
 
 _RESOPENALLREWARDITEM = _descriptor.Descriptor(
   name='ResOpenAllRewardItem',
   full_name='lq.ResOpenAllRewardItem',
   filename=None,
@@ -14370,16 +14377,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31648,
-  serialized_end=31729,
+  serialized_start=31665,
+  serialized_end=31746,
 )
 
 
 _REQCOMPOSESHARD = _descriptor.Descriptor(
   name='ReqComposeShard',
   full_name='lq.ReqComposeShard',
   filename=None,
@@ -14401,16 +14408,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31731,
-  serialized_end=31765,
+  serialized_start=31748,
+  serialized_end=31782,
 )
 
 
 _REQFETCHANNOUNCEMENT = _descriptor.Descriptor(
   name='ReqFetchAnnouncement',
   full_name='lq.ReqFetchAnnouncement',
   filename=None,
@@ -14432,16 +14439,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31767,
-  serialized_end=31803,
+  serialized_start=31784,
+  serialized_end=31820,
 )
 
 
 _RESANNOUNCEMENT = _descriptor.Descriptor(
   name='ResAnnouncement',
   full_name='lq.ResAnnouncement',
   filename=None,
@@ -14484,16 +14491,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31805,
-  serialized_end=31922,
+  serialized_start=31822,
+  serialized_end=31939,
 )
 
 
 _RESMAILINFO = _descriptor.Descriptor(
   name='ResMailInfo',
   full_name='lq.ResMailInfo',
   filename=None,
@@ -14522,16 +14529,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31924,
-  serialized_end=31988,
+  serialized_start=31941,
+  serialized_end=32005,
 )
 
 
 _REQREADMAIL = _descriptor.Descriptor(
   name='ReqReadMail',
   full_name='lq.ReqReadMail',
   filename=None,
@@ -14553,16 +14560,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=31990,
-  serialized_end=32020,
+  serialized_start=32007,
+  serialized_end=32037,
 )
 
 
 _REQDELETEMAIL = _descriptor.Descriptor(
   name='ReqDeleteMail',
   full_name='lq.ReqDeleteMail',
   filename=None,
@@ -14584,16 +14591,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32022,
-  serialized_end=32054,
+  serialized_start=32039,
+  serialized_end=32071,
 )
 
 
 _REQTAKEATTACHMENT = _descriptor.Descriptor(
   name='ReqTakeAttachment',
   full_name='lq.ReqTakeAttachment',
   filename=None,
@@ -14615,16 +14622,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32056,
-  serialized_end=32092,
+  serialized_start=32073,
+  serialized_end=32109,
 )
 
 
 _REQRECEIVEACHIEVEMENTGROUPREWARD = _descriptor.Descriptor(
   name='ReqReceiveAchievementGroupReward',
   full_name='lq.ReqReceiveAchievementGroupReward',
   filename=None,
@@ -14646,16 +14653,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32094,
-  serialized_end=32146,
+  serialized_start=32111,
+  serialized_end=32163,
 )
 
 
 _RESRECEIVEACHIEVEMENTGROUPREWARD = _descriptor.Descriptor(
   name='ResReceiveAchievementGroupReward',
   full_name='lq.ResReceiveAchievementGroupReward',
   filename=None,
@@ -14684,16 +14691,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32148,
-  serialized_end=32251,
+  serialized_start=32165,
+  serialized_end=32268,
 )
 
 
 _REQRECEIVEACHIEVEMENTREWARD = _descriptor.Descriptor(
   name='ReqReceiveAchievementReward',
   full_name='lq.ReqReceiveAchievementReward',
   filename=None,
@@ -14715,16 +14722,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32253,
-  serialized_end=32306,
+  serialized_start=32270,
+  serialized_end=32323,
 )
 
 
 _RESRECEIVEACHIEVEMENTREWARD = _descriptor.Descriptor(
   name='ResReceiveAchievementReward',
   full_name='lq.ResReceiveAchievementReward',
   filename=None,
@@ -14753,16 +14760,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32308,
-  serialized_end=32406,
+  serialized_start=32325,
+  serialized_end=32423,
 )
 
 
 _RESFETCHACHIEVEMENTRATE_ACHIEVEMENTRATE = _descriptor.Descriptor(
   name='AchievementRate',
   full_name='lq.ResFetchAchievementRate.AchievementRate',
   filename=None,
@@ -14791,16 +14798,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32495,
-  serialized_end=32538,
+  serialized_start=32512,
+  serialized_end=32555,
 )
 
 _RESFETCHACHIEVEMENTRATE = _descriptor.Descriptor(
   name='ResFetchAchievementRate',
   full_name='lq.ResFetchAchievementRate',
   filename=None,
   file=DESCRIPTOR,
@@ -14821,16 +14828,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32409,
-  serialized_end=32538,
+  serialized_start=32426,
+  serialized_end=32555,
 )
 
 
 _RESACHIEVEMENT = _descriptor.Descriptor(
   name='ResAchievement',
   full_name='lq.ResAchievement',
   filename=None,
@@ -14866,16 +14873,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32540,
-  serialized_end=32651,
+  serialized_start=32557,
+  serialized_end=32668,
 )
 
 
 _RESTITLELIST = _descriptor.Descriptor(
   name='ResTitleList',
   full_name='lq.ResTitleList',
   filename=None,
@@ -14904,16 +14911,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32653,
-  serialized_end=32713,
+  serialized_start=32670,
+  serialized_end=32730,
 )
 
 
 _REQUSETITLE = _descriptor.Descriptor(
   name='ReqUseTitle',
   full_name='lq.ReqUseTitle',
   filename=None,
@@ -14935,16 +14942,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32715,
-  serialized_end=32743,
+  serialized_start=32732,
+  serialized_end=32760,
 )
 
 
 _REQBUYSHILIAN = _descriptor.Descriptor(
   name='ReqBuyShiLian',
   full_name='lq.ReqBuyShiLian',
   filename=None,
@@ -14966,16 +14973,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32745,
-  serialized_end=32774,
+  serialized_start=32762,
+  serialized_end=32791,
 )
 
 
 _REQUPDATECLIENTVALUE = _descriptor.Descriptor(
   name='ReqUpdateClientValue',
   full_name='lq.ReqUpdateClientValue',
   filename=None,
@@ -15004,16 +15011,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32776,
-  serialized_end=32826,
+  serialized_start=32793,
+  serialized_end=32843,
 )
 
 
 _RESCLIENTVALUE_VALUE = _descriptor.Descriptor(
   name='Value',
   full_name='lq.ResClientValue.Value',
   filename=None,
@@ -15042,16 +15049,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32912,
-  serialized_end=32947,
+  serialized_start=32929,
+  serialized_end=32964,
 )
 
 _RESCLIENTVALUE = _descriptor.Descriptor(
   name='ResClientValue',
   full_name='lq.ResClientValue',
   filename=None,
   file=DESCRIPTOR,
@@ -15079,16 +15086,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32828,
-  serialized_end=32947,
+  serialized_start=32845,
+  serialized_end=32964,
 )
 
 
 _REQCLIENTMESSAGE = _descriptor.Descriptor(
   name='ReqClientMessage',
   full_name='lq.ReqClientMessage',
   filename=None,
@@ -15117,16 +15124,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=32949,
-  serialized_end=33003,
+  serialized_start=32966,
+  serialized_end=33020,
 )
 
 
 _REQCURRENTMATCHINFO = _descriptor.Descriptor(
   name='ReqCurrentMatchInfo',
   full_name='lq.ReqCurrentMatchInfo',
   filename=None,
@@ -15148,16 +15155,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33005,
-  serialized_end=33045,
+  serialized_start=33022,
+  serialized_end=33062,
 )
 
 
 _RESCURRENTMATCHINFO_CURRENTMATCHINFO = _descriptor.Descriptor(
   name='CurrentMatchInfo',
   full_name='lq.ResCurrentMatchInfo.CurrentMatchInfo',
   filename=None,
@@ -15186,16 +15193,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33156,
-  serialized_end=33214,
+  serialized_start=33173,
+  serialized_end=33231,
 )
 
 _RESCURRENTMATCHINFO = _descriptor.Descriptor(
   name='ResCurrentMatchInfo',
   full_name='lq.ResCurrentMatchInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -15223,16 +15230,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33048,
-  serialized_end=33214,
+  serialized_start=33065,
+  serialized_end=33231,
 )
 
 
 _REQUSERCOMPLAIN = _descriptor.Descriptor(
   name='ReqUserComplain',
   full_name='lq.ReqUserComplain',
   filename=None,
@@ -15261,16 +15268,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33216,
-  serialized_end=33266,
+  serialized_start=33233,
+  serialized_end=33283,
 )
 
 
 _REQREADANNOUNCEMENT = _descriptor.Descriptor(
   name='ReqReadAnnouncement',
   full_name='lq.ReqReadAnnouncement',
   filename=None,
@@ -15292,16 +15299,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33268,
-  serialized_end=33314,
+  serialized_start=33285,
+  serialized_end=33331,
 )
 
 
 _RESREVIVECOININFO = _descriptor.Descriptor(
   name='ResReviveCoinInfo',
   full_name='lq.ResReviveCoinInfo',
   filename=None,
@@ -15330,16 +15337,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33316,
-  serialized_end=33381,
+  serialized_start=33333,
+  serialized_end=33398,
 )
 
 
 _RESDAILYTASK = _descriptor.Descriptor(
   name='ResDailyTask',
   full_name='lq.ResDailyTask',
   filename=None,
@@ -15389,16 +15396,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33384,
-  serialized_end=33542,
+  serialized_start=33401,
+  serialized_end=33559,
 )
 
 
 _REQREFRESHDAILYTASK = _descriptor.Descriptor(
   name='ReqRefreshDailyTask',
   full_name='lq.ReqRefreshDailyTask',
   filename=None,
@@ -15420,16 +15427,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33544,
-  serialized_end=33582,
+  serialized_start=33561,
+  serialized_end=33599,
 )
 
 
 _RESREFRESHDAILYTASK = _descriptor.Descriptor(
   name='ResRefreshDailyTask',
   full_name='lq.ResRefreshDailyTask',
   filename=None,
@@ -15465,16 +15472,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33584,
-  serialized_end=33690,
+  serialized_start=33601,
+  serialized_end=33707,
 )
 
 
 _REQUSEGIFTCODE = _descriptor.Descriptor(
   name='ReqUseGiftCode',
   full_name='lq.ReqUseGiftCode',
   filename=None,
@@ -15496,16 +15503,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33692,
-  serialized_end=33722,
+  serialized_start=33709,
+  serialized_end=33739,
 )
 
 
 _RESUSEGIFTCODE = _descriptor.Descriptor(
   name='ResUseGiftCode',
   full_name='lq.ResUseGiftCode',
   filename=None,
@@ -15534,16 +15541,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33724,
-  serialized_end=33799,
+  serialized_start=33741,
+  serialized_end=33816,
 )
 
 
 _RESUSESPECIALGIFTCODE = _descriptor.Descriptor(
   name='ResUseSpecialGiftCode',
   full_name='lq.ResUseSpecialGiftCode',
   filename=None,
@@ -15572,16 +15579,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33801,
-  serialized_end=33886,
+  serialized_start=33818,
+  serialized_end=33903,
 )
 
 
 _REQSENDCLIENTMESSAGE = _descriptor.Descriptor(
   name='ReqSendClientMessage',
   full_name='lq.ReqSendClientMessage',
   filename=None,
@@ -15617,16 +15624,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33888,
-  serialized_end=33960,
+  serialized_start=33905,
+  serialized_end=33977,
 )
 
 
 _REQGAMELIVEINFO = _descriptor.Descriptor(
   name='ReqGameLiveInfo',
   full_name='lq.ReqGameLiveInfo',
   filename=None,
@@ -15648,16 +15655,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=33962,
-  serialized_end=33998,
+  serialized_start=33979,
+  serialized_end=34015,
 )
 
 
 _RESGAMELIVEINFO = _descriptor.Descriptor(
   name='ResGameLiveInfo',
   full_name='lq.ResGameLiveInfo',
   filename=None,
@@ -15707,16 +15714,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34001,
-  serialized_end=34176,
+  serialized_start=34018,
+  serialized_end=34193,
 )
 
 
 _REQGAMELIVELEFTSEGMENT = _descriptor.Descriptor(
   name='ReqGameLiveLeftSegment',
   full_name='lq.ReqGameLiveLeftSegment',
   filename=None,
@@ -15745,16 +15752,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34178,
-  serialized_end=34246,
+  serialized_start=34195,
+  serialized_end=34263,
 )
 
 
 _RESGAMELIVELEFTSEGMENT = _descriptor.Descriptor(
   name='ResGameLiveLeftSegment',
   full_name='lq.ResGameLiveLeftSegment',
   filename=None,
@@ -15804,16 +15811,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34249,
-  serialized_end=34419,
+  serialized_start=34266,
+  serialized_end=34436,
 )
 
 
 _REQGAMELIVELIST = _descriptor.Descriptor(
   name='ReqGameLiveList',
   full_name='lq.ReqGameLiveList',
   filename=None,
@@ -15835,16 +15842,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34421,
-  serialized_end=34457,
+  serialized_start=34438,
+  serialized_end=34474,
 )
 
 
 _RESGAMELIVELIST = _descriptor.Descriptor(
   name='ResGameLiveList',
   full_name='lq.ResGameLiveList',
   filename=None,
@@ -15873,16 +15880,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34459,
-  serialized_end=34539,
+  serialized_start=34476,
+  serialized_end=34556,
 )
 
 
 _RESCOMMENTSETTING = _descriptor.Descriptor(
   name='ResCommentSetting',
   full_name='lq.ResCommentSetting',
   filename=None,
@@ -15911,16 +15918,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34541,
-  serialized_end=34609,
+  serialized_start=34558,
+  serialized_end=34626,
 )
 
 
 _REQUPDATECOMMENTSETTING = _descriptor.Descriptor(
   name='ReqUpdateCommentSetting',
   full_name='lq.ReqUpdateCommentSetting',
   filename=None,
@@ -15942,16 +15949,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34611,
-  serialized_end=34659,
+  serialized_start=34628,
+  serialized_end=34676,
 )
 
 
 _REQFETCHCOMMENTLIST = _descriptor.Descriptor(
   name='ReqFetchCommentList',
   full_name='lq.ReqFetchCommentList',
   filename=None,
@@ -15973,16 +15980,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34661,
-  serialized_end=34701,
+  serialized_start=34678,
+  serialized_end=34718,
 )
 
 
 _RESFETCHCOMMENTLIST = _descriptor.Descriptor(
   name='ResFetchCommentList',
   full_name='lq.ResFetchCommentList',
   filename=None,
@@ -16025,16 +16032,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34703,
-  serialized_end=34820,
+  serialized_start=34720,
+  serialized_end=34837,
 )
 
 
 _REQFETCHCOMMENTCONTENT = _descriptor.Descriptor(
   name='ReqFetchCommentContent',
   full_name='lq.ReqFetchCommentContent',
   filename=None,
@@ -16063,16 +16070,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34822,
-  serialized_end=34890,
+  serialized_start=34839,
+  serialized_end=34907,
 )
 
 
 _RESFETCHCOMMENTCONTENT = _descriptor.Descriptor(
   name='ResFetchCommentContent',
   full_name='lq.ResFetchCommentContent',
   filename=None,
@@ -16101,16 +16108,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34892,
-  serialized_end=34977,
+  serialized_start=34909,
+  serialized_end=34994,
 )
 
 
 _REQLEAVECOMMENT = _descriptor.Descriptor(
   name='ReqLeaveComment',
   full_name='lq.ReqLeaveComment',
   filename=None,
@@ -16139,16 +16146,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=34979,
-  serialized_end=35032,
+  serialized_start=34996,
+  serialized_end=35049,
 )
 
 
 _REQDELETECOMMENT = _descriptor.Descriptor(
   name='ReqDeleteComment',
   full_name='lq.ReqDeleteComment',
   filename=None,
@@ -16177,16 +16184,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35034,
-  serialized_end=35092,
+  serialized_start=35051,
+  serialized_end=35109,
 )
 
 
 _REQUPDATEREADCOMMENT = _descriptor.Descriptor(
   name='ReqUpdateReadComment',
   full_name='lq.ReqUpdateReadComment',
   filename=None,
@@ -16208,16 +16215,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35094,
-  serialized_end=35133,
+  serialized_start=35111,
+  serialized_end=35150,
 )
 
 
 _REQROLLINGNOTICE = _descriptor.Descriptor(
   name='ReqRollingNotice',
   full_name='lq.ReqRollingNotice',
   filename=None,
@@ -16239,16 +16246,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35135,
-  serialized_end=35188,
+  serialized_start=35152,
+  serialized_end=35205,
 )
 
 
 _RESSERVERTIME = _descriptor.Descriptor(
   name='ResServerTime',
   full_name='lq.ResServerTime',
   filename=None,
@@ -16270,16 +16277,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35190,
-  serialized_end=35226,
+  serialized_start=35207,
+  serialized_end=35243,
 )
 
 
 _REQPLATFORMBILLINGPRODUCTS = _descriptor.Descriptor(
   name='ReqPlatformBillingProducts',
   full_name='lq.ReqPlatformBillingProducts',
   filename=None,
@@ -16301,16 +16308,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35228,
-  serialized_end=35276,
+  serialized_start=35245,
+  serialized_end=35293,
 )
 
 
 _RESPLATFORMBILLINGPRODUCTS = _descriptor.Descriptor(
   name='ResPlatformBillingProducts',
   full_name='lq.ResPlatformBillingProducts',
   filename=None,
@@ -16339,16 +16346,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35278,
-  serialized_end=35370,
+  serialized_start=35295,
+  serialized_end=35387,
 )
 
 
 _REQCREATEBILLINGORDER = _descriptor.Descriptor(
   name='ReqCreateBillingOrder',
   full_name='lq.ReqCreateBillingOrder',
   filename=None,
@@ -16391,16 +16398,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35372,
-  serialized_end=35480,
+  serialized_start=35389,
+  serialized_end=35497,
 )
 
 
 _RESCREATEBILLINGORDER = _descriptor.Descriptor(
   name='ResCreateBillingOrder',
   full_name='lq.ResCreateBillingOrder',
   filename=None,
@@ -16429,16 +16436,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35482,
-  serialized_end=35549,
+  serialized_start=35499,
+  serialized_end=35566,
 )
 
 
 _REQSOLVEGOOGLEPLAYORDER = _descriptor.Descriptor(
   name='ReqSolveGooglePlayOrder',
   full_name='lq.ReqSolveGooglePlayOrder',
   filename=None,
@@ -16467,16 +16474,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35551,
-  serialized_end=35635,
+  serialized_start=35568,
+  serialized_end=35652,
 )
 
 
 _REQSOLVEGOOGLEPLAYORDERV3 = _descriptor.Descriptor(
   name='ReqSolveGooglePlayOrderV3',
   full_name='lq.ReqSolveGooglePlayOrderV3',
   filename=None,
@@ -16519,16 +16526,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35637,
-  serialized_end=35741,
+  serialized_start=35654,
+  serialized_end=35758,
 )
 
 
 _REQCANCELGOOGLEPLAYORDER = _descriptor.Descriptor(
   name='ReqCancelGooglePlayOrder',
   full_name='lq.ReqCancelGooglePlayOrder',
   filename=None,
@@ -16550,16 +16557,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35743,
-  serialized_end=35787,
+  serialized_start=35760,
+  serialized_end=35804,
 )
 
 
 _REQCREATEWECHATNATIVEORDER = _descriptor.Descriptor(
   name='ReqCreateWechatNativeOrder',
   full_name='lq.ReqCreateWechatNativeOrder',
   filename=None,
@@ -16602,16 +16609,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35789,
-  serialized_end=35896,
+  serialized_start=35806,
+  serialized_end=35913,
 )
 
 
 _RESCREATEWECHATNATIVEORDER = _descriptor.Descriptor(
   name='ResCreateWechatNativeOrder',
   full_name='lq.ResCreateWechatNativeOrder',
   filename=None,
@@ -16647,16 +16654,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35898,
-  serialized_end=35993,
+  serialized_start=35915,
+  serialized_end=36010,
 )
 
 
 _REQCREATEWECHATAPPORDER = _descriptor.Descriptor(
   name='ReqCreateWechatAppOrder',
   full_name='lq.ReqCreateWechatAppOrder',
   filename=None,
@@ -16699,16 +16706,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=35995,
-  serialized_end=36099,
+  serialized_start=36012,
+  serialized_end=36116,
 )
 
 
 _RESCREATEWECHATAPPORDER_CALLWECHATAPPPARAM = _descriptor.Descriptor(
   name='CallWechatAppParam',
   full_name='lq.ResCreateWechatAppOrder.CallWechatAppParam',
   filename=None,
@@ -16772,16 +16779,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36235,
-  serialized_end=36375,
+  serialized_start=36252,
+  serialized_end=36392,
 )
 
 _RESCREATEWECHATAPPORDER = _descriptor.Descriptor(
   name='ResCreateWechatAppOrder',
   full_name='lq.ResCreateWechatAppOrder',
   filename=None,
   file=DESCRIPTOR,
@@ -16809,16 +16816,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36102,
-  serialized_end=36375,
+  serialized_start=36119,
+  serialized_end=36392,
 )
 
 
 _REQCREATEALIPAYORDER = _descriptor.Descriptor(
   name='ReqCreateAlipayOrder',
   full_name='lq.ReqCreateAlipayOrder',
   filename=None,
@@ -16868,16 +16875,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36378,
-  serialized_end=36506,
+  serialized_start=36395,
+  serialized_end=36523,
 )
 
 
 _RESCREATEALIPAYORDER = _descriptor.Descriptor(
   name='ResCreateAlipayOrder',
   full_name='lq.ResCreateAlipayOrder',
   filename=None,
@@ -16906,16 +16913,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36508,
-  serialized_end=36576,
+  serialized_start=36525,
+  serialized_end=36593,
 )
 
 
 _REQCREATEALIPAYSCANORDER = _descriptor.Descriptor(
   name='ReqCreateAlipayScanOrder',
   full_name='lq.ReqCreateAlipayScanOrder',
   filename=None,
@@ -16951,16 +16958,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36578,
-  serialized_end=36663,
+  serialized_start=36595,
+  serialized_end=36680,
 )
 
 
 _RESCREATEALIPAYSCANORDER = _descriptor.Descriptor(
   name='ResCreateAlipayScanOrder',
   full_name='lq.ResCreateAlipayScanOrder',
   filename=None,
@@ -17003,16 +17010,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36665,
-  serialized_end=36775,
+  serialized_start=36682,
+  serialized_end=36792,
 )
 
 
 _REQCREATEALIPAYAPPORDER = _descriptor.Descriptor(
   name='ReqCreateAlipayAppOrder',
   full_name='lq.ReqCreateAlipayAppOrder',
   filename=None,
@@ -17048,16 +17055,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36777,
-  serialized_end=36861,
+  serialized_start=36794,
+  serialized_end=36878,
 )
 
 
 _RESCREATEALIPAYAPPORDER = _descriptor.Descriptor(
   name='ResCreateAlipayAppOrder',
   full_name='lq.ResCreateAlipayAppOrder',
   filename=None,
@@ -17086,16 +17093,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36863,
-  serialized_end=36934,
+  serialized_start=36880,
+  serialized_end=36951,
 )
 
 
 _REQCREATEJPCREDITCARDORDER = _descriptor.Descriptor(
   name='ReqCreateJPCreditCardOrder',
   full_name='lq.ReqCreateJPCreditCardOrder',
   filename=None,
@@ -17145,16 +17152,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=36937,
-  serialized_end=37066,
+  serialized_start=36954,
+  serialized_end=37083,
 )
 
 
 _RESCREATEJPCREDITCARDORDER = _descriptor.Descriptor(
   name='ResCreateJPCreditCardOrder',
   full_name='lq.ResCreateJPCreditCardOrder',
   filename=None,
@@ -17183,16 +17190,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37068,
-  serialized_end=37140,
+  serialized_start=37085,
+  serialized_end=37157,
 )
 
 
 _REQCREATEJPPAYPALORDER = _descriptor.Descriptor(
   name='ReqCreateJPPaypalOrder',
   full_name='lq.ReqCreateJPPaypalOrder',
   filename=None,
@@ -17242,16 +17249,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37142,
-  serialized_end=37267,
+  serialized_start=37159,
+  serialized_end=37284,
 )
 
 
 _RESCREATEJPPAYPALORDER = _descriptor.Descriptor(
   name='ResCreateJPPaypalOrder',
   full_name='lq.ResCreateJPPaypalOrder',
   filename=None,
@@ -17280,16 +17287,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37269,
-  serialized_end=37337,
+  serialized_start=37286,
+  serialized_end=37354,
 )
 
 
 _REQCREATEJPAUORDER = _descriptor.Descriptor(
   name='ReqCreateJPAuOrder',
   full_name='lq.ReqCreateJPAuOrder',
   filename=None,
@@ -17339,16 +17346,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37339,
-  serialized_end=37460,
+  serialized_start=37356,
+  serialized_end=37477,
 )
 
 
 _RESCREATEJPAUORDER = _descriptor.Descriptor(
   name='ResCreateJPAuOrder',
   full_name='lq.ResCreateJPAuOrder',
   filename=None,
@@ -17377,16 +17384,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37462,
-  serialized_end=37526,
+  serialized_start=37479,
+  serialized_end=37543,
 )
 
 
 _REQCREATEJPDOCOMOORDER = _descriptor.Descriptor(
   name='ReqCreateJPDocomoOrder',
   full_name='lq.ReqCreateJPDocomoOrder',
   filename=None,
@@ -17436,16 +17443,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37528,
-  serialized_end=37653,
+  serialized_start=37545,
+  serialized_end=37670,
 )
 
 
 _RESCREATEJPDOCOMOORDER = _descriptor.Descriptor(
   name='ResCreateJPDocomoOrder',
   full_name='lq.ResCreateJPDocomoOrder',
   filename=None,
@@ -17474,16 +17481,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37655,
-  serialized_end=37723,
+  serialized_start=37672,
+  serialized_end=37740,
 )
 
 
 _REQCREATEJPWEBMONEYORDER = _descriptor.Descriptor(
   name='ReqCreateJPWebMoneyOrder',
   full_name='lq.ReqCreateJPWebMoneyOrder',
   filename=None,
@@ -17533,16 +17540,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37725,
-  serialized_end=37852,
+  serialized_start=37742,
+  serialized_end=37869,
 )
 
 
 _RESCREATEJPWEBMONEYORDER = _descriptor.Descriptor(
   name='ResCreateJPWebMoneyOrder',
   full_name='lq.ResCreateJPWebMoneyOrder',
   filename=None,
@@ -17571,16 +17578,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37854,
-  serialized_end=37924,
+  serialized_start=37871,
+  serialized_end=37941,
 )
 
 
 _REQCREATEJPSOFTBANKORDER = _descriptor.Descriptor(
   name='ReqCreateJPSoftbankOrder',
   full_name='lq.ReqCreateJPSoftbankOrder',
   filename=None,
@@ -17630,16 +17637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=37926,
-  serialized_end=38053,
+  serialized_start=37943,
+  serialized_end=38070,
 )
 
 
 _RESCREATEJPSOFTBANKORDER = _descriptor.Descriptor(
   name='ResCreateJPSoftbankOrder',
   full_name='lq.ResCreateJPSoftbankOrder',
   filename=None,
@@ -17668,16 +17675,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38055,
-  serialized_end=38125,
+  serialized_start=38072,
+  serialized_end=38142,
 )
 
 
 _REQCREATEYOSTARORDER = _descriptor.Descriptor(
   name='ReqCreateYostarOrder',
   full_name='lq.ReqCreateYostarOrder',
   filename=None,
@@ -17720,16 +17727,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38127,
-  serialized_end=38228,
+  serialized_start=38144,
+  serialized_end=38245,
 )
 
 
 _RESCREATEYOSTARORDER = _descriptor.Descriptor(
   name='ResCreateYostarOrder',
   full_name='lq.ResCreateYostarOrder',
   filename=None,
@@ -17758,16 +17765,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38230,
-  serialized_end=38296,
+  serialized_start=38247,
+  serialized_end=38313,
 )
 
 
 _REQCREATEENPAYPALORDER = _descriptor.Descriptor(
   name='ReqCreateENPaypalOrder',
   full_name='lq.ReqCreateENPaypalOrder',
   filename=None,
@@ -17817,16 +17824,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38298,
-  serialized_end=38423,
+  serialized_start=38315,
+  serialized_end=38440,
 )
 
 
 _RESCREATEENPAYPALORDER = _descriptor.Descriptor(
   name='ResCreateENPaypalOrder',
   full_name='lq.ResCreateENPaypalOrder',
   filename=None,
@@ -17855,16 +17862,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38425,
-  serialized_end=38493,
+  serialized_start=38442,
+  serialized_end=38510,
 )
 
 
 _REQCREATEENJCBORDER = _descriptor.Descriptor(
   name='ReqCreateENJCBOrder',
   full_name='lq.ReqCreateENJCBOrder',
   filename=None,
@@ -17914,16 +17921,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38495,
-  serialized_end=38617,
+  serialized_start=38512,
+  serialized_end=38634,
 )
 
 
 _RESCREATEENJCBORDER = _descriptor.Descriptor(
   name='ResCreateENJCBOrder',
   full_name='lq.ResCreateENJCBOrder',
   filename=None,
@@ -17952,16 +17959,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38619,
-  serialized_end=38684,
+  serialized_start=38636,
+  serialized_end=38701,
 )
 
 
 _REQCREATEENMASTERCARDORDER = _descriptor.Descriptor(
   name='ReqCreateENMasterCardOrder',
   full_name='lq.ReqCreateENMasterCardOrder',
   filename=None,
@@ -18011,16 +18018,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38687,
-  serialized_end=38816,
+  serialized_start=38704,
+  serialized_end=38833,
 )
 
 
 _RESCREATEENMASTERCARDORDER = _descriptor.Descriptor(
   name='ResCreateENMasterCardOrder',
   full_name='lq.ResCreateENMasterCardOrder',
   filename=None,
@@ -18049,16 +18056,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38818,
-  serialized_end=38890,
+  serialized_start=38835,
+  serialized_end=38907,
 )
 
 
 _REQCREATEENVISAORDER = _descriptor.Descriptor(
   name='ReqCreateENVisaOrder',
   full_name='lq.ReqCreateENVisaOrder',
   filename=None,
@@ -18108,16 +18115,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38892,
-  serialized_end=39015,
+  serialized_start=38909,
+  serialized_end=39032,
 )
 
 
 _RESCREATEENVISAORDER = _descriptor.Descriptor(
   name='ResCreateENVisaOrder',
   full_name='lq.ResCreateENVisaOrder',
   filename=None,
@@ -18146,16 +18153,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39017,
-  serialized_end=39083,
+  serialized_start=39034,
+  serialized_end=39100,
 )
 
 
 _REQCREATEENALIPAYORDER = _descriptor.Descriptor(
   name='ReqCreateENAlipayOrder',
   full_name='lq.ReqCreateENAlipayOrder',
   filename=None,
@@ -18205,16 +18212,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39085,
-  serialized_end=39210,
+  serialized_start=39102,
+  serialized_end=39227,
 )
 
 
 _RESCREATEENALIPAYORDER = _descriptor.Descriptor(
   name='ResCreateENAlipayOrder',
   full_name='lq.ResCreateENAlipayOrder',
   filename=None,
@@ -18243,16 +18250,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39212,
-  serialized_end=39280,
+  serialized_start=39229,
+  serialized_end=39297,
 )
 
 
 _REQCREATEDMMORDER = _descriptor.Descriptor(
   name='ReqCreateDMMOrder',
   full_name='lq.ReqCreateDMMOrder',
   filename=None,
@@ -18288,16 +18295,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39282,
-  serialized_end=39360,
+  serialized_start=39299,
+  serialized_end=39377,
 )
 
 
 _RESCREATEDMMORDER = _descriptor.Descriptor(
   name='ResCreateDmmOrder',
   full_name='lq.ResCreateDmmOrder',
   filename=None,
@@ -18368,16 +18375,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39363,
-  serialized_end=39550,
+  serialized_start=39380,
+  serialized_end=39567,
 )
 
 
 _REQCREATEIAPORDER = _descriptor.Descriptor(
   name='ReqCreateIAPOrder',
   full_name='lq.ReqCreateIAPOrder',
   filename=None,
@@ -18420,16 +18427,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39552,
-  serialized_end=39652,
+  serialized_start=39569,
+  serialized_end=39669,
 )
 
 
 _RESCREATEIAPORDER = _descriptor.Descriptor(
   name='ResCreateIAPOrder',
   full_name='lq.ResCreateIAPOrder',
   filename=None,
@@ -18458,16 +18465,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39654,
-  serialized_end=39717,
+  serialized_start=39671,
+  serialized_end=39734,
 )
 
 
 _REQVERIFICATIONIAPORDER = _descriptor.Descriptor(
   name='ReqVerificationIAPOrder',
   full_name='lq.ReqVerificationIAPOrder',
   filename=None,
@@ -18510,16 +18517,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39719,
-  serialized_end=39828,
+  serialized_start=39736,
+  serialized_end=39845,
 )
 
 
 _RESVERIFICATIONIAPORDER = _descriptor.Descriptor(
   name='ResVerificationIAPOrder',
   full_name='lq.ResVerificationIAPOrder',
   filename=None,
@@ -18541,16 +18548,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39830,
-  serialized_end=39881,
+  serialized_start=39847,
+  serialized_end=39898,
 )
 
 
 _REQCREATESTEAMORDER = _descriptor.Descriptor(
   name='ReqCreateSteamOrder',
   full_name='lq.ReqCreateSteamOrder',
   filename=None,
@@ -18600,16 +18607,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=39883,
-  serialized_end=39999,
+  serialized_start=39900,
+  serialized_end=40016,
 )
 
 
 _RESCREATESTEAMORDER = _descriptor.Descriptor(
   name='ResCreateSteamOrder',
   full_name='lq.ResCreateSteamOrder',
   filename=None,
@@ -18645,16 +18652,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40001,
-  serialized_end=40093,
+  serialized_start=40018,
+  serialized_end=40110,
 )
 
 
 _REQVERIFYSTEAMORDER = _descriptor.Descriptor(
   name='ReqVerifySteamOrder',
   full_name='lq.ReqVerifySteamOrder',
   filename=None,
@@ -18683,16 +18690,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40095,
-  serialized_end=40154,
+  serialized_start=40112,
+  serialized_end=40171,
 )
 
 
 _REQCREATEMYCARDORDER = _descriptor.Descriptor(
   name='ReqCreateMyCardOrder',
   full_name='lq.ReqCreateMyCardOrder',
   filename=None,
@@ -18728,16 +18735,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40156,
-  serialized_end=40237,
+  serialized_start=40173,
+  serialized_end=40254,
 )
 
 
 _RESCREATEMYCARDORDER = _descriptor.Descriptor(
   name='ResCreateMyCardOrder',
   full_name='lq.ResCreateMyCardOrder',
   filename=None,
@@ -18773,16 +18780,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40239,
-  serialized_end=40324,
+  serialized_start=40256,
+  serialized_end=40341,
 )
 
 
 _REQVERIFYMYCARDORDER = _descriptor.Descriptor(
   name='ReqVerifyMyCardOrder',
   full_name='lq.ReqVerifyMyCardOrder',
   filename=None,
@@ -18811,16 +18818,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40326,
-  serialized_end=40386,
+  serialized_start=40343,
+  serialized_end=40403,
 )
 
 
 _REQCREATEPAYPALORDER = _descriptor.Descriptor(
   name='ReqCreatePaypalOrder',
   full_name='lq.ReqCreatePaypalOrder',
   filename=None,
@@ -18856,16 +18863,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40388,
-  serialized_end=40469,
+  serialized_start=40405,
+  serialized_end=40486,
 )
 
 
 _RESCREATEPAYPALORDER = _descriptor.Descriptor(
   name='ResCreatePaypalOrder',
   full_name='lq.ResCreatePaypalOrder',
   filename=None,
@@ -18901,16 +18908,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40471,
-  serialized_end=40550,
+  serialized_start=40488,
+  serialized_end=40567,
 )
 
 
 _REQCREATEXSOLLAORDER = _descriptor.Descriptor(
   name='ReqCreateXsollaOrder',
   full_name='lq.ReqCreateXsollaOrder',
   filename=None,
@@ -18953,16 +18960,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40552,
-  serialized_end=40657,
+  serialized_start=40569,
+  serialized_end=40674,
 )
 
 
 _RESCREATEXSOLLAORDER = _descriptor.Descriptor(
   name='ResCreateXsollaOrder',
   full_name='lq.ResCreateXsollaOrder',
   filename=None,
@@ -18998,16 +19005,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40659,
-  serialized_end=40738,
+  serialized_start=40676,
+  serialized_end=40755,
 )
 
 
 _REQOPENCHEST = _descriptor.Descriptor(
   name='ReqOpenChest',
   full_name='lq.ReqOpenChest',
   filename=None,
@@ -19043,16 +19050,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40740,
-  serialized_end=40807,
+  serialized_start=40757,
+  serialized_end=40824,
 )
 
 
 _RESOPENCHEST_CHESTREPLACECOUNTDATA = _descriptor.Descriptor(
   name='ChestReplaceCountData',
   full_name='lq.ResOpenChest.ChestReplaceCountData',
   filename=None,
@@ -19081,16 +19088,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40998,
-  serialized_end=41048,
+  serialized_start=41015,
+  serialized_end=41065,
 )
 
 _RESOPENCHEST = _descriptor.Descriptor(
   name='ResOpenChest',
   full_name='lq.ResOpenChest',
   filename=None,
   file=DESCRIPTOR,
@@ -19139,16 +19146,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=40810,
-  serialized_end=41048,
+  serialized_start=40827,
+  serialized_end=41065,
 )
 
 
 _REQBUYFROMCHESTSHOP = _descriptor.Descriptor(
   name='ReqBuyFromChestShop',
   full_name='lq.ReqBuyFromChestShop',
   filename=None,
@@ -19177,16 +19184,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41050,
-  serialized_end=41104,
+  serialized_start=41067,
+  serialized_end=41121,
 )
 
 
 _RESBUYFROMCHESTSHOP = _descriptor.Descriptor(
   name='ResBuyFromChestShop',
   full_name='lq.ResBuyFromChestShop',
   filename=None,
@@ -19229,16 +19236,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41106,
-  serialized_end=41215,
+  serialized_start=41123,
+  serialized_end=41232,
 )
 
 
 _RESDAILYSIGNININFO = _descriptor.Descriptor(
   name='ResDailySignInInfo',
   full_name='lq.ResDailySignInInfo',
   filename=None,
@@ -19267,16 +19274,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41217,
-  serialized_end=41285,
+  serialized_start=41234,
+  serialized_end=41302,
 )
 
 
 _REQDOACTIVITYSIGNIN = _descriptor.Descriptor(
   name='ReqDoActivitySignIn',
   full_name='lq.ReqDoActivitySignIn',
   filename=None,
@@ -19298,16 +19305,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41287,
-  serialized_end=41329,
+  serialized_start=41304,
+  serialized_end=41346,
 )
 
 
 _RESDOACTIVITYSIGNIN_REWARDDATA = _descriptor.Descriptor(
   name='RewardData',
   full_name='lq.ResDoActivitySignIn.RewardData',
   filename=None,
@@ -19336,16 +19343,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41457,
-  serialized_end=41505,
+  serialized_start=41474,
+  serialized_end=41522,
 )
 
 _RESDOACTIVITYSIGNIN = _descriptor.Descriptor(
   name='ResDoActivitySignIn',
   full_name='lq.ResDoActivitySignIn',
   filename=None,
   file=DESCRIPTOR,
@@ -19380,16 +19387,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41332,
-  serialized_end=41505,
+  serialized_start=41349,
+  serialized_end=41522,
 )
 
 
 _RESCHARACTERINFO = _descriptor.Descriptor(
   name='ResCharacterInfo',
   full_name='lq.ResCharacterInfo',
   filename=None,
@@ -19467,16 +19474,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41508,
-  serialized_end=41755,
+  serialized_start=41525,
+  serialized_end=41772,
 )
 
 
 _REQUPDATECHARACTERSORT = _descriptor.Descriptor(
   name='ReqUpdateCharacterSort',
   full_name='lq.ReqUpdateCharacterSort',
   filename=None,
@@ -19498,16 +19505,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41757,
-  serialized_end=41795,
+  serialized_start=41774,
+  serialized_end=41812,
 )
 
 
 _REQCHANGEMAINCHARACTER = _descriptor.Descriptor(
   name='ReqChangeMainCharacter',
   full_name='lq.ReqChangeMainCharacter',
   filename=None,
@@ -19529,16 +19536,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41797,
-  serialized_end=41843,
+  serialized_start=41814,
+  serialized_end=41860,
 )
 
 
 _REQCHANGECHARACTERSKIN = _descriptor.Descriptor(
   name='ReqChangeCharacterSkin',
   full_name='lq.ReqChangeCharacterSkin',
   filename=None,
@@ -19567,16 +19574,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41845,
-  serialized_end=41905,
+  serialized_start=41862,
+  serialized_end=41922,
 )
 
 
 _REQCHANGECHARACTERVIEW = _descriptor.Descriptor(
   name='ReqChangeCharacterView',
   full_name='lq.ReqChangeCharacterView',
   filename=None,
@@ -19612,16 +19619,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41907,
-  serialized_end=41984,
+  serialized_start=41924,
+  serialized_end=42001,
 )
 
 
 _REQSENDGIFTTOCHARACTER_GIFT = _descriptor.Descriptor(
   name='Gift',
   full_name='lq.ReqSendGiftToCharacter.Gift',
   filename=None,
@@ -19650,16 +19657,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42083,
-  serialized_end=42121,
+  serialized_start=42100,
+  serialized_end=42138,
 )
 
 _REQSENDGIFTTOCHARACTER = _descriptor.Descriptor(
   name='ReqSendGiftToCharacter',
   full_name='lq.ReqSendGiftToCharacter',
   filename=None,
   file=DESCRIPTOR,
@@ -19687,16 +19694,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=41987,
-  serialized_end=42121,
+  serialized_start=42004,
+  serialized_end=42138,
 )
 
 
 _RESSENDGIFTTOCHARACTER = _descriptor.Descriptor(
   name='ResSendGiftToCharacter',
   full_name='lq.ResSendGiftToCharacter',
   filename=None,
@@ -19732,16 +19739,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42123,
-  serialized_end=42201,
+  serialized_start=42140,
+  serialized_end=42218,
 )
 
 
 _REQSELLITEM_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.ReqSellItem.Item',
   filename=None,
@@ -19770,16 +19777,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42255,
-  serialized_end=42293,
+  serialized_start=42272,
+  serialized_end=42310,
 )
 
 _REQSELLITEM = _descriptor.Descriptor(
   name='ReqSellItem',
   full_name='lq.ReqSellItem',
   filename=None,
   file=DESCRIPTOR,
@@ -19800,16 +19807,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42203,
-  serialized_end=42293,
+  serialized_start=42220,
+  serialized_end=42310,
 )
 
 
 _RESCOMMONVIEW_SLOT = _descriptor.Descriptor(
   name='Slot',
   full_name='lq.ResCommonView.Slot',
   filename=None,
@@ -19838,16 +19845,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42377,
-  serialized_end=42412,
+  serialized_start=42394,
+  serialized_end=42429,
 )
 
 _RESCOMMONVIEW = _descriptor.Descriptor(
   name='ResCommonView',
   full_name='lq.ResCommonView',
   filename=None,
   file=DESCRIPTOR,
@@ -19875,16 +19882,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42295,
-  serialized_end=42412,
+  serialized_start=42312,
+  serialized_end=42429,
 )
 
 
 _REQCHANGECOMMONVIEW = _descriptor.Descriptor(
   name='ReqChangeCommonView',
   full_name='lq.ReqChangeCommonView',
   filename=None,
@@ -19913,16 +19920,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42414,
-  serialized_end=42464,
+  serialized_start=42431,
+  serialized_end=42481,
 )
 
 
 _REQSAVECOMMONVIEWS = _descriptor.Descriptor(
   name='ReqSaveCommonViews',
   full_name='lq.ReqSaveCommonViews',
   filename=None,
@@ -19958,16 +19965,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42466,
-  serialized_end=42551,
+  serialized_start=42483,
+  serialized_end=42568,
 )
 
 
 _REQCOMMONVIEWS = _descriptor.Descriptor(
   name='ReqCommonViews',
   full_name='lq.ReqCommonViews',
   filename=None,
@@ -19989,16 +19996,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42553,
-  serialized_end=42584,
+  serialized_start=42570,
+  serialized_end=42601,
 )
 
 
 _RESCOMMONVIEWS = _descriptor.Descriptor(
   name='ResCommonViews',
   full_name='lq.ResCommonViews',
   filename=None,
@@ -20020,16 +20027,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42586,
-  serialized_end=42631,
+  serialized_start=42603,
+  serialized_end=42648,
 )
 
 
 _RESALLCOMMONVIEWS_VIEWS = _descriptor.Descriptor(
   name='Views',
   full_name='lq.ResAllcommonViews.Views',
   filename=None,
@@ -20058,16 +20065,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42738,
-  serialized_end=42790,
+  serialized_start=42755,
+  serialized_end=42807,
 )
 
 _RESALLCOMMONVIEWS = _descriptor.Descriptor(
   name='ResAllcommonViews',
   full_name='lq.ResAllcommonViews',
   filename=None,
   file=DESCRIPTOR,
@@ -20102,16 +20109,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42634,
-  serialized_end=42790,
+  serialized_start=42651,
+  serialized_end=42807,
 )
 
 
 _REQUSECOMMONVIEW = _descriptor.Descriptor(
   name='ReqUseCommonView',
   full_name='lq.ReqUseCommonView',
   filename=None,
@@ -20133,16 +20140,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42792,
-  serialized_end=42825,
+  serialized_start=42809,
+  serialized_end=42842,
 )
 
 
 _REQUPGRADECHARACTER = _descriptor.Descriptor(
   name='ReqUpgradeCharacter',
   full_name='lq.ReqUpgradeCharacter',
   filename=None,
@@ -20164,16 +20171,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42827,
-  serialized_end=42870,
+  serialized_start=42844,
+  serialized_end=42887,
 )
 
 
 _RESUPGRADECHARACTER = _descriptor.Descriptor(
   name='ResUpgradeCharacter',
   full_name='lq.ResUpgradeCharacter',
   filename=None,
@@ -20202,16 +20209,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42872,
-  serialized_end=42953,
+  serialized_start=42889,
+  serialized_end=42970,
 )
 
 
 _REQFINISHEDENDING = _descriptor.Descriptor(
   name='ReqFinishedEnding',
   full_name='lq.ReqFinishedEnding',
   filename=None,
@@ -20247,16 +20254,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42955,
-  serialized_end=43033,
+  serialized_start=42972,
+  serialized_end=43050,
 )
 
 
 _REQGMCOMMAND = _descriptor.Descriptor(
   name='ReqGMCommand',
   full_name='lq.ReqGMCommand',
   filename=None,
@@ -20278,16 +20285,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43035,
-  serialized_end=43066,
+  serialized_start=43052,
+  serialized_end=43083,
 )
 
 
 _RESSHOPINFO = _descriptor.Descriptor(
   name='ResShopInfo',
   full_name='lq.ResShopInfo',
   filename=None,
@@ -20316,16 +20323,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43068,
-  serialized_end=43140,
+  serialized_start=43085,
+  serialized_end=43157,
 )
 
 
 _REQBUYFROMSHOP = _descriptor.Descriptor(
   name='ReqBuyFromShop',
   full_name='lq.ReqBuyFromShop',
   filename=None,
@@ -20368,16 +20375,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43142,
-  serialized_end=43253,
+  serialized_start=43159,
+  serialized_end=43270,
 )
 
 
 _RESBUYFROMSHOP = _descriptor.Descriptor(
   name='ResBuyFromShop',
   full_name='lq.ResBuyFromShop',
   filename=None,
@@ -20406,16 +20413,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43255,
-  serialized_end=43330,
+  serialized_start=43272,
+  serialized_end=43347,
 )
 
 
 _REQBUYFROMZHP = _descriptor.Descriptor(
   name='ReqBuyFromZHP',
   full_name='lq.ReqBuyFromZHP',
   filename=None,
@@ -20444,16 +20451,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43332,
-  serialized_end=43380,
+  serialized_start=43349,
+  serialized_end=43397,
 )
 
 
 _REQPAYMONTHTICKET = _descriptor.Descriptor(
   name='ReqPayMonthTicket',
   full_name='lq.ReqPayMonthTicket',
   filename=None,
@@ -20475,16 +20482,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43382,
-  serialized_end=43420,
+  serialized_start=43399,
+  serialized_end=43437,
 )
 
 
 _RESPAYMONTHTICKET = _descriptor.Descriptor(
   name='ResPayMonthTicket',
   full_name='lq.ResPayMonthTicket',
   filename=None,
@@ -20520,16 +20527,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43422,
-  serialized_end=43512,
+  serialized_start=43439,
+  serialized_end=43529,
 )
 
 
 _REQRESHZHPSHOP = _descriptor.Descriptor(
   name='ReqReshZHPShop',
   full_name='lq.ReqReshZHPShop',
   filename=None,
@@ -20558,16 +20565,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43514,
-  serialized_end=43574,
+  serialized_start=43531,
+  serialized_end=43591,
 )
 
 
 _RESREFRESHZHPSHOP = _descriptor.Descriptor(
   name='ResRefreshZHPShop',
   full_name='lq.ResRefreshZHPShop',
   filename=None,
@@ -20596,16 +20603,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43576,
-  serialized_end=43647,
+  serialized_start=43593,
+  serialized_end=43664,
 )
 
 
 _RESMONTHTICKETINFO = _descriptor.Descriptor(
   name='ResMonthTicketInfo',
   full_name='lq.ResMonthTicketInfo',
   filename=None,
@@ -20627,16 +20634,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43649,
-  serialized_end=43717,
+  serialized_start=43666,
+  serialized_end=43734,
 )
 
 
 _REQEXCHANGECURRENCY = _descriptor.Descriptor(
   name='ReqExchangeCurrency',
   full_name='lq.ReqExchangeCurrency',
   filename=None,
@@ -20665,16 +20672,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43719,
-  serialized_end=43767,
+  serialized_start=43736,
+  serialized_end=43784,
 )
 
 
 _RESSERVERSETTINGS = _descriptor.Descriptor(
   name='ResServerSettings',
   full_name='lq.ResServerSettings',
   filename=None,
@@ -20696,16 +20703,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43769,
-  serialized_end=43826,
+  serialized_start=43786,
+  serialized_end=43843,
 )
 
 
 _RESACCOUNTSETTINGS = _descriptor.Descriptor(
   name='ResAccountSettings',
   full_name='lq.ResAccountSettings',
   filename=None,
@@ -20734,16 +20741,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43828,
-  serialized_end=43912,
+  serialized_start=43845,
+  serialized_end=43929,
 )
 
 
 _REQUPDATEACCOUNTSETTINGS = _descriptor.Descriptor(
   name='ReqUpdateAccountSettings',
   full_name='lq.ReqUpdateAccountSettings',
   filename=None,
@@ -20765,16 +20772,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43914,
-  serialized_end=43977,
+  serialized_start=43931,
+  serialized_end=43994,
 )
 
 
 _RESMODNICKNAMETIME = _descriptor.Descriptor(
   name='ResModNicknameTime',
   full_name='lq.ResModNicknameTime',
   filename=None,
@@ -20796,16 +20803,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=43979,
-  serialized_end=44022,
+  serialized_start=43996,
+  serialized_end=44039,
 )
 
 
 _RESMISC_MISCFAITHDATA = _descriptor.Descriptor(
   name='MiscFaithData',
   full_name='lq.ResMisc.MiscFaithData',
   filename=None,
@@ -20834,16 +20841,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44129,
-  serialized_end=44177,
+  serialized_start=44146,
+  serialized_end=44194,
 )
 
 _RESMISC = _descriptor.Descriptor(
   name='ResMisc',
   full_name='lq.ResMisc',
   filename=None,
   file=DESCRIPTOR,
@@ -20878,16 +20885,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44025,
-  serialized_end=44177,
+  serialized_start=44042,
+  serialized_end=44194,
 )
 
 
 _REQMODIFYSIGNATURE = _descriptor.Descriptor(
   name='ReqModifySignature',
   full_name='lq.ReqModifySignature',
   filename=None,
@@ -20909,16 +20916,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44179,
-  serialized_end=44218,
+  serialized_start=44196,
+  serialized_end=44235,
 )
 
 
 _RESIDCARDINFO = _descriptor.Descriptor(
   name='ResIDCardInfo',
   full_name='lq.ResIDCardInfo',
   filename=None,
@@ -20954,16 +20961,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44220,
-  serialized_end=44297,
+  serialized_start=44237,
+  serialized_end=44314,
 )
 
 
 _REQUPDATEIDCARDINFO = _descriptor.Descriptor(
   name='ReqUpdateIDCardInfo',
   full_name='lq.ReqUpdateIDCardInfo',
   filename=None,
@@ -20992,16 +20999,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44299,
-  serialized_end=44355,
+  serialized_start=44316,
+  serialized_end=44372,
 )
 
 
 _RESVIPREWARD = _descriptor.Descriptor(
   name='ResVipReward',
   full_name='lq.ResVipReward',
   filename=None,
@@ -21030,16 +21037,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44357,
-  serialized_end=44424,
+  serialized_start=44374,
+  serialized_end=44441,
 )
 
 
 _REQGAINVIPREWARD = _descriptor.Descriptor(
   name='ReqGainVipReward',
   full_name='lq.ReqGainVipReward',
   filename=None,
@@ -21061,16 +21068,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44426,
-  serialized_end=44463,
+  serialized_start=44443,
+  serialized_end=44480,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTLIST = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestList',
   full_name='lq.ReqFetchCustomizedContestList',
   filename=None,
@@ -21099,16 +21106,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44465,
-  serialized_end=44526,
+  serialized_start=44482,
+  serialized_end=44543,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTLIST = _descriptor.Descriptor(
   name='ResFetchCustomizedContestList',
   full_name='lq.ResFetchCustomizedContestList',
   filename=None,
@@ -21144,16 +21151,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44529,
-  serialized_end=44683,
+  serialized_start=44546,
+  serialized_end=44700,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTEXTENDINFO = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestExtendInfo',
   full_name='lq.ReqFetchCustomizedContestExtendInfo',
   filename=None,
@@ -21175,16 +21182,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44685,
-  serialized_end=44740,
+  serialized_start=44702,
+  serialized_end=44757,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTEXTENDINFO = _descriptor.Descriptor(
   name='ResFetchCustomizedContestExtendInfo',
   full_name='lq.ResFetchCustomizedContestExtendInfo',
   filename=None,
@@ -21213,16 +21220,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44742,
-  serialized_end=44855,
+  serialized_start=44759,
+  serialized_end=44872,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTAUTHINFO = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestAuthInfo',
   full_name='lq.ReqFetchCustomizedContestAuthInfo',
   filename=None,
@@ -21244,16 +21251,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44857,
-  serialized_end=44911,
+  serialized_start=44874,
+  serialized_end=44928,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTAUTHINFO = _descriptor.Descriptor(
   name='ResFetchCustomizedContestAuthInfo',
   full_name='lq.ResFetchCustomizedContestAuthInfo',
   filename=None,
@@ -21282,16 +21289,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=44913,
-  serialized_end=44998,
+  serialized_start=44930,
+  serialized_end=45015,
 )
 
 
 _REQENTERCUSTOMIZEDCONTEST = _descriptor.Descriptor(
   name='ReqEnterCustomizedContest',
   full_name='lq.ReqEnterCustomizedContest',
   filename=None,
@@ -21313,16 +21320,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45000,
-  serialized_end=45046,
+  serialized_start=45017,
+  serialized_end=45063,
 )
 
 
 _RESENTERCUSTOMIZEDCONTEST = _descriptor.Descriptor(
   name='ResEnterCustomizedContest',
   full_name='lq.ResEnterCustomizedContest',
   filename=None,
@@ -21365,16 +21372,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45049,
-  serialized_end=45231,
+  serialized_start=45066,
+  serialized_end=45248,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTONLINEINFO = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestOnlineInfo',
   full_name='lq.ReqFetchCustomizedContestOnlineInfo',
   filename=None,
@@ -21396,16 +21403,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45233,
-  serialized_end=45289,
+  serialized_start=45250,
+  serialized_end=45306,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTONLINEINFO = _descriptor.Descriptor(
   name='ResFetchCustomizedContestOnlineInfo',
   full_name='lq.ResFetchCustomizedContestOnlineInfo',
   filename=None,
@@ -21434,16 +21441,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45291,
-  serialized_end=45377,
+  serialized_start=45308,
+  serialized_end=45394,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTBYCONTESTID = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestByContestId',
   full_name='lq.ReqFetchCustomizedContestByContestId',
   filename=None,
@@ -21465,16 +21472,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45379,
-  serialized_end=45437,
+  serialized_start=45396,
+  serialized_end=45454,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTBYCONTESTID = _descriptor.Descriptor(
   name='ResFetchCustomizedContestByContestId',
   full_name='lq.ResFetchCustomizedContestByContestId',
   filename=None,
@@ -21503,16 +21510,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45439,
-  serialized_end=45556,
+  serialized_start=45456,
+  serialized_end=45573,
 )
 
 
 _REQSTARTCUSTOMIZEDCONTEST = _descriptor.Descriptor(
   name='ReqStartCustomizedContest',
   full_name='lq.ReqStartCustomizedContest',
   filename=None,
@@ -21534,16 +21541,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45558,
-  serialized_end=45604,
+  serialized_start=45575,
+  serialized_end=45621,
 )
 
 
 _REQJOINCUSTOMIZEDCONTESTCHATROOM = _descriptor.Descriptor(
   name='ReqJoinCustomizedContestChatRoom',
   full_name='lq.ReqJoinCustomizedContestChatRoom',
   filename=None,
@@ -21565,16 +21572,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45606,
-  serialized_end=45659,
+  serialized_start=45623,
+  serialized_end=45676,
 )
 
 
 _RESJOINCUSTOMIZEDCONTESTCHATROOM = _descriptor.Descriptor(
   name='ResJoinCustomizedContestChatRoom',
   full_name='lq.ResJoinCustomizedContestChatRoom',
   filename=None,
@@ -21603,16 +21610,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45661,
-  serialized_end=45743,
+  serialized_start=45678,
+  serialized_end=45760,
 )
 
 
 _REQSAYCHATMESSAGE = _descriptor.Descriptor(
   name='ReqSayChatMessage',
   full_name='lq.ReqSayChatMessage',
   filename=None,
@@ -21634,16 +21641,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45745,
-  serialized_end=45781,
+  serialized_start=45762,
+  serialized_end=45798,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTGAMELIVELIST = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestGameLiveList',
   full_name='lq.ReqFetchCustomizedContestGameLiveList',
   filename=None,
@@ -21665,16 +21672,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45783,
-  serialized_end=45841,
+  serialized_start=45800,
+  serialized_end=45858,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTGAMELIVELIST = _descriptor.Descriptor(
   name='ResFetchCustomizedContestGameLiveList',
   full_name='lq.ResFetchCustomizedContestGameLiveList',
   filename=None,
@@ -21703,16 +21710,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45843,
-  serialized_end=45945,
+  serialized_start=45860,
+  serialized_end=45962,
 )
 
 
 _REQFETCHCUSTOMIZEDCONTESTGAMERECORDS = _descriptor.Descriptor(
   name='ReqFetchCustomizedContestGameRecords',
   full_name='lq.ReqFetchCustomizedContestGameRecords',
   filename=None,
@@ -21741,16 +21748,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=45947,
-  serialized_end=46024,
+  serialized_start=45964,
+  serialized_end=46041,
 )
 
 
 _RESFETCHCUSTOMIZEDCONTESTGAMERECORDS = _descriptor.Descriptor(
   name='ResFetchCustomizedContestGameRecords',
   full_name='lq.ResFetchCustomizedContestGameRecords',
   filename=None,
@@ -21786,16 +21793,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46026,
-  serialized_end=46147,
+  serialized_start=46043,
+  serialized_end=46164,
 )
 
 
 _REQTARGETCUSTOMIZEDCONTEST = _descriptor.Descriptor(
   name='ReqTargetCustomizedContest',
   full_name='lq.ReqTargetCustomizedContest',
   filename=None,
@@ -21817,16 +21824,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46149,
-  serialized_end=46196,
+  serialized_start=46166,
+  serialized_end=46213,
 )
 
 
 _RESACTIVITYLIST = _descriptor.Descriptor(
   name='ResActivityList',
   full_name='lq.ResActivityList',
   filename=None,
@@ -21855,16 +21862,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46198,
-  serialized_end=46275,
+  serialized_start=46215,
+  serialized_end=46292,
 )
 
 
 _RESACCOUNTACTIVITYDATA_ACTIVITYSIGNINDATA = _descriptor.Descriptor(
   name='ActivitySignInData',
   full_name='lq.ResAccountActivityData.ActivitySignInData',
   filename=None,
@@ -21900,16 +21907,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46898,
-  serialized_end=46989,
+  serialized_start=46915,
+  serialized_end=47006,
 )
 
 _RESACCOUNTACTIVITYDATA_BUFFDATA = _descriptor.Descriptor(
   name='BuffData',
   full_name='lq.ResAccountActivityData.BuffData',
   filename=None,
   file=DESCRIPTOR,
@@ -21944,16 +21951,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46991,
-  serialized_end=47047,
+  serialized_start=47008,
+  serialized_end=47064,
 )
 
 _RESACCOUNTACTIVITYDATA_ACTIVITYRICHMANDATA = _descriptor.Descriptor(
   name='ActivityRichmanData',
   full_name='lq.ResAccountActivityData.ActivityRichmanData',
   filename=None,
   file=DESCRIPTOR,
@@ -22016,16 +22023,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47050,
-  serialized_end=47241,
+  serialized_start=47067,
+  serialized_end=47258,
 )
 
 _RESACCOUNTACTIVITYDATA_CHESTUPDATA = _descriptor.Descriptor(
   name='ChestUpData',
   full_name='lq.ResAccountActivityData.ChestUpData',
   filename=None,
   file=DESCRIPTOR,
@@ -22053,16 +22060,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47243,
-  serialized_end=47283,
+  serialized_start=47260,
+  serialized_end=47300,
 )
 
 _RESACCOUNTACTIVITYDATA = _descriptor.Descriptor(
   name='ResAccountActivityData',
   full_name='lq.ResAccountActivityData',
   filename=None,
   file=DESCRIPTOR,
@@ -22153,16 +22160,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46278,
-  serialized_end=47283,
+  serialized_start=46295,
+  serialized_end=47300,
 )
 
 
 _REQEXCHANGEACTIVITYITEM = _descriptor.Descriptor(
   name='ReqExchangeActivityItem',
   full_name='lq.ReqExchangeActivityItem',
   filename=None,
@@ -22191,16 +22198,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47285,
-  serialized_end=47346,
+  serialized_start=47302,
+  serialized_end=47363,
 )
 
 
 _RESEXCHANGEACTIVITYITEM = _descriptor.Descriptor(
   name='ResExchangeActivityItem',
   full_name='lq.ResExchangeActivityItem',
   filename=None,
@@ -22229,16 +22236,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47348,
-  serialized_end=47442,
+  serialized_start=47365,
+  serialized_end=47459,
 )
 
 
 _REQCOMPLETEACTIVITYTASK = _descriptor.Descriptor(
   name='ReqCompleteActivityTask',
   full_name='lq.ReqCompleteActivityTask',
   filename=None,
@@ -22260,16 +22267,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47444,
-  serialized_end=47486,
+  serialized_start=47461,
+  serialized_end=47503,
 )
 
 
 _REQRECEIVEACTIVITYFLIPTASK = _descriptor.Descriptor(
   name='ReqReceiveActivityFlipTask',
   full_name='lq.ReqReceiveActivityFlipTask',
   filename=None,
@@ -22291,16 +22298,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47488,
-  serialized_end=47533,
+  serialized_start=47505,
+  serialized_end=47550,
 )
 
 
 _RESRECEIVEACTIVITYFLIPTASK = _descriptor.Descriptor(
   name='ResReceiveActivityFlipTask',
   full_name='lq.ResReceiveActivityFlipTask',
   filename=None,
@@ -22329,16 +22336,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47535,
-  serialized_end=47604,
+  serialized_start=47552,
+  serialized_end=47621,
 )
 
 
 _REQFETCHACTIVITYFLIPINFO = _descriptor.Descriptor(
   name='ReqFetchActivityFlipInfo',
   full_name='lq.ReqFetchActivityFlipInfo',
   filename=None,
@@ -22360,16 +22367,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47606,
-  serialized_end=47653,
+  serialized_start=47623,
+  serialized_end=47670,
 )
 
 
 _RESFETCHACTIVITYFLIPINFO = _descriptor.Descriptor(
   name='ResFetchActivityFlipInfo',
   full_name='lq.ResFetchActivityFlipInfo',
   filename=None,
@@ -22405,16 +22412,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47655,
-  serialized_end=47739,
+  serialized_start=47672,
+  serialized_end=47756,
 )
 
 
 _REQGAINACCUMULATEDPOINTACTIVITYREWARD = _descriptor.Descriptor(
   name='ReqGainAccumulatedPointActivityReward',
   full_name='lq.ReqGainAccumulatedPointActivityReward',
   filename=None,
@@ -22443,16 +22450,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47741,
-  serialized_end=47820,
+  serialized_start=47758,
+  serialized_end=47837,
 )
 
 
 _REQGAINMULTIPOINTACTIVITYREWARD = _descriptor.Descriptor(
   name='ReqGainMultiPointActivityReward',
   full_name='lq.ReqGainMultiPointActivityReward',
   filename=None,
@@ -22481,16 +22488,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47822,
-  serialized_end=47900,
+  serialized_start=47839,
+  serialized_end=47917,
 )
 
 
 _REQFETCHRANKPOINTLEADERBOARD = _descriptor.Descriptor(
   name='ReqFetchRankPointLeaderboard',
   full_name='lq.ReqFetchRankPointLeaderboard',
   filename=None,
@@ -22512,16 +22519,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47902,
-  serialized_end=47956,
+  serialized_start=47919,
+  serialized_end=47973,
 )
 
 
 _RESFETCHRANKPOINTLEADERBOARD_ITEM = _descriptor.Descriptor(
   name='Item',
   full_name='lq.ResFetchRankPointLeaderboard.Item',
   filename=None,
@@ -22564,16 +22571,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48098,
-  serialized_end=48187,
+  serialized_start=48115,
+  serialized_end=48204,
 )
 
 _RESFETCHRANKPOINTLEADERBOARD = _descriptor.Descriptor(
   name='ResFetchRankPointLeaderboard',
   full_name='lq.ResFetchRankPointLeaderboard',
   filename=None,
   file=DESCRIPTOR,
@@ -22608,16 +22615,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=47959,
-  serialized_end=48187,
+  serialized_start=47976,
+  serialized_end=48204,
 )
 
 
 _REQGAINRANKPOINTREWARD = _descriptor.Descriptor(
   name='ReqGainRankPointReward',
   full_name='lq.ReqGainRankPointReward',
   filename=None,
@@ -22646,16 +22653,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48189,
-  serialized_end=48258,
+  serialized_start=48206,
+  serialized_end=48275,
 )
 
 
 _REQRICHMANNEXTMOVE = _descriptor.Descriptor(
   name='ReqRichmanNextMove',
   full_name='lq.ReqRichmanNextMove',
   filename=None,
@@ -22677,16 +22684,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48260,
-  serialized_end=48301,
+  serialized_start=48277,
+  serialized_end=48318,
 )
 
 
 _RESRICHMANNEXTMOVE_REWARDDATA = _descriptor.Descriptor(
   name='RewardData',
   full_name='lq.ResRichmanNextMove.RewardData',
   filename=None,
@@ -22729,16 +22736,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48596,
-  serialized_end=48680,
+  serialized_start=48613,
+  serialized_end=48697,
 )
 
 _RESRICHMANNEXTMOVE_PATHDATA = _descriptor.Descriptor(
   name='PathData',
   full_name='lq.ResRichmanNextMove.PathData',
   filename=None,
   file=DESCRIPTOR,
@@ -22773,16 +22780,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48682,
-  serialized_end=48778,
+  serialized_start=48699,
+  serialized_end=48795,
 )
 
 _RESRICHMANNEXTMOVE_BUFFDATA = _descriptor.Descriptor(
   name='BuffData',
   full_name='lq.ResRichmanNextMove.BuffData',
   filename=None,
   file=DESCRIPTOR,
@@ -22817,16 +22824,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=46991,
-  serialized_end=47047,
+  serialized_start=47008,
+  serialized_end=47064,
 )
 
 _RESRICHMANNEXTMOVE = _descriptor.Descriptor(
   name='ResRichmanNextMove',
   full_name='lq.ResRichmanNextMove',
   filename=None,
   file=DESCRIPTOR,
@@ -22917,16 +22924,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48304,
-  serialized_end=48836,
+  serialized_start=48321,
+  serialized_end=48853,
 )
 
 
 _REQRICHMANSPECIALMOVE = _descriptor.Descriptor(
   name='ReqRichmanSpecialMove',
   full_name='lq.ReqRichmanSpecialMove',
   filename=None,
@@ -22955,16 +22962,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48838,
-  serialized_end=48896,
+  serialized_start=48855,
+  serialized_end=48913,
 )
 
 
 _REQRICHMANCHESTINFO = _descriptor.Descriptor(
   name='ReqRichmanChestInfo',
   full_name='lq.ReqRichmanChestInfo',
   filename=None,
@@ -22986,16 +22993,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48898,
-  serialized_end=48940,
+  serialized_start=48915,
+  serialized_end=48957,
 )
 
 
 _RESRICHMANCHESTINFO_ITEMDATA = _descriptor.Descriptor(
   name='ItemData',
   full_name='lq.ResRichmanChestInfo.ItemData',
   filename=None,
@@ -23024,16 +23031,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49041,
-  serialized_end=49078,
+  serialized_start=49058,
+  serialized_end=49095,
 )
 
 _RESRICHMANCHESTINFO = _descriptor.Descriptor(
   name='ResRichmanChestInfo',
   full_name='lq.ResRichmanChestInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -23061,16 +23068,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=48943,
-  serialized_end=49078,
+  serialized_start=48960,
+  serialized_end=49095,
 )
 
 
 _REQCREATEGAMEOBSERVEAUTH = _descriptor.Descriptor(
   name='ReqCreateGameObserveAuth',
   full_name='lq.ReqCreateGameObserveAuth',
   filename=None,
@@ -23092,16 +23099,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49080,
-  serialized_end=49125,
+  serialized_start=49097,
+  serialized_end=49142,
 )
 
 
 _RESCREATEGAMEOBSERVEAUTH = _descriptor.Descriptor(
   name='ResCreateGameObserveAuth',
   full_name='lq.ResCreateGameObserveAuth',
   filename=None,
@@ -23137,16 +23144,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49127,
-  serialized_end=49212,
+  serialized_start=49144,
+  serialized_end=49229,
 )
 
 
 _REQREFRESHGAMEOBSERVEAUTH = _descriptor.Descriptor(
   name='ReqRefreshGameObserveAuth',
   full_name='lq.ReqRefreshGameObserveAuth',
   filename=None,
@@ -23168,16 +23175,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49214,
-  serialized_end=49256,
+  serialized_start=49231,
+  serialized_end=49273,
 )
 
 
 _RESREFRESHGAMEOBSERVEAUTH = _descriptor.Descriptor(
   name='ResRefreshGameObserveAuth',
   full_name='lq.ResRefreshGameObserveAuth',
   filename=None,
@@ -23206,16 +23213,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49258,
-  serialized_end=49324,
+  serialized_start=49275,
+  serialized_end=49341,
 )
 
 
 _RESACTIVITYBUFF_ACTIVITYBUFFDATA = _descriptor.Descriptor(
   name='ActivityBuffData',
   full_name='lq.ResActivityBuff.ActivityBuffData',
   filename=None,
@@ -23244,16 +23251,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49429,
-  serialized_end=49479,
+  serialized_start=49446,
+  serialized_end=49496,
 )
 
 _RESACTIVITYBUFF = _descriptor.Descriptor(
   name='ResActivityBuff',
   full_name='lq.ResActivityBuff',
   filename=None,
   file=DESCRIPTOR,
@@ -23281,16 +23288,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49327,
-  serialized_end=49479,
+  serialized_start=49344,
+  serialized_end=49496,
 )
 
 
 _REQUPGRADEACTIVITYBUFF = _descriptor.Descriptor(
   name='ReqUpgradeActivityBuff',
   full_name='lq.ReqUpgradeActivityBuff',
   filename=None,
@@ -23312,16 +23319,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49481,
-  serialized_end=49522,
+  serialized_start=49498,
+  serialized_end=49539,
 )
 
 
 _RESUPGRADECHALLENGE = _descriptor.Descriptor(
   name='ResUpgradeChallenge',
   full_name='lq.ResUpgradeChallenge',
   filename=None,
@@ -23378,16 +23385,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49525,
-  serialized_end=49691,
+  serialized_start=49542,
+  serialized_end=49708,
 )
 
 
 _RESREFRESHCHALLENGE = _descriptor.Descriptor(
   name='ResRefreshChallenge',
   full_name='lq.ResRefreshChallenge',
   filename=None,
@@ -23444,16 +23451,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49694,
-  serialized_end=49860,
+  serialized_start=49711,
+  serialized_end=49877,
 )
 
 
 _RESFETCHCHALLENGEINFO = _descriptor.Descriptor(
   name='ResFetchChallengeInfo',
   full_name='lq.ResFetchChallengeInfo',
   filename=None,
@@ -23517,16 +23524,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=49863,
-  serialized_end=50056,
+  serialized_start=49880,
+  serialized_end=50073,
 )
 
 
 _REQFORCECOMPLETECHALLENGETASK = _descriptor.Descriptor(
   name='ReqForceCompleteChallengeTask',
   full_name='lq.ReqForceCompleteChallengeTask',
   filename=None,
@@ -23548,16 +23555,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50058,
-  serialized_end=50106,
+  serialized_start=50075,
+  serialized_end=50123,
 )
 
 
 _RESFETCHABMATCH_MATCHPOINT = _descriptor.Descriptor(
   name='MatchPoint',
   full_name='lq.ResFetchABMatch.MatchPoint',
   filename=None,
@@ -23665,16 +23672,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50109,
-  serialized_end=50364,
+  serialized_start=50126,
+  serialized_end=50381,
 )
 
 
 _REQSTARTUNIFIEDMATCH = _descriptor.Descriptor(
   name='ReqStartUnifiedMatch',
   full_name='lq.ReqStartUnifiedMatch',
   filename=None,
@@ -23696,16 +23703,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50366,
-  serialized_end=50407,
+  serialized_start=50383,
+  serialized_end=50424,
 )
 
 
 _REQCANCELUNIFIEDMATCH = _descriptor.Descriptor(
   name='ReqCancelUnifiedMatch',
   full_name='lq.ReqCancelUnifiedMatch',
   filename=None,
@@ -23727,16 +23734,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50409,
-  serialized_end=50451,
+  serialized_start=50426,
+  serialized_end=50468,
 )
 
 
 _RESCHALLENGESEASONINFO_CHALLENGEINFO = _descriptor.Descriptor(
   name='ChallengeInfo',
   full_name='lq.ResChallengeSeasonInfo.ChallengeInfo',
   filename=None,
@@ -23779,16 +23786,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50553,
-  serialized_end=50640,
+  serialized_start=50570,
+  serialized_end=50657,
 )
 
 _RESCHALLENGESEASONINFO = _descriptor.Descriptor(
   name='ResChallengeSeasonInfo',
   full_name='lq.ResChallengeSeasonInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -23809,16 +23816,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50454,
-  serialized_end=50640,
+  serialized_start=50471,
+  serialized_end=50657,
 )
 
 
 _REQRECEIVECHALLENGERANKREWARD = _descriptor.Descriptor(
   name='ReqReceiveChallengeRankReward',
   full_name='lq.ReqReceiveChallengeRankReward',
   filename=None,
@@ -23840,16 +23847,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50642,
-  serialized_end=50692,
+  serialized_start=50659,
+  serialized_end=50709,
 )
 
 
 _RESRECEIVECHALLENGERANKREWARD_REWARD = _descriptor.Descriptor(
   name='Reward',
   full_name='lq.ResReceiveChallengeRankReward.Reward',
   filename=None,
@@ -23878,16 +23885,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50787,
-  serialized_end=50831,
+  serialized_start=50804,
+  serialized_end=50848,
 )
 
 _RESRECEIVECHALLENGERANKREWARD = _descriptor.Descriptor(
   name='ResReceiveChallengeRankReward',
   full_name='lq.ResReceiveChallengeRankReward',
   filename=None,
   file=DESCRIPTOR,
@@ -23908,16 +23915,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50695,
-  serialized_end=50831,
+  serialized_start=50712,
+  serialized_end=50848,
 )
 
 
 _REQBUYINABMATCH = _descriptor.Descriptor(
   name='ReqBuyInABMatch',
   full_name='lq.ReqBuyInABMatch',
   filename=None,
@@ -23939,16 +23946,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50833,
-  serialized_end=50868,
+  serialized_start=50850,
+  serialized_end=50885,
 )
 
 
 _REQGAMEPOINTRANK = _descriptor.Descriptor(
   name='ReqGamePointRank',
   full_name='lq.ReqGamePointRank',
   filename=None,
@@ -23970,16 +23977,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50870,
-  serialized_end=50909,
+  serialized_start=50887,
+  serialized_end=50926,
 )
 
 
 _RESGAMEPOINTRANK_RANKINFO = _descriptor.Descriptor(
   name='RankInfo',
   full_name='lq.ResGamePointRank.RankInfo',
   filename=None,
@@ -24008,16 +24015,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51022,
-  serialized_end=51067,
+  serialized_start=51039,
+  serialized_end=51084,
 )
 
 _RESGAMEPOINTRANK = _descriptor.Descriptor(
   name='ResGamePointRank',
   full_name='lq.ResGamePointRank',
   filename=None,
   file=DESCRIPTOR,
@@ -24052,16 +24059,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=50912,
-  serialized_end=51067,
+  serialized_start=50929,
+  serialized_end=51084,
 )
 
 
 _RESFETCHSELFGAMEPOINTRANK = _descriptor.Descriptor(
   name='ResFetchSelfGamePointRank',
   full_name='lq.ResFetchSelfGamePointRank',
   filename=None,
@@ -24090,16 +24097,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51069,
-  serialized_end=51141,
+  serialized_start=51086,
+  serialized_end=51158,
 )
 
 
 _ACTIONMJSTART = _descriptor.Descriptor(
   name='ActionMJStart',
   full_name='lq.ActionMJStart',
   filename=None,
@@ -24114,16 +24121,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51143,
-  serialized_end=51158,
+  serialized_start=51160,
+  serialized_end=51175,
 )
 
 
 _NEWROUNDOPENEDTILES = _descriptor.Descriptor(
   name='NewRoundOpenedTiles',
   full_name='lq.NewRoundOpenedTiles',
   filename=None,
@@ -24159,16 +24166,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51160,
-  serialized_end=51225,
+  serialized_start=51177,
+  serialized_end=51242,
 )
 
 
 _MUYUINFO = _descriptor.Descriptor(
   name='MuyuInfo',
   full_name='lq.MuyuInfo',
   filename=None,
@@ -24211,16 +24218,75 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51227,
-  serialized_end=51297,
+  serialized_start=51244,
+  serialized_end=51314,
+)
+
+
+_CHUANMAGANG = _descriptor.Descriptor(
+  name='ChuanmaGang',
+  full_name='lq.ChuanmaGang',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='old_scores', full_name='lq.ChuanmaGang.old_scores', index=0,
+      number=1, type=5, cpp_type=1, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='delta_scores', full_name='lq.ChuanmaGang.delta_scores', index=1,
+      number=2, type=5, cpp_type=1, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='scores', full_name='lq.ChuanmaGang.scores', index=2,
+      number=3, type=5, cpp_type=1, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='gameend', full_name='lq.ChuanmaGang.gameend', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='hules_history', full_name='lq.ChuanmaGang.hules_history', index=4,
+      number=5, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=51317,
+  serialized_end=51455,
 )
 
 
 _ACTIONNEWROUND = _descriptor.Descriptor(
   name='ActionNewRound',
   full_name='lq.ActionNewRound',
   filename=None,
@@ -24335,28 +24401,35 @@
     _descriptor.FieldDescriptor(
       name='muyu', full_name='lq.ActionNewRound.muyu', index=15,
       number=16, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='ju_count', full_name='lq.ActionNewRound.ju_count', index=16,
+      number=17, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51300,
-  serialized_end=51677,
+  serialized_start=51458,
+  serialized_end=51853,
 )
 
 
 _RECORDNEWROUND_TINGPAI = _descriptor.Descriptor(
   name='TingPai',
   full_name='lq.RecordNewRound.TingPai',
   filename=None,
@@ -24385,16 +24458,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52126,
-  serialized_end=52185,
+  serialized_start=52320,
+  serialized_end=52379,
 )
 
 _RECORDNEWROUND = _descriptor.Descriptor(
   name='RecordNewRound',
   full_name='lq.RecordNewRound',
   filename=None,
   file=DESCRIPTOR,
@@ -24529,28 +24602,35 @@
     _descriptor.FieldDescriptor(
       name='operations', full_name='lq.RecordNewRound.operations', index=18,
       number=19, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='ju_count', full_name='lq.RecordNewRound.ju_count', index=19,
+      number=20, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[_RECORDNEWROUND_TINGPAI, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=51680,
-  serialized_end=52185,
+  serialized_start=51856,
+  serialized_end=52379,
 )
 
 
 _GAMESNAPSHOT_PLAYERSNAPSHOT_FULU = _descriptor.Descriptor(
   name='Fulu',
   full_name='lq.GameSnapshot.PlayerSnapshot.Fulu',
   filename=None,
@@ -24586,16 +24666,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52549,
-  serialized_end=52597,
+  serialized_start=52743,
+  serialized_end=52791,
 )
 
 _GAMESNAPSHOT_PLAYERSNAPSHOT = _descriptor.Descriptor(
   name='PlayerSnapshot',
   full_name='lq.GameSnapshot.PlayerSnapshot',
   filename=None,
   file=DESCRIPTOR,
@@ -24644,16 +24724,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52408,
-  serialized_end=52597,
+  serialized_start=52602,
+  serialized_end=52791,
 )
 
 _GAMESNAPSHOT = _descriptor.Descriptor(
   name='GameSnapshot',
   full_name='lq.GameSnapshot',
   filename=None,
   file=DESCRIPTOR,
@@ -24737,16 +24817,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52188,
-  serialized_end=52597,
+  serialized_start=52382,
+  serialized_end=52791,
 )
 
 
 _ACTIONPROTOTYPE = _descriptor.Descriptor(
   name='ActionPrototype',
   full_name='lq.ActionPrototype',
   filename=None,
@@ -24782,16 +24862,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52599,
-  serialized_end=52658,
+  serialized_start=52793,
+  serialized_end=52852,
 )
 
 
 _GAMEDETAILRECORDS = _descriptor.Descriptor(
   name='GameDetailRecords',
   full_name='lq.GameDetailRecords',
   filename=None,
@@ -24813,16 +24893,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52660,
-  serialized_end=52696,
+  serialized_start=52854,
+  serialized_end=52890,
 )
 
 
 _OPTIONALOPERATION = _descriptor.Descriptor(
   name='OptionalOperation',
   full_name='lq.OptionalOperation',
   filename=None,
@@ -24853,28 +24933,35 @@
     _descriptor.FieldDescriptor(
       name='change_tile_states', full_name='lq.OptionalOperation.change_tile_states', index=3,
       number=4, type=5, cpp_type=1, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='gap_type', full_name='lq.OptionalOperation.gap_type', index=4,
+      number=5, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52698,
-  serialized_end=52802,
+  serialized_start=52892,
+  serialized_end=53014,
 )
 
 
 _OPTIONALOPERATIONLIST = _descriptor.Descriptor(
   name='OptionalOperationList',
   full_name='lq.OptionalOperationList',
   filename=None,
@@ -24917,16 +25004,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52804,
-  serialized_end=52926,
+  serialized_start=53016,
+  serialized_end=53138,
 )
 
 
 _LIQISUCCESS = _descriptor.Descriptor(
   name='LiQiSuccess',
   full_name='lq.LiQiSuccess',
   filename=None,
@@ -24969,16 +25056,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52928,
-  serialized_end=53004,
+  serialized_start=53140,
+  serialized_end=53216,
 )
 
 
 _FANINFO = _descriptor.Descriptor(
   name='FanInfo',
   full_name='lq.FanInfo',
   filename=None,
@@ -25014,16 +25101,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53006,
-  serialized_end=53054,
+  serialized_start=53218,
+  serialized_end=53266,
 )
 
 
 _HULEINFO = _descriptor.Descriptor(
   name='HuleInfo',
   full_name='lq.HuleInfo',
   filename=None,
@@ -25178,16 +25265,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53057,
-  serialized_end=53409,
+  serialized_start=53269,
+  serialized_end=53621,
 )
 
 
 _TINGPAIINFO = _descriptor.Descriptor(
   name='TingPaiInfo',
   full_name='lq.TingPaiInfo',
   filename=None,
@@ -25265,16 +25352,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53412,
-  serialized_end=53579,
+  serialized_start=53624,
+  serialized_end=53791,
 )
 
 
 _TINGPAIDISCARDINFO = _descriptor.Descriptor(
   name='TingPaiDiscardInfo',
   full_name='lq.TingPaiDiscardInfo',
   filename=None,
@@ -25310,16 +25397,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53581,
-  serialized_end=53665,
+  serialized_start=53793,
+  serialized_end=53877,
 )
 
 
 _GAMEEND = _descriptor.Descriptor(
   name='GameEnd',
   full_name='lq.GameEnd',
   filename=None,
@@ -25341,16 +25428,150 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53667,
-  serialized_end=53692,
+  serialized_start=53879,
+  serialized_end=53904,
+)
+
+
+_ACTIONSELECTGAP = _descriptor.Descriptor(
+  name='ActionSelectGap',
+  full_name='lq.ActionSelectGap',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gap_types', full_name='lq.ActionSelectGap.gap_types', index=0,
+      number=1, type=13, cpp_type=3, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tingpais0', full_name='lq.ActionSelectGap.tingpais0', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tingpais1', full_name='lq.ActionSelectGap.tingpais1', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='operation', full_name='lq.ActionSelectGap.operation', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=53907,
+  serialized_end=54068,
+)
+
+
+_RECORDSELECTGAP_TINGPAI = _descriptor.Descriptor(
+  name='TingPai',
+  full_name='lq.RecordSelectGap.TingPai',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='seat', full_name='lq.RecordSelectGap.TingPai.seat', index=0,
+      number=1, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tingpais1', full_name='lq.RecordSelectGap.TingPai.tingpais1', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=52320,
+  serialized_end=52379,
+)
+
+_RECORDSELECTGAP = _descriptor.Descriptor(
+  name='RecordSelectGap',
+  full_name='lq.RecordSelectGap',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gap_types', full_name='lq.RecordSelectGap.gap_types', index=0,
+      number=1, type=13, cpp_type=3, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tingpai', full_name='lq.RecordSelectGap.tingpai', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='operation', full_name='lq.RecordSelectGap.operation', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[_RECORDSELECTGAP_TINGPAI, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=54071,
+  serialized_end=54260,
 )
 
 
 _ACTIONCHANGETILE = _descriptor.Descriptor(
   name='ActionChangeTile',
   full_name='lq.ActionChangeTile',
   filename=None,
@@ -25428,16 +25649,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53695,
-  serialized_end=53960,
+  serialized_start=54263,
+  serialized_end=54528,
 )
 
 
 _RECORDCHANGETILE_TINGPAI = _descriptor.Descriptor(
   name='TingPai',
   full_name='lq.RecordChangeTile.TingPai',
   filename=None,
@@ -25466,16 +25687,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=52126,
-  serialized_end=52185,
+  serialized_start=52320,
+  serialized_end=52379,
 )
 
 _RECORDCHANGETILE_CHANGETILE = _descriptor.Descriptor(
   name='ChangeTile',
   full_name='lq.RecordChangeTile.ChangeTile',
   filename=None,
   file=DESCRIPTOR,
@@ -25517,16 +25738,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=54233,
-  serialized_end=54331,
+  serialized_start=54848,
+  serialized_end=54946,
 )
 
 _RECORDCHANGETILE = _descriptor.Descriptor(
   name='RecordChangeTile',
   full_name='lq.RecordChangeTile',
   filename=None,
   file=DESCRIPTOR,
@@ -25563,28 +25784,35 @@
     _descriptor.FieldDescriptor(
       name='change_type', full_name='lq.RecordChangeTile.change_type', index=4,
       number=5, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='operations', full_name='lq.RecordChangeTile.operations', index=5,
+      number=6, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[_RECORDCHANGETILE_TINGPAI, _RECORDCHANGETILE_CHANGETILE, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=53963,
-  serialized_end=54331,
+  serialized_start=54531,
+  serialized_end=54946,
 )
 
 
 _ACTIONDISCARDTILE = _descriptor.Descriptor(
   name='ActionDiscardTile',
   full_name='lq.ActionDiscardTile',
   filename=None,
@@ -25676,16 +25904,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=54334,
-  serialized_end=54593,
+  serialized_start=54949,
+  serialized_end=55208,
 )
 
 
 _RECORDDISCARDTILE = _descriptor.Descriptor(
   name='RecordDiscardTile',
   full_name='lq.RecordDiscardTile',
   filename=None,
@@ -25777,16 +26005,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=54596,
-  serialized_end=54856,
+  serialized_start=55211,
+  serialized_end=55471,
 )
 
 
 _ACTIONDEALTILE = _descriptor.Descriptor(
   name='ActionDealTile',
   full_name='lq.ActionDealTile',
   filename=None,
@@ -25871,16 +26099,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=54859,
-  serialized_end=55128,
+  serialized_start=55474,
+  serialized_end=55743,
 )
 
 
 _RECORDDEALTILE = _descriptor.Descriptor(
   name='RecordDealTile',
   full_name='lq.RecordDealTile',
   filename=None,
@@ -25958,16 +26186,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=55131,
-  serialized_end=55358,
+  serialized_start=55746,
+  serialized_end=55973,
 )
 
 
 _ACTIONCHIPENGGANG = _descriptor.Descriptor(
   name='ActionChiPengGang',
   full_name='lq.ActionChiPengGang',
   filename=None,
@@ -26052,16 +26280,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=55361,
-  serialized_end=55624,
+  serialized_start=55976,
+  serialized_end=56239,
 )
 
 
 _RECORDCHIPENGGANG = _descriptor.Descriptor(
   name='RecordChiPengGang',
   full_name='lq.RecordChiPengGang',
   filename=None,
@@ -26139,16 +26367,140 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=55627,
-  serialized_end=55848,
+  serialized_start=56242,
+  serialized_end=56463,
+)
+
+
+_ACTIONGANGRESULT = _descriptor.Descriptor(
+  name='ActionGangResult',
+  full_name='lq.ActionGangResult',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gang_infos', full_name='lq.ActionGangResult.gang_infos', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=56465,
+  serialized_end=56520,
+)
+
+
+_RECORDGANGRESULT = _descriptor.Descriptor(
+  name='RecordGangResult',
+  full_name='lq.RecordGangResult',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gang_infos', full_name='lq.RecordGangResult.gang_infos', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=56522,
+  serialized_end=56577,
+)
+
+
+_ACTIONGANGRESULTEND = _descriptor.Descriptor(
+  name='ActionGangResultEnd',
+  full_name='lq.ActionGangResultEnd',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gang_infos', full_name='lq.ActionGangResultEnd.gang_infos', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=56579,
+  serialized_end=56637,
+)
+
+
+_RECORDGANGRESULTEND = _descriptor.Descriptor(
+  name='RecordGangResultEnd',
+  full_name='lq.RecordGangResultEnd',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='gang_infos', full_name='lq.RecordGangResultEnd.gang_infos', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=56639,
+  serialized_end=56697,
 )
 
 
 _ACTIONANGANGADDGANG = _descriptor.Descriptor(
   name='ActionAnGangAddGang',
   full_name='lq.ActionAnGangAddGang',
   filename=None,
@@ -26219,16 +26571,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=55851,
-  serialized_end=56057,
+  serialized_start=56700,
+  serialized_end=56906,
 )
 
 
 _RECORDANGANGADDGANG = _descriptor.Descriptor(
   name='RecordAnGangAddGang',
   full_name='lq.RecordAnGangAddGang',
   filename=None,
@@ -26285,16 +26637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56060,
-  serialized_end=56214,
+  serialized_start=56909,
+  serialized_end=57063,
 )
 
 
 _ACTIONBABEI = _descriptor.Descriptor(
   name='ActionBaBei',
   full_name='lq.ActionBaBei',
   filename=None,
@@ -26365,16 +26717,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56217,
-  serialized_end=56421,
+  serialized_start=57066,
+  serialized_end=57270,
 )
 
 
 _RECORDBABEI = _descriptor.Descriptor(
   name='RecordBaBei',
   full_name='lq.RecordBaBei',
   filename=None,
@@ -26431,16 +26783,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56424,
-  serialized_end=56576,
+  serialized_start=57273,
+  serialized_end=57425,
 )
 
 
 _ACTIONHULE = _descriptor.Descriptor(
   name='ActionHule',
   full_name='lq.ActionHule',
   filename=None,
@@ -26499,28 +26851,35 @@
     _descriptor.FieldDescriptor(
       name='muyu', full_name='lq.ActionHule.muyu', index=7,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='baopai', full_name='lq.ActionHule.baopai', index=8,
+      number=9, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56579,
-  serialized_end=56773,
+  serialized_start=57428,
+  serialized_end=57638,
 )
 
 
 _RECORDHULE = _descriptor.Descriptor(
   name='RecordHule',
   full_name='lq.RecordHule',
   filename=None,
@@ -26579,28 +26938,35 @@
     _descriptor.FieldDescriptor(
       name='muyu', full_name='lq.RecordHule.muyu', index=7,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='baopai', full_name='lq.RecordHule.baopai', index=8,
+      number=9, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56776,
-  serialized_end=56970,
+  serialized_start=57641,
+  serialized_end=57851,
 )
 
 
 _HUINFOXUEZHANMID = _descriptor.Descriptor(
   name='HuInfoXueZhanMid',
   full_name='lq.HuInfoXueZhanMid',
   filename=None,
@@ -26692,16 +27058,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56973,
-  serialized_end=57171,
+  serialized_start=57854,
+  serialized_end=58052,
 )
 
 
 _ACTIONHULEXUEZHANMID = _descriptor.Descriptor(
   name='ActionHuleXueZhanMid',
   full_name='lq.ActionHuleXueZhanMid',
   filename=None,
@@ -26772,16 +27138,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=57174,
-  serialized_end=57383,
+  serialized_start=58055,
+  serialized_end=58264,
 )
 
 
 _RECORDHULEXUEZHANMID = _descriptor.Descriptor(
   name='RecordHuleXueZhanMid',
   full_name='lq.RecordHuleXueZhanMid',
   filename=None,
@@ -26852,16 +27218,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=57386,
-  serialized_end=57595,
+  serialized_start=58267,
+  serialized_end=58476,
 )
 
 
 _ACTIONHULEXUEZHANEND = _descriptor.Descriptor(
   name='ActionHuleXueZhanEnd',
   full_name='lq.ActionHuleXueZhanEnd',
   filename=None,
@@ -26939,16 +27305,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=57598,
-  serialized_end=57847,
+  serialized_start=58479,
+  serialized_end=58728,
 )
 
 
 _RECORDHULEXUEZHANEND = _descriptor.Descriptor(
   name='RecordHuleXueZhanEnd',
   full_name='lq.RecordHuleXueZhanEnd',
   filename=None,
@@ -27026,16 +27392,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=57850,
-  serialized_end=58099,
+  serialized_start=58731,
+  serialized_end=58980,
 )
 
 
 _ACTIONLIUJU = _descriptor.Descriptor(
   name='ActionLiuJu',
   full_name='lq.ActionLiuJu',
   filename=None,
@@ -27106,16 +27472,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58102,
-  serialized_end=58308,
+  serialized_start=58983,
+  serialized_end=59189,
 )
 
 
 _RECORDLIUJU = _descriptor.Descriptor(
   name='RecordLiuJu',
   full_name='lq.RecordLiuJu',
   filename=None,
@@ -27186,16 +27552,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58311,
-  serialized_end=58517,
+  serialized_start=59192,
+  serialized_end=59398,
 )
 
 
 _NOTILEPLAYERINFO = _descriptor.Descriptor(
   name='NoTilePlayerInfo',
   full_name='lq.NoTilePlayerInfo',
   filename=None,
@@ -27238,16 +27604,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58519,
-  serialized_end=58622,
+  serialized_start=59400,
+  serialized_end=59503,
 )
 
 
 _NOTILESCOREINFO = _descriptor.Descriptor(
   name='NoTileScoreInfo',
   full_name='lq.NoTileScoreInfo',
   filename=None,
@@ -27299,28 +27665,42 @@
     _descriptor.FieldDescriptor(
       name='score', full_name='lq.NoTileScoreInfo.score', index=6,
       number=7, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='taxes', full_name='lq.NoTileScoreInfo.taxes', index=7,
+      number=8, type=5, cpp_type=1, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='lines', full_name='lq.NoTileScoreInfo.lines', index=8,
+      number=9, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58625,
-  serialized_end=58756,
+  serialized_start=59506,
+  serialized_end=59667,
 )
 
 
 _ACTIONNOTILE = _descriptor.Descriptor(
   name='ActionNoTile',
   full_name='lq.ActionNoTile',
   filename=None,
@@ -27377,16 +27757,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58759,
-  serialized_end=58953,
+  serialized_start=59670,
+  serialized_end=59864,
 )
 
 
 _RECORDNOTILE = _descriptor.Descriptor(
   name='RecordNoTile',
   full_name='lq.RecordNoTile',
   filename=None,
@@ -27443,16 +27823,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=58956,
-  serialized_end=59150,
+  serialized_start=59867,
+  serialized_end=60061,
 )
 
 
 _PLAYERLEAVING = _descriptor.Descriptor(
   name='PlayerLeaving',
   full_name='lq.PlayerLeaving',
   filename=None,
@@ -27474,16 +27854,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59152,
-  serialized_end=59181,
+  serialized_start=60063,
+  serialized_end=60092,
 )
 
 
 _REQAUTHGAME = _descriptor.Descriptor(
   name='ReqAuthGame',
   full_name='lq.ReqAuthGame',
   filename=None,
@@ -27519,16 +27899,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59183,
-  serialized_end=59250,
+  serialized_start=60094,
+  serialized_end=60161,
 )
 
 
 _RESAUTHGAME = _descriptor.Descriptor(
   name='ResAuthGame',
   full_name='lq.ResAuthGame',
   filename=None,
@@ -27585,16 +27965,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59253,
-  serialized_end=59431,
+  serialized_start=60164,
+  serialized_end=60342,
 )
 
 
 _GAMERESTORE = _descriptor.Descriptor(
   name='GameRestore',
   full_name='lq.GameRestore',
   filename=None,
@@ -27651,16 +28031,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59434,
-  serialized_end=59618,
+  serialized_start=60345,
+  serialized_end=60529,
 )
 
 
 _RESENTERGAME = _descriptor.Descriptor(
   name='ResEnterGame',
   full_name='lq.ResEnterGame',
   filename=None,
@@ -27703,16 +28083,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59620,
-  serialized_end=59729,
+  serialized_start=60531,
+  serialized_end=60640,
 )
 
 
 _REQSYNCGAME = _descriptor.Descriptor(
   name='ReqSyncGame',
   full_name='lq.ReqSyncGame',
   filename=None,
@@ -27741,16 +28121,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59731,
-  serialized_end=59776,
+  serialized_start=60642,
+  serialized_end=60687,
 )
 
 
 _RESSYNCGAME = _descriptor.Descriptor(
   name='ResSyncGame',
   full_name='lq.ResSyncGame',
   filename=None,
@@ -27793,16 +28173,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59778,
-  serialized_end=59886,
+  serialized_start=60689,
+  serialized_end=60797,
 )
 
 
 _REQSELFOPERATION = _descriptor.Descriptor(
   name='ReqSelfOperation',
   full_name='lq.ReqSelfOperation',
   filename=None,
@@ -27868,28 +28248,35 @@
     _descriptor.FieldDescriptor(
       name='tile_states', full_name='lq.ReqSelfOperation.tile_states', index=8,
       number=9, type=5, cpp_type=1, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='gap_type', full_name='lq.ReqSelfOperation.gap_type', index=9,
+      number=10, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=59889,
-  serialized_end=60071,
+  serialized_start=60800,
+  serialized_end=61000,
 )
 
 
 _REQCHIPENGGANG = _descriptor.Descriptor(
   name='ReqChiPengGang',
   full_name='lq.ReqChiPengGang',
   filename=None,
@@ -27932,16 +28319,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60073,
-  serialized_end=60161,
+  serialized_start=61002,
+  serialized_end=61090,
 )
 
 
 _REQBROADCASTINGAME = _descriptor.Descriptor(
   name='ReqBroadcastInGame',
   full_name='lq.ReqBroadcastInGame',
   filename=None,
@@ -27970,16 +28357,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60163,
-  serialized_end=60221,
+  serialized_start=61092,
+  serialized_end=61150,
 )
 
 
 _REQGMCOMMANDINGAMING = _descriptor.Descriptor(
   name='ReqGMCommandInGaming',
   full_name='lq.ReqGMCommandInGaming',
   filename=None,
@@ -28001,16 +28388,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60223,
-  serialized_end=60264,
+  serialized_start=61152,
+  serialized_end=61193,
 )
 
 
 _RESGAMEPLAYERSTATE = _descriptor.Descriptor(
   name='ResGamePlayerState',
   full_name='lq.ResGamePlayerState',
   filename=None,
@@ -28039,16 +28426,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60266,
-  serialized_end=60353,
+  serialized_start=61195,
+  serialized_end=61282,
 )
 
 
 _REQVOTEGAMEEND = _descriptor.Descriptor(
   name='ReqVoteGameEnd',
   full_name='lq.ReqVoteGameEnd',
   filename=None,
@@ -28070,16 +28457,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60355,
-  serialized_end=60384,
+  serialized_start=61284,
+  serialized_end=61313,
 )
 
 
 _RESGAMEENDVOTE = _descriptor.Descriptor(
   name='ResGameEndVote',
   full_name='lq.ResGameEndVote',
   filename=None,
@@ -28115,16 +28502,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60386,
-  serialized_end=60471,
+  serialized_start=61315,
+  serialized_end=61400,
 )
 
 
 _REQAUTHOBSERVE = _descriptor.Descriptor(
   name='ReqAuthObserve',
   full_name='lq.ReqAuthObserve',
   filename=None,
@@ -28146,16 +28533,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60473,
-  serialized_end=60504,
+  serialized_start=61402,
+  serialized_end=61433,
 )
 
 
 _RESSTARTOBSERVE = _descriptor.Descriptor(
   name='ResStartObserve',
   full_name='lq.ResStartObserve',
   filename=None,
@@ -28184,16 +28571,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60506,
-  serialized_end=60592,
+  serialized_start=61435,
+  serialized_end=61521,
 )
 
 
 _NOTIFYNEWGAME = _descriptor.Descriptor(
   name='NotifyNewGame',
   full_name='lq.NotifyNewGame',
   filename=None,
@@ -28222,16 +28609,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60594,
-  serialized_end=60649,
+  serialized_start=61523,
+  serialized_end=61578,
 )
 
 
 _NOTIFYPLAYERLOADGAMEREADY = _descriptor.Descriptor(
   name='NotifyPlayerLoadGameReady',
   full_name='lq.NotifyPlayerLoadGameReady',
   filename=None,
@@ -28253,16 +28640,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60651,
-  serialized_end=60701,
+  serialized_start=61580,
+  serialized_end=61630,
 )
 
 
 _NOTIFYGAMEBROADCAST = _descriptor.Descriptor(
   name='NotifyGameBroadcast',
   full_name='lq.NotifyGameBroadcast',
   filename=None,
@@ -28291,16 +28678,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60703,
-  serialized_end=60755,
+  serialized_start=61632,
+  serialized_end=61684,
 )
 
 
 _NOTIFYGAMEENDRESULT = _descriptor.Descriptor(
   name='NotifyGameEndResult',
   full_name='lq.NotifyGameEndResult',
   filename=None,
@@ -28322,16 +28709,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60757,
-  serialized_end=60813,
+  serialized_start=61686,
+  serialized_end=61742,
 )
 
 
 _NOTIFYGAMETERMINATE = _descriptor.Descriptor(
   name='NotifyGameTerminate',
   full_name='lq.NotifyGameTerminate',
   filename=None,
@@ -28353,16 +28740,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60815,
-  serialized_end=60852,
+  serialized_start=61744,
+  serialized_end=61781,
 )
 
 
 _NOTIFYPLAYERCONNECTIONSTATE = _descriptor.Descriptor(
   name='NotifyPlayerConnectionState',
   full_name='lq.NotifyPlayerConnectionState',
   filename=None,
@@ -28391,16 +28778,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60854,
-  serialized_end=60933,
+  serialized_start=61783,
+  serialized_end=61862,
 )
 
 
 _NOTIFYACCOUNTLEVELCHANGE = _descriptor.Descriptor(
   name='NotifyAccountLevelChange',
   full_name='lq.NotifyAccountLevelChange',
   filename=None,
@@ -28436,16 +28823,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=60935,
-  serialized_end=61042,
+  serialized_start=61864,
+  serialized_end=61971,
 )
 
 
 _NOTIFYGAMEFINISHREWARD_LEVELCHANGE = _descriptor.Descriptor(
   name='LevelChange',
   full_name='lq.NotifyGameFinishReward.LevelChange',
   filename=None,
@@ -28481,16 +28868,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61342,
-  serialized_end=61436,
+  serialized_start=62271,
+  serialized_end=62365,
 )
 
 _NOTIFYGAMEFINISHREWARD_MATCHCHEST = _descriptor.Descriptor(
   name='MatchChest',
   full_name='lq.NotifyGameFinishReward.MatchChest',
   filename=None,
   file=DESCRIPTOR,
@@ -28539,16 +28926,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61438,
-  serialized_end=61551,
+  serialized_start=62367,
+  serialized_end=62480,
 )
 
 _NOTIFYGAMEFINISHREWARD_MAINCHARACTER = _descriptor.Descriptor(
   name='MainCharacter',
   full_name='lq.NotifyGameFinishReward.MainCharacter',
   filename=None,
   file=DESCRIPTOR,
@@ -28583,16 +28970,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61553,
-  serialized_end=61609,
+  serialized_start=62482,
+  serialized_end=62538,
 )
 
 _NOTIFYGAMEFINISHREWARD_CHARACTERGIFT = _descriptor.Descriptor(
   name='CharacterGift',
   full_name='lq.NotifyGameFinishReward.CharacterGift',
   filename=None,
   file=DESCRIPTOR,
@@ -28634,16 +29021,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61611,
-  serialized_end=61689,
+  serialized_start=62540,
+  serialized_end=62618,
 )
 
 _NOTIFYGAMEFINISHREWARD = _descriptor.Descriptor(
   name='NotifyGameFinishReward',
   full_name='lq.NotifyGameFinishReward',
   filename=None,
   file=DESCRIPTOR,
@@ -28692,16 +29079,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61045,
-  serialized_end=61689,
+  serialized_start=61974,
+  serialized_end=62618,
 )
 
 
 _NOTIFYACTIVITYREWARD_ACTIVITYREWARD = _descriptor.Descriptor(
   name='ActivityReward',
   full_name='lq.NotifyActivityReward.ActivityReward',
   filename=None,
@@ -28730,16 +29117,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61782,
-  serialized_end=61852,
+  serialized_start=62711,
+  serialized_end=62781,
 )
 
 _NOTIFYACTIVITYREWARD = _descriptor.Descriptor(
   name='NotifyActivityReward',
   full_name='lq.NotifyActivityReward',
   filename=None,
   file=DESCRIPTOR,
@@ -28760,16 +29147,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61692,
-  serialized_end=61852,
+  serialized_start=62621,
+  serialized_end=62781,
 )
 
 
 _NOTIFYACTIVITYPOINT_ACTIVITYPOINT = _descriptor.Descriptor(
   name='ActivityPoint',
   full_name='lq.NotifyActivityPoint.ActivityPoint',
   filename=None,
@@ -28798,16 +29185,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61942,
-  serialized_end=61993,
+  serialized_start=62871,
+  serialized_end=62922,
 )
 
 _NOTIFYACTIVITYPOINT = _descriptor.Descriptor(
   name='NotifyActivityPoint',
   full_name='lq.NotifyActivityPoint',
   filename=None,
   file=DESCRIPTOR,
@@ -28828,16 +29215,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61855,
-  serialized_end=61993,
+  serialized_start=62784,
+  serialized_end=62922,
 )
 
 
 _NOTIFYLEADERBOARDPOINT_LEADERBOARDPOINT = _descriptor.Descriptor(
   name='LeaderboardPoint',
   full_name='lq.NotifyLeaderboardPoint.LeaderboardPoint',
   filename=None,
@@ -28866,16 +29253,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=62095,
-  serialized_end=62152,
+  serialized_start=63024,
+  serialized_end=63081,
 )
 
 _NOTIFYLEADERBOARDPOINT = _descriptor.Descriptor(
   name='NotifyLeaderboardPoint',
   full_name='lq.NotifyLeaderboardPoint',
   filename=None,
   file=DESCRIPTOR,
@@ -28896,16 +29283,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=61996,
-  serialized_end=62152,
+  serialized_start=62925,
+  serialized_end=63081,
 )
 
 
 _NOTIFYGAMEPAUSE = _descriptor.Descriptor(
   name='NotifyGamePause',
   full_name='lq.NotifyGamePause',
   filename=None,
@@ -28927,16 +29314,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=62154,
-  serialized_end=62187,
+  serialized_start=63083,
+  serialized_end=63116,
 )
 
 
 _NOTIFYENDGAMEVOTE_VOTERESULT = _descriptor.Descriptor(
   name='VoteResult',
   full_name='lq.NotifyEndGameVote.VoteResult',
   filename=None,
@@ -28965,16 +29352,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=62305,
-  serialized_end=62350,
+  serialized_start=63234,
+  serialized_end=63279,
 )
 
 _NOTIFYENDGAMEVOTE = _descriptor.Descriptor(
   name='NotifyEndGameVote',
   full_name='lq.NotifyEndGameVote',
   filename=None,
   file=DESCRIPTOR,
@@ -29009,16 +29396,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=62190,
-  serialized_end=62350,
+  serialized_start=63119,
+  serialized_end=63279,
 )
 
 
 _NOTIFYOBSERVEDATA = _descriptor.Descriptor(
   name='NotifyObserveData',
   full_name='lq.NotifyObserveData',
   filename=None,
@@ -29040,16 +29427,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=62352,
-  serialized_end=62403,
+  serialized_start=63281,
+  serialized_end=63332,
 )
 
 _NOTIFYROOMPLAYERREADY_ACCOUNTREADYSTATE.containing_type = _NOTIFYROOMPLAYERREADY
 _NOTIFYROOMPLAYERREADY.fields_by_name['account_list'].message_type = _NOTIFYROOMPLAYERREADY_ACCOUNTREADYSTATE
 _NOTIFYROOMPLAYERDRESSING_ACCOUNTDRESSINGSTATE.containing_type = _NOTIFYROOMPLAYERDRESSING
 _NOTIFYROOMPLAYERDRESSING.fields_by_name['account_list'].message_type = _NOTIFYROOMPLAYERDRESSING_ACCOUNTDRESSINGSTATE
 _NOTIFYROOMPLAYERUPDATE.fields_by_name['update_list'].message_type = _PLAYERBASEVIEW
@@ -29531,14 +29918,16 @@
 _RESCHALLENGESEASONINFO.fields_by_name['challenge_season_list'].message_type = _RESCHALLENGESEASONINFO_CHALLENGEINFO
 _RESRECEIVECHALLENGERANKREWARD_REWARD.containing_type = _RESRECEIVECHALLENGERANKREWARD
 _RESRECEIVECHALLENGERANKREWARD.fields_by_name['rewards'].message_type = _RESRECEIVECHALLENGERANKREWARD_REWARD
 _RESGAMEPOINTRANK_RANKINFO.containing_type = _RESGAMEPOINTRANK
 _RESGAMEPOINTRANK.fields_by_name['error'].message_type = _ERROR
 _RESGAMEPOINTRANK.fields_by_name['rank'].message_type = _RESGAMEPOINTRANK_RANKINFO
 _RESFETCHSELFGAMEPOINTRANK.fields_by_name['error'].message_type = _ERROR
+_CHUANMAGANG.fields_by_name['gameend'].message_type = _GAMEEND
+_CHUANMAGANG.fields_by_name['hules_history'].message_type = _HULEINFO
 _ACTIONNEWROUND.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONNEWROUND.fields_by_name['tingpais0'].message_type = _TINGPAIDISCARDINFO
 _ACTIONNEWROUND.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
 _ACTIONNEWROUND.fields_by_name['opens'].message_type = _NEWROUNDOPENEDTILES
 _ACTIONNEWROUND.fields_by_name['muyu'].message_type = _MUYUINFO
 _RECORDNEWROUND_TINGPAI.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
 _RECORDNEWROUND_TINGPAI.containing_type = _RECORDNEWROUND
@@ -29550,23 +29939,31 @@
 _GAMESNAPSHOT_PLAYERSNAPSHOT_FULU.containing_type = _GAMESNAPSHOT_PLAYERSNAPSHOT
 _GAMESNAPSHOT_PLAYERSNAPSHOT.fields_by_name['mings'].message_type = _GAMESNAPSHOT_PLAYERSNAPSHOT_FULU
 _GAMESNAPSHOT_PLAYERSNAPSHOT.containing_type = _GAMESNAPSHOT
 _GAMESNAPSHOT.fields_by_name['players'].message_type = _GAMESNAPSHOT_PLAYERSNAPSHOT
 _OPTIONALOPERATIONLIST.fields_by_name['operation_list'].message_type = _OPTIONALOPERATION
 _HULEINFO.fields_by_name['fans'].message_type = _FANINFO
 _TINGPAIDISCARDINFO.fields_by_name['infos'].message_type = _TINGPAIINFO
+_ACTIONSELECTGAP.fields_by_name['tingpais0'].message_type = _TINGPAIDISCARDINFO
+_ACTIONSELECTGAP.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
+_ACTIONSELECTGAP.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
+_RECORDSELECTGAP_TINGPAI.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
+_RECORDSELECTGAP_TINGPAI.containing_type = _RECORDSELECTGAP
+_RECORDSELECTGAP.fields_by_name['tingpai'].message_type = _RECORDSELECTGAP_TINGPAI
+_RECORDSELECTGAP.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONCHANGETILE.fields_by_name['tingpais0'].message_type = _TINGPAIDISCARDINFO
 _ACTIONCHANGETILE.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
 _ACTIONCHANGETILE.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _RECORDCHANGETILE_TINGPAI.fields_by_name['tingpais1'].message_type = _TINGPAIINFO
 _RECORDCHANGETILE_TINGPAI.containing_type = _RECORDCHANGETILE
 _RECORDCHANGETILE_CHANGETILE.containing_type = _RECORDCHANGETILE
 _RECORDCHANGETILE.fields_by_name['tingpai'].message_type = _RECORDCHANGETILE_TINGPAI
 _RECORDCHANGETILE.fields_by_name['change_tile_infos'].message_type = _RECORDCHANGETILE_CHANGETILE
 _RECORDCHANGETILE.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
+_RECORDCHANGETILE.fields_by_name['operations'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONDISCARDTILE.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONDISCARDTILE.fields_by_name['tingpais'].message_type = _TINGPAIINFO
 _ACTIONDISCARDTILE.fields_by_name['muyu'].message_type = _MUYUINFO
 _RECORDDISCARDTILE.fields_by_name['tingpais'].message_type = _TINGPAIINFO
 _RECORDDISCARDTILE.fields_by_name['operations'].message_type = _OPTIONALOPERATIONLIST
 _RECORDDISCARDTILE.fields_by_name['muyu'].message_type = _MUYUINFO
 _ACTIONDEALTILE.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
@@ -29579,14 +29976,18 @@
 _ACTIONCHIPENGGANG.fields_by_name['liqi'].message_type = _LIQISUCCESS
 _ACTIONCHIPENGGANG.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONCHIPENGGANG.fields_by_name['tingpais'].message_type = _TINGPAIDISCARDINFO
 _ACTIONCHIPENGGANG.fields_by_name['muyu'].message_type = _MUYUINFO
 _RECORDCHIPENGGANG.fields_by_name['liqi'].message_type = _LIQISUCCESS
 _RECORDCHIPENGGANG.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _RECORDCHIPENGGANG.fields_by_name['muyu'].message_type = _MUYUINFO
+_ACTIONGANGRESULT.fields_by_name['gang_infos'].message_type = _CHUANMAGANG
+_RECORDGANGRESULT.fields_by_name['gang_infos'].message_type = _CHUANMAGANG
+_ACTIONGANGRESULTEND.fields_by_name['gang_infos'].message_type = _CHUANMAGANG
+_RECORDGANGRESULTEND.fields_by_name['gang_infos'].message_type = _CHUANMAGANG
 _ACTIONANGANGADDGANG.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONANGANGADDGANG.fields_by_name['tingpais'].message_type = _TINGPAIINFO
 _ACTIONANGANGADDGANG.fields_by_name['muyu'].message_type = _MUYUINFO
 _RECORDANGANGADDGANG.fields_by_name['operations'].message_type = _OPTIONALOPERATIONLIST
 _RECORDANGANGADDGANG.fields_by_name['muyu'].message_type = _MUYUINFO
 _ACTIONBABEI.fields_by_name['operation'].message_type = _OPTIONALOPERATIONLIST
 _ACTIONBABEI.fields_by_name['tingpais'].message_type = _TINGPAIINFO
@@ -30118,35 +30519,42 @@
 DESCRIPTOR.message_types_by_name['ReqBuyInABMatch'] = _REQBUYINABMATCH
 DESCRIPTOR.message_types_by_name['ReqGamePointRank'] = _REQGAMEPOINTRANK
 DESCRIPTOR.message_types_by_name['ResGamePointRank'] = _RESGAMEPOINTRANK
 DESCRIPTOR.message_types_by_name['ResFetchSelfGamePointRank'] = _RESFETCHSELFGAMEPOINTRANK
 DESCRIPTOR.message_types_by_name['ActionMJStart'] = _ACTIONMJSTART
 DESCRIPTOR.message_types_by_name['NewRoundOpenedTiles'] = _NEWROUNDOPENEDTILES
 DESCRIPTOR.message_types_by_name['MuyuInfo'] = _MUYUINFO
+DESCRIPTOR.message_types_by_name['ChuanmaGang'] = _CHUANMAGANG
 DESCRIPTOR.message_types_by_name['ActionNewRound'] = _ACTIONNEWROUND
 DESCRIPTOR.message_types_by_name['RecordNewRound'] = _RECORDNEWROUND
 DESCRIPTOR.message_types_by_name['GameSnapshot'] = _GAMESNAPSHOT
 DESCRIPTOR.message_types_by_name['ActionPrototype'] = _ACTIONPROTOTYPE
 DESCRIPTOR.message_types_by_name['GameDetailRecords'] = _GAMEDETAILRECORDS
 DESCRIPTOR.message_types_by_name['OptionalOperation'] = _OPTIONALOPERATION
 DESCRIPTOR.message_types_by_name['OptionalOperationList'] = _OPTIONALOPERATIONLIST
 DESCRIPTOR.message_types_by_name['LiQiSuccess'] = _LIQISUCCESS
 DESCRIPTOR.message_types_by_name['FanInfo'] = _FANINFO
 DESCRIPTOR.message_types_by_name['HuleInfo'] = _HULEINFO
 DESCRIPTOR.message_types_by_name['TingPaiInfo'] = _TINGPAIINFO
 DESCRIPTOR.message_types_by_name['TingPaiDiscardInfo'] = _TINGPAIDISCARDINFO
 DESCRIPTOR.message_types_by_name['GameEnd'] = _GAMEEND
+DESCRIPTOR.message_types_by_name['ActionSelectGap'] = _ACTIONSELECTGAP
+DESCRIPTOR.message_types_by_name['RecordSelectGap'] = _RECORDSELECTGAP
 DESCRIPTOR.message_types_by_name['ActionChangeTile'] = _ACTIONCHANGETILE
 DESCRIPTOR.message_types_by_name['RecordChangeTile'] = _RECORDCHANGETILE
 DESCRIPTOR.message_types_by_name['ActionDiscardTile'] = _ACTIONDISCARDTILE
 DESCRIPTOR.message_types_by_name['RecordDiscardTile'] = _RECORDDISCARDTILE
 DESCRIPTOR.message_types_by_name['ActionDealTile'] = _ACTIONDEALTILE
 DESCRIPTOR.message_types_by_name['RecordDealTile'] = _RECORDDEALTILE
 DESCRIPTOR.message_types_by_name['ActionChiPengGang'] = _ACTIONCHIPENGGANG
 DESCRIPTOR.message_types_by_name['RecordChiPengGang'] = _RECORDCHIPENGGANG
+DESCRIPTOR.message_types_by_name['ActionGangResult'] = _ACTIONGANGRESULT
+DESCRIPTOR.message_types_by_name['RecordGangResult'] = _RECORDGANGRESULT
+DESCRIPTOR.message_types_by_name['ActionGangResultEnd'] = _ACTIONGANGRESULTEND
+DESCRIPTOR.message_types_by_name['RecordGangResultEnd'] = _RECORDGANGRESULTEND
 DESCRIPTOR.message_types_by_name['ActionAnGangAddGang'] = _ACTIONANGANGADDGANG
 DESCRIPTOR.message_types_by_name['RecordAnGangAddGang'] = _RECORDANGANGADDGANG
 DESCRIPTOR.message_types_by_name['ActionBaBei'] = _ACTIONBABEI
 DESCRIPTOR.message_types_by_name['RecordBaBei'] = _RECORDBABEI
 DESCRIPTOR.message_types_by_name['ActionHule'] = _ACTIONHULE
 DESCRIPTOR.message_types_by_name['RecordHule'] = _RECORDHULE
 DESCRIPTOR.message_types_by_name['HuInfoXueZhanMid'] = _HUINFOXUEZHANMID
@@ -33985,14 +34393,21 @@
 MuyuInfo = _reflection.GeneratedProtocolMessageType('MuyuInfo', (_message.Message,), dict(
   DESCRIPTOR = _MUYUINFO,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.MuyuInfo)
   ))
 _sym_db.RegisterMessage(MuyuInfo)
 
+ChuanmaGang = _reflection.GeneratedProtocolMessageType('ChuanmaGang', (_message.Message,), dict(
+  DESCRIPTOR = _CHUANMAGANG,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.ChuanmaGang)
+  ))
+_sym_db.RegisterMessage(ChuanmaGang)
+
 ActionNewRound = _reflection.GeneratedProtocolMessageType('ActionNewRound', (_message.Message,), dict(
   DESCRIPTOR = _ACTIONNEWROUND,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.ActionNewRound)
   ))
 _sym_db.RegisterMessage(ActionNewRound)
 
@@ -34100,14 +34515,36 @@
 GameEnd = _reflection.GeneratedProtocolMessageType('GameEnd', (_message.Message,), dict(
   DESCRIPTOR = _GAMEEND,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.GameEnd)
   ))
 _sym_db.RegisterMessage(GameEnd)
 
+ActionSelectGap = _reflection.GeneratedProtocolMessageType('ActionSelectGap', (_message.Message,), dict(
+  DESCRIPTOR = _ACTIONSELECTGAP,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.ActionSelectGap)
+  ))
+_sym_db.RegisterMessage(ActionSelectGap)
+
+RecordSelectGap = _reflection.GeneratedProtocolMessageType('RecordSelectGap', (_message.Message,), dict(
+
+  TingPai = _reflection.GeneratedProtocolMessageType('TingPai', (_message.Message,), dict(
+    DESCRIPTOR = _RECORDSELECTGAP_TINGPAI,
+    __module__ = 'protocol_pb2'
+    # @@protoc_insertion_point(class_scope:lq.RecordSelectGap.TingPai)
+    ))
+  ,
+  DESCRIPTOR = _RECORDSELECTGAP,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.RecordSelectGap)
+  ))
+_sym_db.RegisterMessage(RecordSelectGap)
+_sym_db.RegisterMessage(RecordSelectGap.TingPai)
+
 ActionChangeTile = _reflection.GeneratedProtocolMessageType('ActionChangeTile', (_message.Message,), dict(
   DESCRIPTOR = _ACTIONCHANGETILE,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.ActionChangeTile)
   ))
 _sym_db.RegisterMessage(ActionChangeTile)
 
@@ -34172,14 +34609,42 @@
 RecordChiPengGang = _reflection.GeneratedProtocolMessageType('RecordChiPengGang', (_message.Message,), dict(
   DESCRIPTOR = _RECORDCHIPENGGANG,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.RecordChiPengGang)
   ))
 _sym_db.RegisterMessage(RecordChiPengGang)
 
+ActionGangResult = _reflection.GeneratedProtocolMessageType('ActionGangResult', (_message.Message,), dict(
+  DESCRIPTOR = _ACTIONGANGRESULT,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.ActionGangResult)
+  ))
+_sym_db.RegisterMessage(ActionGangResult)
+
+RecordGangResult = _reflection.GeneratedProtocolMessageType('RecordGangResult', (_message.Message,), dict(
+  DESCRIPTOR = _RECORDGANGRESULT,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.RecordGangResult)
+  ))
+_sym_db.RegisterMessage(RecordGangResult)
+
+ActionGangResultEnd = _reflection.GeneratedProtocolMessageType('ActionGangResultEnd', (_message.Message,), dict(
+  DESCRIPTOR = _ACTIONGANGRESULTEND,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.ActionGangResultEnd)
+  ))
+_sym_db.RegisterMessage(ActionGangResultEnd)
+
+RecordGangResultEnd = _reflection.GeneratedProtocolMessageType('RecordGangResultEnd', (_message.Message,), dict(
+  DESCRIPTOR = _RECORDGANGRESULTEND,
+  __module__ = 'protocol_pb2'
+  # @@protoc_insertion_point(class_scope:lq.RecordGangResultEnd)
+  ))
+_sym_db.RegisterMessage(RecordGangResultEnd)
+
 ActionAnGangAddGang = _reflection.GeneratedProtocolMessageType('ActionAnGangAddGang', (_message.Message,), dict(
   DESCRIPTOR = _ACTIONANGANGADDGANG,
   __module__ = 'protocol_pb2'
   # @@protoc_insertion_point(class_scope:lq.ActionAnGangAddGang)
   ))
 _sym_db.RegisterMessage(ActionAnGangAddGang)
 
@@ -34573,16 +35038,16 @@
 
 _LOBBY = _descriptor.ServiceDescriptor(
   name='Lobby',
   full_name='lq.Lobby',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=62469,
-  serialized_end=77913,
+  serialized_start=63398,
+  serialized_end=78842,
   methods=[
   _descriptor.MethodDescriptor(
     name='fetchConnectionInfo',
     full_name='lq.Lobby.fetchConnectionInfo',
     index=0,
     containing_service=None,
     input_type=_REQCOMMON,
@@ -36676,16 +37141,16 @@
 
 _FASTTEST = _descriptor.ServiceDescriptor(
   name='FastTest',
   full_name='lq.FastTest',
   file=DESCRIPTOR,
   index=1,
   serialized_options=None,
-  serialized_start=77916,
-  serialized_end=78801,
+  serialized_start=78845,
+  serialized_end=79730,
   methods=[
   _descriptor.MethodDescriptor(
     name='authGame',
     full_name='lq.FastTest.authGame',
     index=0,
     containing_service=None,
     input_type=_REQAUTHGAME,
```

### Comparing `ms_api-0.9.59/ms/rpc.py` & `ms_api-0.9.70/ms/rpc.py`

 * *Files identical despite different names*

### Comparing `ms_api-0.9.59/ms_api.egg-info/PKG-INFO` & `ms_api-0.9.70/ms_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ms-api
-Version: 0.9.59
+Version: 0.9.70
 Summary: Python wrapper for the Mahjong Soul (Majsoul) Protobuf objects. It allows to use their API.
 Home-page: https://github.com/MahjongRepository/mahjong_soul_api
 Author: Nihisil
 Author-email: alexey@nihisil.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ms_api-0.9.59/setup.py` & `ms_api-0.9.70/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name='ms_api',
     packages=[
         'ms',
     ],
-    version='0.9.59',
+    version='0.9.70',
     description='Python wrapper for the Mahjong Soul (Majsoul) Protobuf objects. It allows to use their API.',
     long_description='',
     author='Nihisil',
     author_email='alexey@nihisil.com',
     url='https://github.com/MahjongRepository/mahjong_soul_api',
     install_requires=requirements,
     classifiers=[
```

