# Comparing `tmp/PyroFork-dev-2.1.5.dev202304141749.tar.gz` & `tmp/PyroFork-dev-2.1.5a1.dev202304141812.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-dev-2.1.5.dev202304141749.tar", last modified: Fri Apr 14 17:50:00 2023, max compression
+gzip compressed data, was "PyroFork-dev-2.1.5a1.dev202304141812.tar", last modified: Fri Apr 14 18:12:51 2023, max compression
```

## Comparing `PyroFork-dev-2.1.5.dev202304141749.tar` & `PyroFork-dev-2.1.5a1.dev202304141812.tar`

### file list

```diff
@@ -1,522 +1,527 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-14 17:50:00.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-04-14 17:50:00.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:50:00.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:49:59.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 17:50:00.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 17:50:00.000000 PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   166709 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.203165 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.207165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 17:49:53.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40417 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.207165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.207165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.207165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.207165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.211165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.211165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.211165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.211165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.211165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.215165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.215165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.223165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.223165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.223165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.227165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.231165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.231165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.231165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.235165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.235165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.235165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.235165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.235165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.239165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.243165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.247165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.247165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.247165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.251165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153174 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 17:49:53.000000 PyroFork-dev-2.1.5.dev202304141749/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:00.255165 PyroFork-dev-2.1.5.dev202304141749/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-14 17:49:45.000000 PyroFork-dev-2.1.5.dev202304141749/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:12:51.000000 PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   166709 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.570810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.574810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.574810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.578810 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.578810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 18:12:42.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41625 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.582810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.582810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.582810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.582810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.586810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.590810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.590810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/conversation_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.594810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.594810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.606810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.610810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.622810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.622810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.626810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.630810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.646810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/wait_for_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/wait_for_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.646810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.646810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.650810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.650810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/nav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.654810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.654810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.654810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.658810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.658810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.658810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.658810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.658810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.662810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.670810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.678810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.678810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.682810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.686810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156883 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 18:12:42.000000 PyroFork-dev-2.1.5a1.dev202304141812/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:12:51.698810 PyroFork-dev-2.1.5a1.dev202304141812/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-14 18:12:32.000000 PyroFork-dev-2.1.5a1.dev202304141812/tests/test_file_id.py
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/COPYING` & `PyroFork-dev-2.1.5a1.dev202304141812/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/COPYING.lesser` & `PyroFork-dev-2.1.5a1.dev202304141812/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/NOTICE` & `PyroFork-dev-2.1.5a1.dev202304141812/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/PKG-INFO` & `PyroFork-dev-2.1.5a1.dev202304141812/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.1.5.dev202304141749
+Version: 2.1.5a1.dev202304141812
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.1.5.dev202304141749
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.1.5a1.dev202304141812
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/PKG-INFO` & `PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.1.5.dev202304141749
+Version: 2.1.5a1.dev202304141812
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.1.5.dev202304141749
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.1.5a1.dev202304141812
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/PyroFork_dev.egg-info/SOURCES.txt` & `PyroFork-dev-2.1.5a1.dev202304141812/PyroFork_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 compiler/errors/template/sub_class.txt
 pyrogram/__init__.py
 pyrogram/client.py
 pyrogram/dispatcher.py
 pyrogram/emoji.py
 pyrogram/file_id.py
 pyrogram/filters.py
+pyrogram/helpers.py
 pyrogram/mime_types.py
+pyrogram/nav.py
 pyrogram/py.typed
 pyrogram/sync.py
 pyrogram/utils.py
 pyrogram/connection/__init__.py
 pyrogram/connection/connection.py
 pyrogram/connection/transport/__init__.py
 pyrogram/connection/transport/tcp/__init__.py
@@ -80,14 +82,15 @@
 pyrogram/errors/__init__.py
 pyrogram/errors/rpc_error.py
 pyrogram/handlers/__init__.py
 pyrogram/handlers/callback_query_handler.py
 pyrogram/handlers/chat_join_request_handler.py
 pyrogram/handlers/chat_member_updated_handler.py
 pyrogram/handlers/chosen_inline_result_handler.py
+pyrogram/handlers/conversation_handler.py
 pyrogram/handlers/deleted_messages_handler.py
 pyrogram/handlers/disconnect_handler.py
 pyrogram/handlers/edited_message_handler.py
 pyrogram/handlers/handler.py
 pyrogram/handlers/inline_query_handler.py
 pyrogram/handlers/message_handler.py
 pyrogram/handlers/poll_handler.py
@@ -266,14 +269,16 @@
 pyrogram/methods/messages/send_venue.py
 pyrogram/methods/messages/send_video.py
 pyrogram/methods/messages/send_video_note.py
 pyrogram/methods/messages/send_voice.py
 pyrogram/methods/messages/stop_poll.py
 pyrogram/methods/messages/stream_media.py
 pyrogram/methods/messages/vote_poll.py
+pyrogram/methods/messages/wait_for_callback_query.py
+pyrogram/methods/messages/wait_for_message.py
 pyrogram/methods/password/__init__.py
 pyrogram/methods/password/change_cloud_password.py
 pyrogram/methods/password/enable_cloud_password.py
 pyrogram/methods/password/remove_cloud_password.py
 pyrogram/methods/stickers/__init__.py
 pyrogram/methods/stickers/add_sticker_to_set.py
 pyrogram/methods/stickers/create_sticker_set.py
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/README.md` & `PyroFork-dev-2.1.5a1.dev202304141812/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/compiler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/auth_key.tl` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/main_api.tl` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/source/sys_msgs.tl` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/template/combinator.txt` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/api/template/type.txt` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/docs/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/docs/compiler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/compiler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/sort.py` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-dev-2.1.5a1.dev202304141812/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork-dev"
-__version__ = "2.1.5.dev202304141749"
+__version__ = "2.1.5a1.dev202304141812"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/client.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 from pyrogram import raw
 from pyrogram import utils
 from pyrogram.crypto import aes
 from pyrogram.errors import CDNFileHashMismatch
 from pyrogram.errors import (
     SessionPasswordNeeded,
     VolumeLocNotFound, ChannelPrivate,
-    AuthBytesInvalid, BadRequest
+    AuthBytesInvalid, BadRequest,
+    ListenerCanceled
 )
 from pyrogram.handlers.handler import Handler
 from pyrogram.methods import Methods
 from pyrogram.session import Auth, Session
 from pyrogram.storage import FileStorage, MemoryStorage
 from pyrogram.types import User, TermsOfService
 from pyrogram.utils import ainput
@@ -289,14 +290,46 @@
 
     async def __aexit__(self, *args):
         try:
             await self.stop()
         except ConnectionError:
             pass
 
+    async def listen(self, chat_id, filters=None, timeout=None):
+        if type(chat_id) != int:
+            chat = await self.get_chat(chat_id)
+            chat_id = chat.id
+
+        future = self.loop.create_future()
+        future.add_done_callback(
+            functools.partial(self.clear_listener, chat_id)
+        )
+        self.listening.update({
+            chat_id: {"future": future, "filters": filters}
+        })
+        return await asyncio.wait_for(future, timeout)
+
+    async def ask(self, chat_id, text, filters=None, timeout=None, *args, **kwargs):
+        request = await self.send_message(chat_id, text, *args, **kwargs)
+        response = await self.listen(chat_id, filters, timeout)
+        response.request = request
+        return response
+
+    def clear_listener(self, chat_id, future):
+        if future == self.listening[chat_id]:
+            self.listening.pop(chat_id, None)
+
+    def cancel_listener(self, chat_id):
+        listener = self.listening.get(chat_id)
+        if not listener or listener['future'].done():
+            return
+
+        listener['future'].set_exception(ListenerCanceled())
+        self.clear_listener(chat_id, listener['future'])
+
     async def authorize(self) -> User:
         if self.bot_token:
             return await self.sign_in_bot(self.bot_token)
 
         print(f"Welcome to Pyrogram (version {__version__})")
         print(f"Pyrogram is free software and comes with ABSOLUTELY NO WARRANTY. Licensed\n"
               f"under the terms of the {__license__}.\n")
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/connection.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/aes.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/mtproto.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/prime.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/crypto/rsa.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/dispatcher.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from collections import OrderedDict
 
 import pyrogram
 from pyrogram import utils
 from pyrogram.handlers import (
     CallbackQueryHandler, MessageHandler, EditedMessageHandler, DeletedMessagesHandler,
     UserStatusHandler, RawUpdateHandler, InlineQueryHandler, PollHandler,
-    ChosenInlineResultHandler, ChatMemberUpdatedHandler, ChatJoinRequestHandler
+    ChosenInlineResultHandler, ChatMemberUpdatedHandler, ChatJoinRequestHandler,
+    ConversationHandler
 )
 from pyrogram.raw.types import (
     UpdateNewMessage, UpdateNewChannelMessage, UpdateNewScheduledMessage,
     UpdateEditMessage, UpdateEditChannelMessage,
     UpdateDeleteMessages, UpdateDeleteChannelMessages,
     UpdateBotCallbackQuery, UpdateInlineBotCallbackQuery,
     UpdateUserStatus, UpdateBotInlineQuery, UpdateMessagePoll,
@@ -59,14 +60,17 @@
 
         self.handler_worker_tasks = []
         self.locks_list = []
 
         self.updates_queue = asyncio.Queue()
         self.groups = OrderedDict()
 
+        self.conversation_handler = ConversationHandler()
+        self.groups[0] = [self.conversation_handler]
+
         async def message_parser(update, users, chats):
             return (
                 await pyrogram.types.Message._parse(self.client, update.message, users, chats,
                                                     isinstance(update, UpdateNewScheduledMessage)),
                 MessageHandler
             )
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/emoji.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/auto_name.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_action.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_event_action.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_member_status.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_members_filter.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/chat_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_entity_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_media_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/message_service_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/messages_filter.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/next_code_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/parse_mode.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/poll_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/sent_code_type.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/enums/user_status.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/errors/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/errors/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,11 @@
 
 
 class CDNFileHashMismatch(SecurityError):
     """Raised when a CDN file hash mismatch occurs."""
 
     def __init__(self):
         super().__init__("A CDN file hash mismatch has occurred.")
+
+class ListenerCanceled(Exception):
+    """Raised when a Pyromod listener is canceled."""
+    pass
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/errors/rpc_error.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/file_id.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/filters.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,38 +435,41 @@
 media_spoiler = create(media_spoiler_filter)
 """Filter media messages that contain a spoiler."""
 
 
 # endregion
 
 # region private_filter
-async def private_filter(_, __, m: Message):
-    return bool(m.chat and m.chat.type in {enums.ChatType.PRIVATE, enums.ChatType.BOT})
+async def private_filter(_, __, u: Update):
+    m = u.message if isinstance(u, CallbackQuery) else u
+    return bool(m and m.chat and m.chat.type in {enums.ChatType.PRIVATE, enums.ChatType.BOT})
 
 
 private = create(private_filter)
 """Filter messages sent in private chats."""
 
 
 # endregion
 
 # region group_filter
-async def group_filter(_, __, m: Message):
-    return bool(m.chat and m.chat.type in {enums.ChatType.GROUP, enums.ChatType.SUPERGROUP})
+async def group_filter(_, __, u: Update):
+    m = u.message if isinstance(u, CallbackQuery) else u
+    return bool(m and m.chat and m.chat.type in {enums.ChatType.GROUP, enums.ChatType.SUPERGROUP})
 
 
 group = create(group_filter)
 """Filter messages sent in group or supergroup chats."""
 
 
 # endregion
 
 # region channel_filter
-async def channel_filter(_, __, m: Message):
-    return bool(m.chat and m.chat.type == enums.ChatType.CHANNEL)
+async def channel_filter(_, __, u: Update):
+    m = u.message if isinstance(u, CallbackQuery) else u
+    return bool(m and m.chat and m.chat.type == enums.ChatType.CHANNEL)
 
 
 channel = create(channel_filter)
 """Filter messages sent in channels."""
 
 
 # endregion
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from .callback_query_handler import CallbackQueryHandler
 from .chat_join_request_handler import ChatJoinRequestHandler
 from .chat_member_updated_handler import ChatMemberUpdatedHandler
+from .conversation_handler import ConversationHandler
 from .chosen_inline_result_handler import ChosenInlineResultHandler
 from .deleted_messages_handler import DeletedMessagesHandler
 from .disconnect_handler import DisconnectHandler
 from .edited_message_handler import EditedMessageHandler
 from .inline_query_handler import InlineQueryHandler
 from .message_handler import MessageHandler
 from .poll_handler import PollHandler
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/callback_query_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/disconnect_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/edited_message_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/inline_query_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/message_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/user_status_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,33 +17,31 @@
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Callable
 
 from .handler import Handler
 
 
-class MessageHandler(Handler):
-    """The Message handler class. Used to handle new messages.
-    It is intended to be used with :meth:`~pyrogram.Client.add_handler`
+class UserStatusHandler(Handler):
+    """The UserStatus handler class. Used to handle user status updates (user going online or offline).
+    It is intended to be used with :meth:`~pyrogram.Client.add_handler`.
 
-    For a nicer way to register this handler, have a look at the
-    :meth:`~pyrogram.Client.on_message` decorator.
+    For a nicer way to register this handler, have a look at the :meth:`~pyrogram.Client.on_user_status` decorator.
 
     Parameters:
         callback (``Callable``):
-            Pass a function that will be called when a new Message arrives. It takes *(client, message)*
+            Pass a function that will be called when a new user status update arrives. It takes *(client, user)*
             as positional arguments (look at the section below for a detailed description).
 
         filters (:obj:`Filters`):
-            Pass one or more filters to allow only a subset of messages to be passed
-            in your callback function.
+            Pass one or more filters to allow only a subset of users to be passed in your callback function.
 
     Other parameters:
         client (:obj:`~pyrogram.Client`):
-            The Client itself, useful when you want to call other API methods inside the message handler.
+            The Client itself, useful when you want to call other API methods inside the user status handler.
 
-        message (:obj:`~pyrogram.types.Message`):
-            The received message.
+        user (:obj:`~pyrogram.types.User`):
+            The user containing the updated status.
     """
 
     def __init__(self, callback: Callable, filters=None):
         super().__init__(callback, filters)
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/poll_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/raw_update_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/handlers/user_status_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/log_out.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Callable
+import logging
 
-from .handler import Handler
+import pyrogram
+from pyrogram import raw
 
+log = logging.getLogger(__name__)
 
-class UserStatusHandler(Handler):
-    """The UserStatus handler class. Used to handle user status updates (user going online or offline).
-    It is intended to be used with :meth:`~pyrogram.Client.add_handler`.
 
-    For a nicer way to register this handler, have a look at the :meth:`~pyrogram.Client.on_user_status` decorator.
+class LogOut:
+    async def log_out(
+        self: "pyrogram.Client",
+    ):
+        """Log out from Telegram and delete the *\\*.session* file.
 
-    Parameters:
-        callback (``Callable``):
-            Pass a function that will be called when a new user status update arrives. It takes *(client, user)*
-            as positional arguments (look at the section below for a detailed description).
+        When you log out, the current client is stopped and the storage session deleted.
+        No more API calls can be made until you start the client and re-authorize again.
 
-        filters (:obj:`Filters`):
-            Pass one or more filters to allow only a subset of users to be passed in your callback function.
+        .. include:: /_includes/usable-by/users-bots.rst
 
-    Other parameters:
-        client (:obj:`~pyrogram.Client`):
-            The Client itself, useful when you want to call other API methods inside the user status handler.
+        Returns:
+            ``bool``: On success, True is returned.
 
-        user (:obj:`~pyrogram.types.User`):
-            The user containing the updated status.
-    """
+        Example:
+            .. code-block:: python
 
-    def __init__(self, callback: Callable, filters=None):
-        super().__init__(callback, filters)
+                # Log out.
+                app.log_out()
+        """
+        await self.invoke(raw.functions.auth.LogOut())
+        await self.stop()
+        await self.storage.delete()
+
+        return True
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/invoke.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/advanced/save_file.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/check_password.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/connect.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/disconnect.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/initialize.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/log_out.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import logging
+from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
-log = logging.getLogger(__name__)
 
-
-class LogOut:
-    async def log_out(
+class SetChatProtectedContent:
+    async def set_chat_protected_content(
         self: "pyrogram.Client",
-    ):
-        """Log out from Telegram and delete the *\\*.session* file.
-
-        When you log out, the current client is stopped and the storage session deleted.
-        No more API calls can be made until you start the client and re-authorize again.
+        chat_id: Union[int, str],
+        enabled: bool
+    ) -> bool:
+        """Set the chat protected content setting.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
-        Returns:
-            ``bool``: On success, True is returned.
+        Parameters:
+            chat_id (``int`` | ``str``):
+                Unique identifier (int) or username (str) of the target chat.
 
-        Example:
-            .. code-block:: python
+            enabled (``bool``):
+                Pass True to enable the protected content setting, False to disable.
 
-                # Log out.
-                app.log_out()
+        Returns:
+            ``bool``: On success, True is returned.
         """
-        await self.invoke(raw.functions.auth.LogOut())
-        await self.stop()
-        await self.storage.delete()
+
+        await self.invoke(
+            raw.functions.messages.ToggleNoForwards(
+                peer=await self.resolve_peer(chat_id),
+                enabled=enabled
+            )
+        )
 
         return True
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/recover_password.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/resend_code.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/send_code.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_in.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/sign_up.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/auth/terminate.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/send_game.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/bots/set_game_score.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/archive_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_channel.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_group.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_channel.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/join_chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/leave_chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,36 +18,45 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class SetChatProtectedContent:
-    async def set_chat_protected_content(
+class GetDiscussionRepliesCount:
+    async def get_discussion_replies_count(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
-        enabled: bool
-    ) -> bool:
-        """Set the chat protected content setting.
+        message_id: int,
+    ) -> int:
+        """Get the total count of replies in a discussion thread.
 
-        .. include:: /_includes/usable-by/users-bots.rst
+        .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
-            enabled (``bool``):
-                Pass True to enable the protected content setting, False to disable.
+            message_id (``int``):
+                Message id.
 
-        Returns:
-            ``bool``: On success, True is returned.
+        Example:
+            .. code-block:: python
+
+                count = await app.get_discussion_replies_count(chat_id, message_id)
         """
 
-        await self.invoke(
-            raw.functions.messages.ToggleNoForwards(
+        r = await self.invoke(
+            raw.functions.messages.GetReplies(
                 peer=await self.resolve_peer(chat_id),
-                enabled=enabled
+                msg_id=message_id,
+                offset_id=0,
+                offset_date=0,
+                add_offset=0,
+                limit=1,
+                max_id=0,
+                min_id=0,
+                hash=0
             )
         )
 
-        return True
+        return r.count
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/add_contact.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_poll.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 from .send_venue import SendVenue
 from .send_video import SendVideo
 from .send_video_note import SendVideoNote
 from .send_voice import SendVoice
 from .stop_poll import StopPoll
 from .stream_media import StreamMedia
 from .vote_poll import VotePoll
+from .wait_for_message import WaitForMessage
+from .wait_for_callback_query import WaitForCallbackQuery
 
 
 class Messages(
     DeleteMessages,
     EditMessageCaption,
     EditMessageReplyMarkup,
     EditMessageMedia,
@@ -110,10 +112,12 @@
     SearchMessagesCount,
     SearchGlobalCount,
     GetDiscussionMessage,
     SendReaction,
     GetDiscussionReplies,
     GetDiscussionRepliesCount,
     StreamMedia,
-    GetCustomEmojiStickers
+    GetCustomEmojiStickers,
+    WaitForMessage,
+    WaitForCallbackQuery
 ):
     pass
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/copy_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/delete_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/download_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/forward_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_reaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,45 +18,56 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class GetDiscussionRepliesCount:
-    async def get_discussion_replies_count(
+class SendReaction:
+    async def send_reaction(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         message_id: int,
-    ) -> int:
-        """Get the total count of replies in a discussion thread.
+        emoji: str = "",
+        big: bool = False
+    ) -> bool:
+        """Send a reaction to a message.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
             message_id (``int``):
-                Message id.
+                Identifier of the message.
+
+            emoji (``str``, *optional*):
+                Reaction emoji.
+                Pass "" as emoji (default) to retract the reaction.
+            
+            big (``bool``, *optional*):
+                Pass True to show a bigger and longer reaction.
+                Defaults to False.
+
+        Returns:
+            ``bool``: On success, True is returned.
 
         Example:
             .. code-block:: python
 
-                count = await app.get_discussion_replies_count(chat_id, message_id)
-        """
+                # Send a reaction
+                await app.send_reaction(chat_id, message_id, "🔥")
 
-        r = await self.invoke(
-            raw.functions.messages.GetReplies(
+                # Retract a reaction
+                await app.send_reaction(chat_id, message_id)
+        """
+        await self.invoke(
+            raw.functions.messages.SendReaction(
                 peer=await self.resolve_peer(chat_id),
                 msg_id=message_id,
-                offset_id=0,
-                offset_date=0,
-                add_offset=0,
-                limit=1,
-                max_id=0,
-                min_id=0,
-                hash=0
+                reaction=[raw.types.ReactionEmoji(emoticon=emoji)] if emoji else None,
+                big=big
             )
         )
 
-        return r.count
+        return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_media_group.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/get_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/inline_session.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/retract_vote.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_global.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_global_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_messages.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_animation.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_audio.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_contact.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_dice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_document.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_location.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_media_group.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_poll.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_reaction.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/vote_poll.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,62 +12,58 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union
+from typing import Union, List
 
 import pyrogram
 from pyrogram import raw
+from pyrogram import types
 
 
-class SendReaction:
-    async def send_reaction(
+class VotePoll:
+    async def vote_poll(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
-        message_id: int,
-        emoji: str = "",
-        big: bool = False
-    ) -> bool:
-        """Send a reaction to a message.
+        message_id: id,
+        options: Union[int, List[int]]
+    ) -> "types.Poll":
+        """Vote a poll.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
+                For your personal cloud (Saved Messages) you can simply use "me" or "self".
+                For a contact that exists in your Telegram address book you can use his phone number (str).
 
             message_id (``int``):
-                Identifier of the message.
+                Identifier of the original message with the poll.
 
-            emoji (``str``, *optional*):
-                Reaction emoji.
-                Pass "" as emoji (default) to retract the reaction.
-            
-            big (``bool``, *optional*):
-                Pass True to show a bigger and longer reaction.
-                Defaults to False.
+            options (``Int`` | List of ``int``):
+                Index or list of indexes (for multiple answers) of the poll option(s) you want to vote for (0 to 9).
 
         Returns:
-            ``bool``: On success, True is returned.
+            :obj:`~pyrogram.types.Poll` - On success, the poll with the chosen option is returned.
 
         Example:
             .. code-block:: python
 
-                # Send a reaction
-                await app.send_reaction(chat_id, message_id, "🔥")
-
-                # Retract a reaction
-                await app.send_reaction(chat_id, message_id)
+                await app.vote_poll(chat_id, message_id, 6)
         """
-        await self.invoke(
-            raw.functions.messages.SendReaction(
+
+        poll = (await self.get_messages(chat_id, message_id)).poll
+        options = [options] if not isinstance(options, list) else options
+
+        r = await self.invoke(
+            raw.functions.messages.SendVote(
                 peer=await self.resolve_peer(chat_id),
                 msg_id=message_id,
-                reaction=[raw.types.ReactionEmoji(emoticon=emoji)] if emoji else None,
-                big=big
+                options=[poll.options[option].data for option in options]
             )
         )
 
-        return True
+        return types.Poll._parse(self, r.updates[0])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_sticker.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_venue.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_video.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_video_note.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/send_voice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/stop_poll.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/stream_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/messages/vote_poll.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_document.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,58 +12,54 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union, List
+from typing import Optional, List, Union, BinaryIO
 
-import pyrogram
-from pyrogram import raw
-from pyrogram import types
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
+
+
+class InputMediaDocument(InputMedia):
+    """A generic file to be sent inside an album.
+
+    Parameters:
+        media (``str`` | ``BinaryIO``):
+            File to send.
+            Pass a file_id as string to send a file that exists on the Telegram servers or
+            pass a file path as string to upload a new file that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get a file from the Internet.
+
+        thumb (``str``):
+            Thumbnail of the file sent.
+            The thumbnail should be in JPEG format and less than 200 KB in size.
+            A thumbnail's width and height should not exceed 320 pixels.
+            Thumbnails can't be reused and can be only uploaded as a new file.
+
+        caption (``str``, *optional*):
+            Caption of the document to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
+
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+    """
+
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        thumb: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None
+    ):
+        super().__init__(media, caption, parse_mode, caption_entities)
 
-
-class VotePoll:
-    async def vote_poll(
-        self: "pyrogram.Client",
-        chat_id: Union[int, str],
-        message_id: id,
-        options: Union[int, List[int]]
-    ) -> "types.Poll":
-        """Vote a poll.
-
-        .. include:: /_includes/usable-by/users.rst
-
-        Parameters:
-            chat_id (``int`` | ``str``):
-                Unique identifier (int) or username (str) of the target chat.
-                For your personal cloud (Saved Messages) you can simply use "me" or "self".
-                For a contact that exists in your Telegram address book you can use his phone number (str).
-
-            message_id (``int``):
-                Identifier of the original message with the poll.
-
-            options (``Int`` | List of ``int``):
-                Index or list of indexes (for multiple answers) of the poll option(s) you want to vote for (0 to 9).
-
-        Returns:
-            :obj:`~pyrogram.types.Poll` - On success, the poll with the chosen option is returned.
-
-        Example:
-            .. code-block:: python
-
-                await app.vote_poll(chat_id, message_id, 6)
-        """
-
-        poll = (await self.get_messages(chat_id, message_id)).poll
-        options = [options] if not isinstance(options, list) else options
-
-        r = await self.invoke(
-            raw.functions.messages.SendVote(
-                peer=await self.resolve_peer(chat_id),
-                msg_id=message_id,
-                options=[poll.options[option].data for option in options]
-            )
-        )
-
-        return types.Poll._parse(self, r.updates[0])
+        self.thumb = thumb
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/block_user.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_common_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_me.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/get_users.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/set_username.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/unblock_user.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/users/update_profile.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/add_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/compose.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/idle.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/restart.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/run.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/start.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/stop.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/mime_types.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/html.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/markdown.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/parser.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/parser/utils.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/future_salt.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/future_salts.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/gzip_packed.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/list.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/msg_container.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/bool.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/double.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/int.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/string.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/primitives/vector.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/raw/core/tl_object.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/auth.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/data_center.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/msg_factory.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/msg_id.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/internals/seq_no.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/session/session.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/file_storage.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/memory_storage.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/sqlite_storage.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/storage/storage.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/sync.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/sent_code.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_document.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_photo.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,47 +19,45 @@
 from typing import Optional, List, Union, BinaryIO
 
 from .input_media import InputMedia
 from ..messages_and_media import MessageEntity
 from ... import enums
 
 
-class InputMediaDocument(InputMedia):
-    """A generic file to be sent inside an album.
+class InputMediaPhoto(InputMedia):
+    """A photo to be sent inside an album.
+    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
 
     Parameters:
         media (``str`` | ``BinaryIO``):
-            File to send.
-            Pass a file_id as string to send a file that exists on the Telegram servers or
-            pass a file path as string to upload a new file that exists on your local machine or
+            Photo to send.
+            Pass a file_id as string to send a photo that exists on the Telegram servers or
+            pass a file path as string to upload a new photo that exists on your local machine or
             pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a file from the Internet.
-
-        thumb (``str``):
-            Thumbnail of the file sent.
-            The thumbnail should be in JPEG format and less than 200 KB in size.
-            A thumbnail's width and height should not exceed 320 pixels.
-            Thumbnails can't be reused and can be only uploaded as a new file.
+            pass an HTTP URL as a string for Telegram to get a photo from the Internet.
 
         caption (``str``, *optional*):
-            Caption of the document to be sent, 0-1024 characters.
+            Caption of the photo to be sent, 0-1024 characters.
             If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+
+        has_spoiler (``bool``, *optional*):
+            Pass True if the photo needs to be covered with a spoiler animation.
     """
 
     def __init__(
         self,
         media: Union[str, BinaryIO],
-        thumb: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None
+        caption_entities: List[MessageEntity] = None,
+        has_spoiler: bool = None
     ):
         super().__init__(media, caption, parse_mode, caption_entities)
 
-        self.thumb = thumb
+        self.has_spoiler = has_spoiler
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_media_video.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,45 +19,73 @@
 from typing import Optional, List, Union, BinaryIO
 
 from .input_media import InputMedia
 from ..messages_and_media import MessageEntity
 from ... import enums
 
 
-class InputMediaPhoto(InputMedia):
-    """A photo to be sent inside an album.
+class InputMediaVideo(InputMedia):
+    """A video to be sent inside an album.
     It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
 
     Parameters:
         media (``str`` | ``BinaryIO``):
-            Photo to send.
-            Pass a file_id as string to send a photo that exists on the Telegram servers or
-            pass a file path as string to upload a new photo that exists on your local machine or
+            Video to send.
+            Pass a file_id as string to send a video that exists on the Telegram servers or
+            pass a file path as string to upload a new video that exists on your local machine or
             pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a photo from the Internet.
+            pass an HTTP URL as a string for Telegram to get a video from the Internet.
+
+        thumb (``str``):
+            Thumbnail of the video sent.
+            The thumbnail should be in JPEG format and less than 200 KB in size.
+            A thumbnail's width and height should not exceed 320 pixels.
+            Thumbnails can't be reused and can be only uploaded as a new file.
 
         caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
+            Caption of the video to be sent, 0-1024 characters.
             If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+        width (``int``, *optional*):
+            Video width.
+
+        height (``int``, *optional*):
+            Video height.
+
+        duration (``int``, *optional*):
+            Video duration.
+
+        supports_streaming (``bool``, *optional*):
+            Pass True, if the uploaded video is suitable for streaming.
+
         has_spoiler (``bool``, *optional*):
             Pass True if the photo needs to be covered with a spoiler animation.
     """
 
     def __init__(
         self,
         media: Union[str, BinaryIO],
+        thumb: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List[MessageEntity] = None,
-        has_spoiler: bool = None
+        width: int = 0,
+        height: int = 0,
+        duration: int = 0,
+        supports_streaming: bool = True,
+        has_spoiler: bool = None,
     ):
         super().__init__(media, caption, parse_mode, caption_entities)
 
+        self.thumb = thumb
+        self.width = width
+        self.height = height
+        self.duration = duration
+        self.supports_streaming = supports_streaming
         self.has_spoiler = has_spoiler
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_media_video.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,80 +12,100 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List, Union, BinaryIO
+from typing import List, Optional, Union
 
-from .input_media import InputMedia
-from ..messages_and_media import MessageEntity
-from ... import enums
+import pyrogram
+from pyrogram import raw
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from ..object import Object
 
 
-class InputMediaVideo(InputMedia):
-    """A video to be sent inside an album.
-    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
+class Thumbnail(Object):
+    """One size of a photo or a file/sticker thumbnail.
 
     Parameters:
-        media (``str`` | ``BinaryIO``):
-            Video to send.
-            Pass a file_id as string to send a video that exists on the Telegram servers or
-            pass a file path as string to upload a new video that exists on your local machine or
-            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a video from the Internet.
-
-        thumb (``str``):
-            Thumbnail of the video sent.
-            The thumbnail should be in JPEG format and less than 200 KB in size.
-            A thumbnail's width and height should not exceed 320 pixels.
-            Thumbnails can't be reused and can be only uploaded as a new file.
-
-        caption (``str``, *optional*):
-            Caption of the video to be sent, 0-1024 characters.
-            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
-
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
-
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
-
-        width (``int``, *optional*):
-            Video width.
-
-        height (``int``, *optional*):
-            Video height.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        duration (``int``, *optional*):
-            Video duration.
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        supports_streaming (``bool``, *optional*):
-            Pass True, if the uploaded video is suitable for streaming.
+        width (``int``):
+            Photo width.
 
-        has_spoiler (``bool``, *optional*):
-            Pass True if the photo needs to be covered with a spoiler animation.
+        height (``int``):
+            Photo height.
+
+        file_size (``int``):
+            File size.
     """
 
     def __init__(
         self,
-        media: Union[str, BinaryIO],
-        thumb: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None,
-        width: int = 0,
-        height: int = 0,
-        duration: int = 0,
-        supports_streaming: bool = True,
-        has_spoiler: bool = None,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        file_size: int
     ):
-        super().__init__(media, caption, parse_mode, caption_entities)
+        super().__init__(client)
 
-        self.thumb = thumb
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
         self.width = width
         self.height = height
-        self.duration = duration
-        self.supports_streaming = supports_streaming
-        self.has_spoiler = has_spoiler
+        self.file_size = file_size
+
+    @staticmethod
+    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
+        if isinstance(media, raw.types.Photo):
+            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
+            raw_thumbs.sort(key=lambda p: p.size)
+            raw_thumbs = raw_thumbs[:-1]
+
+            file_type = FileType.PHOTO
+        elif isinstance(media, raw.types.Document):
+            raw_thumbs = media.thumbs
+            file_type = FileType.THUMBNAIL
+        else:
+            return
+
+        parsed_thumbs = []
+
+        for thumb in raw_thumbs:
+            if not isinstance(thumb, raw.types.PhotoSize):
+                continue
+
+            parsed_thumbs.append(
+                Thumbnail(
+                    file_id=FileId(
+                        file_type=file_type,
+                        dc_id=media.dc_id,
+                        media_id=media.id,
+                        access_hash=media.access_hash,
+                        file_reference=media.file_reference,
+                        thumbnail_file_type=file_type,
+                        thumbnail_source=ThumbnailSource.THUMBNAIL,
+                        thumbnail_size=thumb.type,
+                        volume_id=0,
+                        local_id=0
+                    ).encode(),
+                    file_unique_id=FileUniqueId(
+                        file_unique_type=FileUniqueType.DOCUMENT,
+                        media_id=media.id
+                    ).encode(),
+                    width=thumb.w,
+                    height=thumb.h,
+                    file_size=thumb.size,
+                    client=client
+                )
+            )
+
+        return parsed_thumbs or None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/list.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/animation.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/audio.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/contact.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/dice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/document.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/game.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/location.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -9567,8 +9567,240 @@
 000255e0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
 000255f0: 636c 6965 6e74 2e75 6e70 696e 5f63 6861  client.unpin_cha
 00025600: 745f 6d65 7373 6167 6528 0a20 2020 2020  t_message(.     
 00025610: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
 00025620: 656c 662e 6368 6174 2e69 642c 0a20 2020  elf.chat.id,.   
 00025630: 2020 2020 2020 2020 206d 6573 7361 6765           message
 00025640: 5f69 643d 7365 6c66 2e69 640a 2020 2020  _id=self.id.    
-00025650: 2020 2020 290a                               ).
+00025650: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
+00025660: 2064 6566 2061 736b 280a 2020 2020 2020   def ask(.      
+00025670: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00025680: 7465 7874 3a20 7374 722c 0a20 2020 2020  text: str,.     
+00025690: 2020 2071 756f 7465 3a20 626f 6f6c 203d     quote: bool =
+000256a0: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+000256b0: 6172 7365 5f6d 6f64 653a 204f 7074 696f  arse_mode: Optio
+000256c0: 6e61 6c5b 2265 6e75 6d73 2e50 6172 7365  nal["enums.Parse
+000256d0: 4d6f 6465 225d 203d 204e 6f6e 652c 0a20  Mode"] = None,. 
+000256e0: 2020 2020 2020 2065 6e74 6974 6965 733a         entities:
+000256f0: 204c 6973 745b 2274 7970 6573 2e4d 6573   List["types.Mes
+00025700: 7361 6765 456e 7469 7479 225d 203d 204e  sageEntity"] = N
+00025710: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
+00025720: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
+00025730: 6576 6965 773a 2062 6f6f 6c20 3d20 4e6f  eview: bool = No
+00025740: 6e65 2c0a 2020 2020 2020 2020 6469 7361  ne,.        disa
+00025750: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00025760: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+00025770: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
+00025780: 6d65 7373 6167 655f 6964 3a20 696e 7420  message_id: int 
+00025790: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000257a0: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
+000257b0: 652c 0a20 2020 2020 2020 2066 696c 7465  e,.        filte
+000257c0: 7273 3d4e 6f6e 652c 0a20 2020 2020 2020  rs=None,.       
+000257d0: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
+000257e0: 4e6f 6e65 0a20 2020 2029 202d 3e20 224d  None.    ) -> "M
+000257f0: 6573 7361 6765 223a 0a20 2020 2020 2020  essage":.       
+00025800: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
+00025810: 202a 6173 6b2a 206f 6620 3a6f 626a 3a60   *ask* of :obj:`
+00025820: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+00025830: 4d65 7373 6167 6560 2e0a 2020 2020 2020  Message`..      
+00025840: 2020 0a20 2020 2020 2020 2055 7365 2061    .        Use a
+00025850: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
+00025860: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
+00025870: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+00025880: 6e0a 0a20 2020 2020 2020 2020 2020 2063  n..            c
+00025890: 6c69 656e 742e 7365 6e64 5f6d 6573 7361  lient.send_messa
+000258a0: 6765 2863 6861 745f 6964 2c20 2257 6861  ge(chat_id, "Wha
+000258b0: 7420 6973 2079 6f75 7220 6e61 6d65 3f22  t is your name?"
+000258c0: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
+000258d0: 6965 6e74 2e77 6169 745f 666f 725f 6d65  ient.wait_for_me
+000258e0: 7373 6167 6528 6368 6174 5f69 6429 0a20  ssage(chat_id). 
+000258f0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00025900: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
+00025910: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
+00025920: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00025930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025940: 206d 6573 7361 6765 2e61 736b 2822 5768   message.ask("Wh
+00025950: 6174 2069 7320 796f 7572 206e 616d 653f  at is your name?
+00025960: 2229 0a0a 2020 2020 2020 2020 5061 7261  ")..        Para
+00025970: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00025980: 2020 2020 7465 7874 2028 6060 7374 7260      text (``str`
+00025990: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
+000259a0: 2020 2020 5465 7874 206f 6620 7468 6520      Text of the 
+000259b0: 6d65 7373 6167 6520 746f 2062 6520 7365  message to be se
+000259c0: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
+000259d0: 2071 756f 7465 2028 6060 626f 6f6c 6060   quote (``bool``
+000259e0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+000259f0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00025a00: 6620 6060 5472 7565 6060 2c20 7468 6520  f ``True``, the 
+00025a10: 6d65 7373 6167 6520 7769 6c6c 2062 6520  message will be 
+00025a20: 7365 6e74 2061 7320 6120 7265 706c 7920  sent as a reply 
+00025a30: 746f 2074 6869 7320 6d65 7373 6167 652e  to this message.
+00025a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025a50: 2049 6620 2a72 6570 6c79 5f74 6f5f 6d65   If *reply_to_me
+00025a60: 7373 6167 655f 6964 2a20 6973 2070 6173  ssage_id* is pas
+00025a70: 7365 642c 2074 6869 7320 7061 7261 6d65  sed, this parame
+00025a80: 7465 7220 7769 6c6c 2062 6520 6967 6e6f  ter will be igno
+00025a90: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
+00025aa0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00025ab0: 2060 6054 7275 6560 6020 696e 2067 726f   ``True`` in gro
+00025ac0: 7570 2063 6861 7473 2061 6e64 2060 6046  up chats and ``F
+00025ad0: 616c 7365 6060 2069 6e20 7072 6976 6174  alse`` in privat
+00025ae0: 6520 6368 6174 732e 0a0a 2020 2020 2020  e chats...      
+00025af0: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
+00025b00: 2028 3a6f 626a 3a60 7e70 7972 6f67 7261   (:obj:`~pyrogra
+00025b10: 6d2e 656e 756d 732e 5061 7273 654d 6f64  m.enums.ParseMod
+00025b20: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
+00025b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025b40: 2042 7920 6465 6661 756c 742c 2074 6578   By default, tex
+00025b50: 7473 2061 7265 2070 6172 7365 6420 7573  ts are parsed us
+00025b60: 696e 6720 626f 7468 204d 6172 6b64 6f77  ing both Markdow
+00025b70: 6e20 616e 6420 4854 4d4c 2073 7479 6c65  n and HTML style
+00025b80: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00025b90: 2020 2059 6f75 2063 616e 2063 6f6d 6269     You can combi
+00025ba0: 6e65 2062 6f74 6820 7379 6e74 6178 6573  ne both syntaxes
+00025bb0: 2074 6f67 6574 6865 722e 0a0a 2020 2020   together...    
+00025bc0: 2020 2020 2020 2020 656e 7469 7469 6573          entities
+00025bd0: 2028 4c69 7374 206f 6620 3a6f 626a 3a60   (List of :obj:`
+00025be0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+00025bf0: 4d65 7373 6167 6545 6e74 6974 7960 293a  MessageEntity`):
+00025c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025c10: 204c 6973 7420 6f66 2073 7065 6369 616c   List of special
+00025c20: 2065 6e74 6974 6965 7320 7468 6174 2061   entities that a
+00025c30: 7070 6561 7220 696e 206d 6573 7361 6765  ppear in message
+00025c40: 2074 6578 742c 2077 6869 6368 2063 616e   text, which can
+00025c50: 2062 6520 7370 6563 6966 6965 6420 696e   be specified in
+00025c60: 7374 6561 6420 6f66 202a 7061 7273 655f  stead of *parse_
+00025c70: 6d6f 6465 2a2e 0a0a 2020 2020 2020 2020  mode*...        
+00025c80: 2020 2020 6469 7361 626c 655f 7765 625f      disable_web_
+00025c90: 7061 6765 5f70 7265 7669 6577 2028 6060  page_preview (``
+00025ca0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+00025cb0: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
+00025cc0: 2020 2020 2044 6973 6162 6c65 7320 6c69       Disables li
+00025cd0: 6e6b 2070 7265 7669 6577 7320 666f 7220  nk previews for 
+00025ce0: 6c69 6e6b 7320 696e 2074 6869 7320 6d65  links in this me
+00025cf0: 7373 6167 652e 0a0a 2020 2020 2020 2020  ssage...        
+00025d00: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
+00025d10: 6669 6361 7469 6f6e 2028 6060 626f 6f6c  fication (``bool
+00025d20: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00025d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025d40: 2053 656e 6473 2074 6865 206d 6573 7361   Sends the messa
+00025d50: 6765 2073 696c 656e 746c 792e 0a20 2020  ge silently..   
+00025d60: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+00025d70: 7273 2077 696c 6c20 7265 6365 6976 6520  rs will receive 
+00025d80: 6120 6e6f 7469 6669 6361 7469 6f6e 2077  a notification w
+00025d90: 6974 6820 6e6f 2073 6f75 6e64 2e0a 0a20  ith no sound... 
+00025da0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00025db0: 5f74 6f5f 6d65 7373 6167 655f 6964 2028  _to_message_id (
+00025dc0: 6060 696e 7460 602c 202a 6f70 7469 6f6e  ``int``, *option
+00025dd0: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+00025de0: 2020 2020 2020 4966 2074 6865 206d 6573        If the mes
+00025df0: 7361 6765 2069 7320 6120 7265 706c 792c  sage is a reply,
+00025e00: 2049 4420 6f66 2074 6865 206f 7269 6769   ID of the origi
+00025e10: 6e61 6c20 6d65 7373 6167 652e 0a0a 2020  nal message...  
+00025e20: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00025e30: 6d61 726b 7570 2028 3a6f 626a 3a60 7e70  markup (:obj:`~p
+00025e40: 7972 6f67 7261 6d2e 7479 7065 732e 496e  yrogram.types.In
+00025e50: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+00025e60: 7570 6020 7c20 3a6f 626a 3a60 7e70 7972  up` | :obj:`~pyr
+00025e70: 6f67 7261 6d2e 7479 7065 732e 5265 706c  ogram.types.Repl
+00025e80: 794b 6579 626f 6172 644d 6172 6b75 7060  yKeyboardMarkup`
+00025e90: 207c 203a 6f62 6a3a 607e 7079 726f 6772   | :obj:`~pyrogr
+00025ea0: 616d 2e74 7970 6573 2e52 6570 6c79 4b65  am.types.ReplyKe
+00025eb0: 7962 6f61 7264 5265 6d6f 7665 6020 7c20  yboardRemove` | 
+00025ec0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00025ed0: 7479 7065 732e 466f 7263 6552 6570 6c79  types.ForceReply
+00025ee0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00025ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f00: 4164 6469 7469 6f6e 616c 2069 6e74 6572  Additional inter
+00025f10: 6661 6365 206f 7074 696f 6e73 2e20 416e  face options. An
+00025f20: 206f 626a 6563 7420 666f 7220 616e 2069   object for an i
+00025f30: 6e6c 696e 6520 6b65 7962 6f61 7264 2c20  nline keyboard, 
+00025f40: 6375 7374 6f6d 2072 6570 6c79 206b 6579  custom reply key
+00025f50: 626f 6172 642c 0a20 2020 2020 2020 2020  board,.         
+00025f60: 2020 2020 2020 2069 6e73 7472 7563 7469         instructi
+00025f70: 6f6e 7320 746f 2072 656d 6f76 6520 7265  ons to remove re
+00025f80: 706c 7920 6b65 7962 6f61 7264 206f 7220  ply keyboard or 
+00025f90: 746f 2066 6f72 6365 2061 2072 6570 6c79  to force a reply
+00025fa0: 2066 726f 6d20 7468 6520 7573 6572 2e0a   from the user..
+00025fb0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00025fc0: 7465 7273 2028 3a6f 626a 3a60 4669 6c74  ters (:obj:`Filt
+00025fd0: 6572 7360 293a 0a20 2020 2020 2020 2020  ers`):.         
+00025fe0: 2020 2020 2020 2050 6173 7320 6f6e 6520         Pass one 
+00025ff0: 6f72 206d 6f72 6520 6669 6c74 6572 7320  or more filters 
+00026000: 746f 2061 6c6c 6f77 206f 6e6c 7920 6120  to allow only a 
+00026010: 7375 6273 6574 206f 6620 6361 6c6c 6261  subset of callba
+00026020: 636b 2071 7565 7269 6573 2074 6f20 6265  ck queries to be
+00026030: 2070 6173 7365 640a 2020 2020 2020 2020   passed.        
+00026040: 2020 2020 2020 2020 696e 2079 6f75 7220          in your 
+00026050: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
+00026060: 6e2e 0a0a 2020 2020 2020 2020 2020 2020  n...            
+00026070: 7469 6d65 6f75 7420 2860 6069 6e74 6060  timeout (``int``
+00026080: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+00026090: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000260a0: 696d 656f 7574 2069 6e20 7365 636f 6e64  imeout in second
+000260b0: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
+000260c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+000260d0: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+000260e0: 2e74 7970 6573 2e4d 6573 7361 6765 603a  .types.Message`:
+000260f0: 204f 6e20 7375 6363 6573 732c 2074 6865   On success, the
+00026100: 2072 6570 6c79 206d 6573 7361 6765 2069   reply message i
+00026110: 7320 7265 7475 726e 6564 2e0a 0a20 2020  s returned...   
+00026120: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+00026130: 2020 2020 2020 2020 2052 5043 4572 726f           RPCErro
+00026140: 723a 2049 6e20 6361 7365 206f 6620 6120  r: In case of a 
+00026150: 5465 6c65 6772 616d 2052 5043 2065 7272  Telegram RPC err
+00026160: 6f72 2e0a 2020 2020 2020 2020 2020 2020  or..            
+00026170: 6173 796e 6369 6f2e 5469 6d65 6f75 7445  asyncio.TimeoutE
+00026180: 7272 6f72 3a20 496e 2063 6173 6520 7265  rror: In case re
+00026190: 706c 7920 6e6f 7420 7265 6365 6976 6564  ply not received
+000261a0: 2077 6974 6869 6e20 7468 6520 7469 6d65   within the time
+000261b0: 6f75 742e 0a20 2020 2020 2020 2022 2222  out..        """
+000261c0: 0a20 2020 2020 2020 2069 6620 7175 6f74  .        if quot
+000261d0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+000261e0: 2020 2020 2020 2071 756f 7465 203d 2073         quote = s
+000261f0: 656c 662e 6368 6174 2e74 7970 6520 213d  elf.chat.type !=
+00026200: 2022 7072 6976 6174 6522 0a0a 2020 2020   "private"..    
+00026210: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
+00026220: 6d65 7373 6167 655f 6964 2069 7320 4e6f  message_id is No
+00026230: 6e65 2061 6e64 2071 756f 7465 3a0a 2020  ne and quote:.  
+00026240: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00026250: 746f 5f6d 6573 7361 6765 5f69 6420 3d20  to_message_id = 
+00026260: 7365 6c66 2e69 640a 0a20 2020 2020 2020  self.id..       
+00026270: 2072 6571 7565 7374 203d 2061 7761 6974   request = await
+00026280: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
+00026290: 6e64 5f6d 6573 7361 6765 280a 2020 2020  nd_message(.    
+000262a0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+000262b0: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
+000262c0: 2020 2020 2020 2020 2020 7465 7874 3d74            text=t
+000262d0: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
+000262e0: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
+000262f0: 655f 6d6f 6465 2c0a 2020 2020 2020 2020  e_mode,.        
+00026300: 2020 2020 656e 7469 7469 6573 3d65 6e74      entities=ent
+00026310: 6974 6965 732c 0a20 2020 2020 2020 2020  ities,.         
+00026320: 2020 2064 6973 6162 6c65 5f77 6562 5f70     disable_web_p
+00026330: 6167 655f 7072 6576 6965 773d 6469 7361  age_preview=disa
+00026340: 626c 655f 7765 625f 7061 6765 5f70 7265  ble_web_page_pre
+00026350: 7669 6577 2c0a 2020 2020 2020 2020 2020  view,.          
+00026360: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+00026370: 6361 7469 6f6e 3d64 6973 6162 6c65 5f6e  cation=disable_n
+00026380: 6f74 6966 6963 6174 696f 6e2c 0a20 2020  otification,.   
+00026390: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
+000263a0: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
+000263b0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000263c0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+000263d0: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
+000263e0: 5f6d 6172 6b75 700a 2020 2020 2020 2020  _markup.        
+000263f0: 290a 0a20 2020 2020 2020 2072 6570 6c79  )..        reply
+00026400: 5f6d 6573 7361 6765 203d 2061 7761 6974  _message = await
+00026410: 2073 656c 662e 5f63 6c69 656e 742e 7761   self._client.wa
+00026420: 6974 5f66 6f72 5f6d 6573 7361 6765 280a  it_for_message(.
+00026430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00026440: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
+00026450: 2020 2020 2020 6669 6c74 6572 733d 6669        filters=fi
+00026460: 6c74 6572 732c 0a20 2020 2020 2020 2020  lters,.         
+00026470: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
+00026480: 7574 0a20 2020 2020 2020 2029 0a0a 2020  ut.        )..  
+00026490: 2020 2020 2020 7265 706c 795f 6d65 7373        reply_mess
+000264a0: 6167 652e 7265 7175 6573 7420 3d20 7265  age.request = re
+000264b0: 7175 6573 740a 2020 2020 2020 2020 7265  quest.        re
+000264c0: 7475 726e 2072 6570 6c79 5f6d 6573 7361  turn reply_messa
+000264d0: 6765 0a                                  ge.
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/poll.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/voice.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,100 +12,85 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import List, Optional, Union
+from datetime import datetime
 
 import pyrogram
-from pyrogram import raw
-from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from pyrogram import raw, utils
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
 from ..object import Object
 
 
-class Thumbnail(Object):
-    """One size of a photo or a file/sticker thumbnail.
+class Voice(Object):
+    """A voice note.
 
     Parameters:
         file_id (``str``):
             Identifier for this file, which can be used to download or reuse the file.
 
         file_unique_id (``str``):
             Unique identifier for this file, which is supposed to be the same over time and for different accounts.
             Can't be used to download or reuse the file.
 
-        width (``int``):
-            Photo width.
+        duration (``int``):
+            Duration of the audio in seconds as defined by sender.
 
-        height (``int``):
-            Photo height.
+        waveform (``bytes``, *optional*):
+            Voice waveform.
 
-        file_size (``int``):
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
+
+        file_size (``int``, *optional*):
             File size.
+
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the voice was sent.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         file_id: str,
         file_unique_id: str,
-        width: int,
-        height: int,
-        file_size: int
+        duration: int,
+        waveform: bytes = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None
     ):
         super().__init__(client)
 
         self.file_id = file_id
         self.file_unique_id = file_unique_id
-        self.width = width
-        self.height = height
+        self.duration = duration
+        self.waveform = waveform
+        self.mime_type = mime_type
         self.file_size = file_size
+        self.date = date
 
     @staticmethod
-    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
-        if isinstance(media, raw.types.Photo):
-            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
-            raw_thumbs.sort(key=lambda p: p.size)
-            raw_thumbs = raw_thumbs[:-1]
-
-            file_type = FileType.PHOTO
-        elif isinstance(media, raw.types.Document):
-            raw_thumbs = media.thumbs
-            file_type = FileType.THUMBNAIL
-        else:
-            return
-
-        parsed_thumbs = []
-
-        for thumb in raw_thumbs:
-            if not isinstance(thumb, raw.types.PhotoSize):
-                continue
-
-            parsed_thumbs.append(
-                Thumbnail(
-                    file_id=FileId(
-                        file_type=file_type,
-                        dc_id=media.dc_id,
-                        media_id=media.id,
-                        access_hash=media.access_hash,
-                        file_reference=media.file_reference,
-                        thumbnail_file_type=file_type,
-                        thumbnail_source=ThumbnailSource.THUMBNAIL,
-                        thumbnail_size=thumb.type,
-                        volume_id=0,
-                        local_id=0
-                    ).encode(),
-                    file_unique_id=FileUniqueId(
-                        file_unique_type=FileUniqueType.DOCUMENT,
-                        media_id=media.id
-                    ).encode(),
-                    width=thumb.w,
-                    height=thumb.h,
-                    file_size=thumb.size,
-                    client=client
-                )
-            )
-
-        return parsed_thumbs or None
+    def _parse(client, voice: "raw.types.Document", attributes: "raw.types.DocumentAttributeAudio") -> "Voice":
+        return Voice(
+            file_id=FileId(
+                file_type=FileType.VOICE,
+                dc_id=voice.dc_id,
+                media_id=voice.id,
+                access_hash=voice.access_hash,
+                file_reference=voice.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=voice.id
+            ).encode(),
+            duration=attributes.duration,
+            mime_type=voice.mime_type,
+            file_size=voice.size,
+            waveform=attributes.waveform,
+            date=utils.timestamp_to_datetime(voice.date),
+            client=client
+        )
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/venue.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/video.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/voice.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,84 +13,70 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
+from typing import Dict
 
 import pyrogram
-from pyrogram import raw, utils
-from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from pyrogram import raw, types, utils
 from ..object import Object
 
 
-class Voice(Object):
-    """A voice note.
+class ChatJoiner(Object):
+    """Contains information about a joiner member of a chat.
 
     Parameters:
-        file_id (``str``):
-            Identifier for this file, which can be used to download or reuse the file.
+        user (:obj:`~pyrogram.types.User`):
+            Information about the user.
 
-        file_unique_id (``str``):
-            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
-            Can't be used to download or reuse the file.
+        date (:py:obj:`~datetime.datetime`):
+            Date when the user joined.
 
-        duration (``int``):
-            Duration of the audio in seconds as defined by sender.
+        bio (``str``, *optional*):
+            Bio of the user.
 
-        waveform (``bytes``, *optional*):
-            Voice waveform.
+        pending (``bool``, *optional*):
+            True in case the chat joiner has a pending request.
 
-        mime_type (``str``, *optional*):
-            MIME type of the file as defined by sender.
-
-        file_size (``int``, *optional*):
-            File size.
-
-        date (:py:obj:`~datetime.datetime`, *optional*):
-            Date the voice was sent.
+        approved_by (:obj:`~pyrogram.types.User`, *optional*):
+            Administrator who approved this chat joiner.
     """
 
     def __init__(
         self,
         *,
-        client: "pyrogram.Client" = None,
-        file_id: str,
-        file_unique_id: str,
-        duration: int,
-        waveform: bytes = None,
-        mime_type: str = None,
-        file_size: int = None,
-        date: datetime = None
+        client: "pyrogram.Client",
+        user: "types.User",
+        date: datetime = None,
+        bio: str = None,
+        pending: bool = None,
+        approved_by: "types.User" = None,
     ):
         super().__init__(client)
 
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.duration = duration
-        self.waveform = waveform
-        self.mime_type = mime_type
-        self.file_size = file_size
+        self.user = user
         self.date = date
+        self.bio = bio
+        self.pending = pending
+        self.approved_by = approved_by
 
     @staticmethod
-    def _parse(client, voice: "raw.types.Document", attributes: "raw.types.DocumentAttributeAudio") -> "Voice":
-        return Voice(
-            file_id=FileId(
-                file_type=FileType.VOICE,
-                dc_id=voice.dc_id,
-                media_id=voice.id,
-                access_hash=voice.access_hash,
-                file_reference=voice.file_reference
-            ).encode(),
-            file_unique_id=FileUniqueId(
-                file_unique_type=FileUniqueType.DOCUMENT,
-                media_id=voice.id
-            ).encode(),
-            duration=attributes.duration,
-            mime_type=voice.mime_type,
-            file_size=voice.size,
-            waveform=attributes.waveform,
-            date=utils.timestamp_to_datetime(voice.date),
+    def _parse(
+        client: "pyrogram.Client",
+        joiner: "raw.base.ChatInviteImporter",
+        users: Dict[int, "raw.base.User"],
+    ) -> "ChatJoiner":
+        return ChatJoiner(
+            user=types.User._parse(client, users[joiner.user_id]),
+            date=utils.timestamp_to_datetime(joiner.date),
+            pending=joiner.requested,
+            bio=joiner.about,
+            approved_by=(
+                types.User._parse(client, users[joiner.approved_by])
+                if joiner.approved_by
+                else None
+            ),
             client=client
         )
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/object.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/update.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,23 @@
         if isinstance(chat, (raw.types.Chat, raw.types.ChatForbidden)):
             return Chat._parse_chat_chat(client, chat)
         elif isinstance(chat, raw.types.User):
             return Chat._parse_user_chat(client, chat)
         else:
             return Chat._parse_channel_chat(client, chat)
 
+    def listen(self, *args, **kwargs):
+        return self._client.listen(self.id, *args, **kwargs)
+
+    def ask(self, *args, **kwargs):
+        return self._client.ask(self.id, *args, **kwargs)
+
+    def cancel_listener(self):
+        return self._client.cancel_listener(self.id)
+
     async def archive(self):
         """Bound method *archive* of :obj:`~pyrogram.types.Chat`.
 
         Use as a shortcut for:
 
         .. code-block:: python
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/user.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,23 @@
     def _parse_user_status(client, user_status: "raw.types.UpdateUserStatus"):
         return User(
             id=user_status.user_id,
             **User._parse_status(user_status.status),
             client=client
         )
 
+    def listen(self, *args, **kwargs):
+        return self._client.listen(self.id, *args, **kwargs)
+
+    def ask(self, *args, **kwargs):
+        return self._client.ask(self.id, *args, **kwargs)
+
+    def cancel_listener(self):
+        return self._client.cancel_listener(self.id)
+
     async def archive(self):
         """Bound method *archive* of :obj:`~pyrogram.types.User`.
 
         Use as a shortcut for:
 
         .. code-block:: python
```

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/username.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/types/user_and_chats/video_chat_started.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/pyrogram/utils.py` & `PyroFork-dev-2.1.5a1.dev202304141812/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/setup.py` & `PyroFork-dev-2.1.5a1.dev202304141812/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/filters/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/filters/test_command.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/parser/__init__.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/parser/test_html.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.1.5.dev202304141749/tests/test_file_id.py` & `PyroFork-dev-2.1.5a1.dev202304141812/tests/test_file_id.py`

 * *Files identical despite different names*

