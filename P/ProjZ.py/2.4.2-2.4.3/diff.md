# Comparing `tmp/ProjZ.py-2.4.2.tar.gz` & `tmp/ProjZ.py-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.4.2.tar", last modified: Sat Apr 29 17:20:23 2023, max compression
+gzip compressed data, was "ProjZ.py-2.4.3.tar", last modified: Sat Apr 29 22:44:41 2023, max compression
```

## Comparing `ProjZ.py-2.4.2.tar` & `ProjZ.py-2.4.3.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.970257 ProjZ.py-2.4.2/
--rw-rw-rw-   0        0        0     4049 2023-04-29 17:20:23.971254 ProjZ.py-2.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.758002 ProjZ.py-2.4.2/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     4049 2023-04-29 17:20:23.000000 ProjZ.py-2.4.2/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2284 2023-04-29 17:20:23.000000 ProjZ.py-2.4.2/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:20:23.000000 ProjZ.py-2.4.2/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-29 17:20:23.000000 ProjZ.py-2.4.2/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 17:20:23.000000 ProjZ.py-2.4.2/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3640 2023-04-29 17:20:16.000000 ProjZ.py-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.768555 ProjZ.py-2.4.2/projz/
--rw-rw-rw-   0        0        0      112 2023-04-29 15:41:29.000000 ProjZ.py-2.4.2/projz/__init__.py
--rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.772547 ProjZ.py-2.4.2/projz/api/
--rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.779529 ProjZ.py-2.4.2/projz/api/control/
--rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/control/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/control/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.787508 ProjZ.py-2.4.2/projz/api/headers/
--rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/headers/__init__.py
--rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.2/projz/api/headers/abc_headers_provider.py
--rw-rw-rw-   0        0        0     2334 2023-04-29 15:38:12.000000 ProjZ.py-2.4.2/projz/api/headers/headers_provider.py
--rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/request_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.791496 ProjZ.py-2.4.2/projz/api/secret/
--rw-rw-rw-   0        0        0      661 2023-04-29 17:19:39.000000 ProjZ.py-2.4.2/projz/api/secret/__init__.py
--rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.2/projz/api/secret/data.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.801470 ProjZ.py-2.4.2/projz/api/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/util/__init__.py
--rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/api/util/copy_to_buffer_writer.py
--rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/client.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.851461 ProjZ.py-2.4.2/projz/enum/
--rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/__init__.py
--rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/auth_purpose.py
--rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/auth_type.py
--rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/chat_message_type.py
--rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/chat_query_type.py
--rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/chat_thread_type.py
--rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/circle_filter_type.py
--rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/circle_members_query_type.py
--rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/comment_type.py
--rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/content_region.py
--rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/currency_type.py
--rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/gender.py
--rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/object_type.py
--rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/party_query_type.py
--rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/upload_target.py
--rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/user_task_type.py
--rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/enum/ws_event_type.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.855102 ProjZ.py-2.4.2/projz/error/
--rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/error/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/error/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.931511 ProjZ.py-2.4.2/projz/model/
--rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/__init__.py
--rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/account.py
--rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/blocked_item_wrapper.py
--rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/blog.py
--rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/category.py
--rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/chat.py
--rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/chat_message.py
--rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/circle.py
--rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/comment.py
--rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/currency.py
--rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/default_background_media.py
--rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/dice.py
--rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/gift_box.py
--rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/link_info.py
--rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/media.py
--rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/member_title.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.936473 ProjZ.py-2.4.2/projz/model/parse/
--rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/parse/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/parse/parseutils.py
--rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/party.py
--rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/poll.py
--rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/qi_vote_full_info.py
--rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/qi_vote_info.py
--rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.946580 ProjZ.py-2.4.2/projz/model/response/
--rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/response/__init__.py
--rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/response/auth_result.py
--rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/response/member_titles_info.py
--rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/response/multi_invitation_code_info.py
--rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/rich_format.py
--rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/sticker.py
--rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/transfer_order.py
--rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/user.py
--rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/user_task.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.958310 ProjZ.py-2.4.2/projz/model/util/
--rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/util/__init__.py
--rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/util/paginated_list.py
--rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/util/rich_format_builder.py
--rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/util/rich_format_text_builder.py
--rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/model/wallet.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.962274 ProjZ.py-2.4.2/projz/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/util/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/util/subscription_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:20:23.967258 ProjZ.py-2.4.2/projz/websocket/
--rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/websocket/__init__.py
--rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.2/projz/websocket/websocket_listener.py
--rw-rw-rw-   0        0        0       42 2023-04-29 17:20:23.974073 ProjZ.py-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1929 2023-04-29 17:20:16.000000 ProjZ.py-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:41.002530 ProjZ.py-2.4.3/
+-rw-rw-rw-   0        0        0     4049 2023-04-29 22:44:41.002530 ProjZ.py-2.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.211450 ProjZ.py-2.4.3/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     4049 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2325 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3640 2023-04-29 17:20:16.000000 ProjZ.py-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.239629 ProjZ.py-2.4.3/projz/
+-rw-rw-rw-   0        0        0      112 2023-04-29 17:24:41.000000 ProjZ.py-2.4.3/projz/__init__.py
+-rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.251616 ProjZ.py-2.4.3/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.274564 ProjZ.py-2.4.3/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.306444 ProjZ.py-2.4.3/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.3/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2334 2023-04-29 15:38:12.000000 ProjZ.py-2.4.3/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-29 20:52:00.000000 ProjZ.py-2.4.3/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.318419 ProjZ.py-2.4.3/projz/api/secret/
+-rw-rw-rw-   0        0        0      661 2023-04-29 17:19:39.000000 ProjZ.py-2.4.3/projz/api/secret/__init__.py
+-rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.3/projz/api/secret/data.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.339165 ProjZ.py-2.4.3/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    58016 2023-04-29 22:00:27.000000 ProjZ.py-2.4.3/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.510447 ProjZ.py-2.4.3/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      165 2023-04-29 20:27:50.000000 ProjZ.py-2.4.3/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.539845 ProjZ.py-2.4.3/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.817526 ProjZ.py-2.4.3/projz/model/
+-rw-rw-rw-   0        0        0     1140 2023-04-29 21:59:15.000000 ProjZ.py-2.4.3/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.864850 ProjZ.py-2.4.3/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.904379 ProjZ.py-2.4.3/projz/model/response/
+-rw-rw-rw-   0        0        0      198 2023-04-29 21:59:15.000000 ProjZ.py-2.4.3/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      363 2023-04-29 21:58:26.000000 ProjZ.py-2.4.3/projz/model/response/block_users_info.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.951558 ProjZ.py-2.4.3/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4388 2023-04-29 17:46:35.000000 ProjZ.py-2.4.3/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.973505 ProjZ.py-2.4.3/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.997555 ProjZ.py-2.4.3/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:44:41.005523 ProjZ.py-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1929 2023-04-29 22:44:20.000000 ProjZ.py-2.4.3/setup.py
```

### Comparing `ProjZ.py-2.4.2/PKG-INFO` & `ProjZ.py-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.2
+Version: 2.4.3
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4rkwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.4.2/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.4.3/ProjZ.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.2
+Version: 2.4.3
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4rkwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.4.2/ProjZ.py.egg-info/SOURCES.txt` & `ProjZ.py-2.4.3/ProjZ.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 projz/model/user.py
 projz/model/user_task.py
 projz/model/wallet.py
 projz/model/parse/__init__.py
 projz/model/parse/parseutils.py
 projz/model/response/__init__.py
 projz/model/response/auth_result.py
+projz/model/response/block_users_info.py
 projz/model/response/member_titles_info.py
 projz/model/response/multi_invitation_code_info.py
 projz/model/util/__init__.py
 projz/model/util/paginated_list.py
 projz/model/util/rich_format_builder.py
 projz/model/util/rich_format_text_builder.py
 projz/util/__init__.py
```

### Comparing `ProjZ.py-2.4.2/README.md` & `ProjZ.py-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/__main__.py` & `ProjZ.py-2.4.3/projz/__main__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/control/rpc.py` & `ProjZ.py-2.4.3/projz/api/control/rpc.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/headers/abc_headers_provider.py` & `ProjZ.py-2.4.3/projz/api/headers/abc_headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/headers/headers_provider.py` & `ProjZ.py-2.4.3/projz/api/headers/headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/request_manager.py` & `ProjZ.py-2.4.3/projz/api/request_manager.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/secret/__init__.py` & `ProjZ.py-2.4.3/projz/api/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/api/secret/data.txt` & `ProjZ.py-2.4.3/projz/api/secret/data.txt`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/client.py` & `ProjZ.py-2.4.3/projz/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,47 +380,63 @@
                            message_type: Union[ChatMessageType, int] = 1,
                            content: Optional[str] = None,
                            reply_to: Optional[int] = None,
                            message_rich_format: Optional[RichFormat] = None,
                            attached_media: Optional[Media] = None,
                            attached_audio: Optional[Media] = None,
                            poll_id: Optional[int] = None,
-                           dice_id: Optional[int] = None) -> ChatMessage:
+                           dice_id: Optional[int] = None,
+                           *,
+                           get_sent_message: bool = True) -> Optional[ChatMessage]:
         """
         Send message to the chat
         :param thread_id: id of the chat
         :param message_type: ChatMessageType enum field or int identifier
         :param content: text content of the message
         :param reply_to: reply message id
         :param message_rich_format: RichFormat object, can be created by RichFormatBuilder
         :param attached_media: attached to the message file model.Media object
         :param attached_audio: attached to the message audio model.Media object
         :param poll_id: attached to the message poll id
         :param dice_id: attached to the message dice id
+        :param get_sent_message: If set to False, the request for information about the
+        sent message will not be executed and the function will return None.
         :return:
         """
         if attached_media is not None and attached_audio is not None:
             raise ValueError("You can't send audio and media in one message")
         seq_id = randint(0, maxsize)
         data = {
             "type": message_type if isinstance(message_type, int) else message_type.value,
             "threadId": thread_id,
             "uid": self.user_profile.uid,
             "seqId": seq_id,
             "extensions": {}
         }
         if content is not None: data["content"] = content
-        if reply_to is not None: data["extensions"]["replyMessage"] = reply_to
+        if reply_to is not None: data["extensions"]["replyMessageId"] = reply_to
         if message_rich_format is not None: data["richFormat"] = message_rich_format.to_dict()
         if attached_media is not None: data["media"] = attached_media.to_dict()
         if attached_audio is not None: data["media"] = attached_audio.to_dict()
         if poll_id is not None: data["extensions"]["pollId"] = poll_id
         if dice_id is not None: data["extensions"]["diceId"] = dice_id
         resp = await self.websocket.send_request(1, True, seq_id, **dict(threadId=thread_id, msg=data))
-        return await self.get_chat_message(resp["threadId"], resp["messageId"])
+        if get_sent_message:
+            return await self.get_chat_message(resp["threadId"], resp["messageId"])
+
+    async def show_typing(self, thread_id: int) -> None:
+        """
+        Displays the text to the chat members that the account is "typing".
+        :param thread_id: id of the chat
+        :return:
+        """
+        await self.send_message(thread_id, ChatMessageType.TYPING, get_sent_message=False)
+
+    async def get_block_users_info(self) -> BlockUsersInfo:
+        return BlockUsersInfo.from_dict(await self.get("/v1/users/block-uids"))
 
     async def get_link_info(self, link: str) -> LinkInfo:
         """
         Get object info by link
         :param link: object link
         :return: model.LinkInfo
         """
```

### Comparing `ProjZ.py-2.4.2/projz/enum/__init__.py` & `ProjZ.py-2.4.3/projz/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/error/classes.py` & `ProjZ.py-2.4.3/projz/error/classes.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/__init__.py` & `ProjZ.py-2.4.3/projz/model/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .response import AuthResult
+from .response import MemberTitlesInfo
 from .response import MultiInvitationCodeInfo
+from .response import BlockUsersInfo
 from .util import PaginatedList
 from .util import RichFormatBuilder
 from .util import RichFormatTextBuilder
 from .media import Media
 from .account import Account
 from .user import User
 from .link_info import LinkInfo
@@ -17,15 +19,14 @@
 from .chat_message import ChatMessage
 from .poll import Poll
 from .dice import Dice
 from .rich_format import RichFormat
 from .qi_vote_info import QiVoteInfo
 from .qi_vote_full_info import QiVoteFullInfo
 from .member_title import MemberTitle
-from .response import MemberTitlesInfo
 from .comment import Comment
 from .currency import Currency
 from .user_task import UserTask
 from .wallet import Wallet
 from .gift_box import GiftBox
 from .transfer_order import TransferOrder
 from .party import Party
```

### Comparing `ProjZ.py-2.4.2/projz/model/account.py` & `ProjZ.py-2.4.3/projz/model/account.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/blocked_item_wrapper.py` & `ProjZ.py-2.4.3/projz/model/blocked_item_wrapper.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/blog.py` & `ProjZ.py-2.4.3/projz/model/blog.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/category.py` & `ProjZ.py-2.4.3/projz/model/category.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/chat.py` & `ProjZ.py-2.4.3/projz/model/chat.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/chat_message.py` & `ProjZ.py-2.4.3/projz/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/circle.py` & `ProjZ.py-2.4.3/projz/model/circle.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/comment.py` & `ProjZ.py-2.4.3/projz/model/comment.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/currency.py` & `ProjZ.py-2.4.3/projz/model/currency.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/default_background_media.py` & `ProjZ.py-2.4.3/projz/model/default_background_media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/gift_box.py` & `ProjZ.py-2.4.3/projz/model/gift_box.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/media.py` & `ProjZ.py-2.4.3/projz/model/media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/member_title.py` & `ProjZ.py-2.4.3/projz/model/member_title.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/parse/parseutils.py` & `ProjZ.py-2.4.3/projz/model/parse/parseutils.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/poll.py` & `ProjZ.py-2.4.3/projz/model/poll.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/qi_vote_full_info.py` & `ProjZ.py-2.4.3/projz/model/qi_vote_full_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/qi_vote_info.py` & `ProjZ.py-2.4.3/projz/model/qi_vote_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/reaction.py` & `ProjZ.py-2.4.3/projz/model/reaction.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/response/member_titles_info.py` & `ProjZ.py-2.4.3/projz/model/response/member_titles_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/response/multi_invitation_code_info.py` & `ProjZ.py-2.4.3/projz/model/response/multi_invitation_code_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/rich_format.py` & `ProjZ.py-2.4.3/projz/model/rich_format.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/transfer_order.py` & `ProjZ.py-2.4.3/projz/model/transfer_order.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/user.py` & `ProjZ.py-2.4.3/projz/model/user.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/user_task.py` & `ProjZ.py-2.4.3/projz/model/user_task.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/util/rich_format_builder.py` & `ProjZ.py-2.4.3/projz/model/util/rich_format_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,23 @@
     ) -> "RichFormatBuilder":
         self._fmt.text_spans.append(RichFormat.TextSpan(start, end, RichFormat.TextSpan.Data(
             bold, italic, strikethrough, underline, foreground, background
         )))
         return self
 
     def paragraph_span(self, start: int, end: int, style: Optional[str] = None, alignment: Optional[str] = None) -> "RichFormatBuilder":
-        self._fmt.paragraph_spans.append(RichFormat.ParagraphSpan(start, end, RichFormat.ParagraphSpan.Data(style, alignment)))
+        self._fmt.paragraph_spans.append(
+            RichFormat.ParagraphSpan(start, end, RichFormat.ParagraphSpan.Data(style, alignment))
+        )
+        return self
+
+    def attachment_span(self, start: int, end: int, data: RichFormat.AttachmentSpan.Data) -> "RichFormatBuilder":
+        self._fmt.attachment_spans.append(
+            RichFormat.AttachmentSpan(start, end, data)
+        )
         return self
 
     def bold(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end, bold=True)
 
     def italic(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end, italic=True)
 
     def strikethrough(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end,strikethrough=True)
@@ -57,38 +65,34 @@
         self,
         start: int,
         url: str,
         custom_title: str = "",
         title: str = "",
         media_id: int = 0
     ) -> "RichFormatBuilder":
-        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
+        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="link",
             link=RichFormat.AttachmentSpan.Data.Link(url, custom_title, title, media_id, str(uuid4()))
-        )))
-        return self
+        ))
 
     def mention(self, start: int, username: str, uid: int, role_id: int = 0,
                 role_name_length: int = 0) -> "RichFormatBuilder":
         end = len(f"@{username}" if not username.startswith("@") else username)
-        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, end, RichFormat.AttachmentSpan.Data(
+        return self.attachment_span(start, end, RichFormat.AttachmentSpan.Data(
             type="mention",
             mention=RichFormat.AttachmentSpan.Data.Mention(uid, role_id, role_name_length)
-        )))
-        return self
+        ))
 
     def poll(self, start: int, poll_id: int) -> "RichFormatBuilder":
-        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
+        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="poll",
             poll=RichFormat.AttachmentSpan.Data.Poll(poll_id)
-        )))
-        return self
+        ))
 
     def media(self, start: int, media_id: int) -> "RichFormatBuilder":
-        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
+        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="media",
             media=RichFormat.AttachmentSpan.Data.Media(media_id)
-        )))
-        return self
+        ))
 
     def build(self) -> RichFormat:
         return self._fmt
```

### Comparing `ProjZ.py-2.4.2/projz/model/util/rich_format_text_builder.py` & `ProjZ.py-2.4.3/projz/model/util/rich_format_text_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/model/wallet.py` & `ProjZ.py-2.4.3/projz/model/wallet.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/util/subscription_handler.py` & `ProjZ.py-2.4.3/projz/util/subscription_handler.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/projz/websocket/websocket_listener.py` & `ProjZ.py-2.4.3/projz/websocket/websocket_listener.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.2/setup.py` & `ProjZ.py-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             else:
                 print("Failed to install Sox. The stability of the library is not guaranteed.")
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.4.2",
+        version="2.4.3",
         author="D4rkwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
```

