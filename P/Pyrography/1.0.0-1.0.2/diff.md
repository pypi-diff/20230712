# Comparing `tmp/Pyrography-1.0.0.tar.gz` & `tmp/Pyrography-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyrography-1.0.0.tar", last modified: Wed Jun 28 18:14:11 2023, max compression
+gzip compressed data, was "Pyrography-1.0.2.tar", last modified: Wed Jul 12 06:12:45 2023, max compression
```

## Comparing `Pyrography-1.0.0.tar` & `Pyrography-1.0.2.tar`

### file list

```diff
@@ -1,494 +1,494 @@
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.642978 Pyrography-1.0.0/
--rw-r--r--   0 lelzin    (1000) users      (985)    35148 2023-06-25 15:16:49.000000 Pyrography-1.0.0/COPYING
--rw-r--r--   0 lelzin    (1000) users      (985)     7651 2023-06-25 15:16:49.000000 Pyrography-1.0.0/COPYING.lesser
--rw-r--r--   0 lelzin    (1000) users      (985)      305 2023-06-25 15:16:49.000000 Pyrography-1.0.0/MANIFEST.in
--rw-r--r--   0 lelzin    (1000) users      (985)      949 2023-06-28 17:44:57.000000 Pyrography-1.0.0/NOTICE
--rw-r--r--   0 lelzin    (1000) users      (985)     6230 2023-06-28 18:14:11.642978 Pyrography-1.0.0/PKG-INFO
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/Pyrography.egg-info/
--rw-r--r--   0 lelzin    (1000) users      (985)     6230 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/PKG-INFO
--rw-r--r--   0 lelzin    (1000) users      (985)    19638 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/SOURCES.txt
--rw-r--r--   0 lelzin    (1000) users      (985)        1 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/dependency_links.txt
--rw-r--r--   0 lelzin    (1000) users      (985)        1 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/not-zip-safe
--rw-r--r--   0 lelzin    (1000) users      (985)       57 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/requires.txt
--rw-r--r--   0 lelzin    (1000) users      (985)       11 2023-06-28 18:14:11.000000 Pyrography-1.0.0/Pyrography.egg-info/top_level.txt
--rw-r--r--   0 lelzin    (1000) users      (985)     4339 2023-06-28 17:44:14.000000 Pyrography-1.0.0/README.md
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/compiler/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.0/compiler/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/compiler/api/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.0/compiler/api/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)    22578 2023-06-28 17:44:58.000000 Pyrography-1.0.0/compiler/api/compiler.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/compiler/api/source/
--rw-r--r--   0 lelzin    (1000) users      (985)     2233 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/api/source/auth_key.tl
--rw-r--r--   0 lelzin    (1000) users      (985)   168867 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/api/source/main_api.tl
--rw-r--r--   0 lelzin    (1000) users      (985)     3425 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/compiler/api/template/
--rw-r--r--   0 lelzin    (1000) users      (985)      749 2023-06-28 17:44:58.000000 Pyrography-1.0.0/compiler/api/template/combinator.txt
--rw-r--r--   0 lelzin    (1000) users      (985)      641 2023-06-28 17:44:58.000000 Pyrography-1.0.0/compiler/api/template/type.txt
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.519645 Pyrography-1.0.0/compiler/docs/
--rw-r--r--   0 lelzin    (1000) users      (985)      818 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/docs/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)    19250 2023-06-28 17:44:58.000000 Pyrography-1.0.0/compiler/docs/compiler.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.536311 Pyrography-1.0.0/compiler/docs/template/
--rw-r--r--   0 lelzin    (1000) users      (985)       73 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/docs/template/page.txt
--rw-r--r--   0 lelzin    (1000) users      (985)       91 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.539645 Pyrography-1.0.0/compiler/errors/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.0/compiler/errors/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5061 2023-06-28 17:44:58.000000 Pyrography-1.0.0/compiler/errors/compiler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1403 2023-06-28 17:44:57.000000 Pyrography-1.0.0/compiler/errors/sort.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.542978 Pyrography-1.0.0/compiler/errors/source/
--rw-r--r--   0 lelzin    (1000) users      (985)      470 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)    22642 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)      678 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)     2000 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)     1177 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)      470 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)     4219 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 lelzin    (1000) users      (985)      155 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.546311 Pyrography-1.0.0/compiler/errors/template/
--rw-r--r--   0 lelzin    (1000) users      (985)      178 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/template/class.txt
--rw-r--r--   0 lelzin    (1000) users      (985)      120 2023-06-25 15:16:49.000000 Pyrography-1.0.0/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.549645 Pyrography-1.0.0/pyrography/
--rw-r--r--   0 lelzin    (1000) users      (985)     1796 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)    42533 2023-06-28 17:45:00.000000 Pyrography-1.0.0/pyrography/client.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.549645 Pyrography-1.0.0/pyrography/connection/
--rw-r--r--   0 lelzin    (1000) users      (985)      994 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2682 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/connection.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.549645 Pyrography-1.0.0/pyrography/connection/transport/
--rw-r--r--   0 lelzin    (1000) users      (985)      978 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.552978 Pyrography-1.0.0/pyrography/connection/transport/tcp/
--rw-r--r--   0 lelzin    (1000) users      (985)     1184 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4229 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1908 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2978 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2046 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1651 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2595 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.552978 Pyrography-1.0.0/pyrography/crypto/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/crypto/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4153 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/crypto/aes.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4162 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/crypto/mtproto.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2586 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/crypto/prime.py
--rw-r--r--   0 lelzin    (1000) users      (985)    13577 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/crypto/rsa.py
--rw-r--r--   0 lelzin    (1000) users      (985)    12151 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/dispatcher.py
--rw-r--r--   0 lelzin    (1000) users      (985)   208161 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/emoji.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.556311 Pyrography-1.0.0/pyrography/enums/
--rw-r--r--   0 lelzin    (1000) users      (985)     1876 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1144 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/auto_name.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2451 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/chat_action.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4345 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/chat_event_action.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1407 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/chat_member_status.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1590 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/chat_members_filter.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1380 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/chat_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2608 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/message_entity_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1741 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/message_media_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2042 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/message_service_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2552 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/messages_filter.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1665 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/next_code_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1328 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/parse_mode.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1189 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/poll_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1867 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/sent_code_type.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1441 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/enums/user_status.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.559645 Pyrography-1.0.0/pyrography/errors/
--rw-r--r--   0 lelzin    (1000) users      (985)     2745 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/errors/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3463 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/errors/rpc_error.py
--rw-r--r--   0 lelzin    (1000) users      (985)    15296 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/file_id.py
--rw-r--r--   0 lelzin    (1000) users      (985)    26783 2023-06-28 17:45:00.000000 Pyrography-1.0.0/pyrography/filters.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.562978 Pyrography-1.0.0/pyrography/handlers/
--rw-r--r--   0 lelzin    (1000) users      (985)     1615 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2174 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/callback_query_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2159 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/chat_join_request_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2194 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/chat_member_updated_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2249 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2699 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/deleted_messages_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1848 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/disconnect_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2127 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/edited_message_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1698 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2132 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/inline_query_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2083 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/message_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2062 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/poll_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3104 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/raw_update_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2137 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/handlers/user_status_handler.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.562978 Pyrography-1.0.0/pyrography/methods/
--rw-r--r--   0 lelzin    (1000) users      (985)     1460 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.562978 Pyrography-1.0.0/pyrography/methods/advanced/
--rw-r--r--   0 lelzin    (1000) users      (985)     1128 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/advanced/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3289 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/advanced/invoke.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4712 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/advanced/resolve_peer.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8573 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/advanced/save_file.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.566311 Pyrography-1.0.0/pyrography/methods/auth/
--rw-r--r--   0 lelzin    (1000) users      (985)     1795 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1614 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2094 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/check_password.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1895 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/connect.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1648 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/disconnect.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1453 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/get_password_hint.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1906 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/initialize.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1772 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/log_out.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1981 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/recover_password.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2302 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/resend_code.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2940 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/send_code.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1619 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/send_recovery_code.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3241 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/sign_in.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2877 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/sign_in_bot.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2507 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/sign_up.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2190 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/auth/terminate.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.569645 Pyrography-1.0.0/pyrography/methods/bots/
--rw-r--r--   0 lelzin    (1000) users      (985)     2181 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3457 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/answer_callback_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5142 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/answer_inline_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2141 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/answer_web_app_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2510 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/delete_bot_commands.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2725 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/get_bot_commands.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2199 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2467 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2948 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/get_game_high_scores.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3517 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2993 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/request_callback_answer.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4108 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/send_game.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2976 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2866 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/set_bot_commands.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3338 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2200 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4096 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/bots/set_game_score.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.579645 Pyrography-1.0.0/pyrography/methods/chats/
--rw-r--r--   0 lelzin    (1000) users      (985)     3579 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3510 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/add_chat_members.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2362 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/archive_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4770 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/ban_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1967 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/create_channel.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2433 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/create_group.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2107 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/create_supergroup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1731 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/delete_channel.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2453 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/delete_chat_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1749 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/delete_supergroup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2115 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/delete_user_history.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3436 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4184 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat_event_log.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3490 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5442 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat_members.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2410 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat_members_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1869 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_chat_online_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3508 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_dialogs.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2242 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_dialogs_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2553 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_nearby_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2286 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/get_send_as_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2844 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/join_chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2751 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/leave_chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1674 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/mark_chat_unread.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3305 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/pin_chat_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4009 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/promote_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4466 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/restrict_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3282 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_administrator_title.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2393 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_description.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3569 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_permissions.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4755 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1873 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2718 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_title.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2444 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_chat_username.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2130 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_send_as_chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2229 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/set_slow_mode.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2376 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/unarchive_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2451 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/unban_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2086 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2285 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.579645 Pyrography-1.0.0/pyrography/methods/contacts/
--rw-r--r--   0 lelzin    (1000) users      (985)     1294 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2716 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/add_contact.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2598 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/delete_contacts.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1755 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/get_contacts.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1568 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/get_contacts_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2086 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/contacts/import_contacts.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.586311 Pyrography-1.0.0/pyrography/methods/decorators/
--rw-r--r--   0 lelzin    (1000) users      (985)     1764 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2337 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_callback_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2325 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2346 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2373 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2339 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1705 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_disconnect.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2328 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_edited_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2323 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_inline_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2294 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2276 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_poll.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1970 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_raw_update.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2310 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/decorators/on_user_status.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.589645 Pyrography-1.0.0/pyrography/methods/invite_links/
--rw-r--r--   0 lelzin    (1000) users      (985)     2575 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2040 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2070 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3521 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2041 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2071 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2177 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1897 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3683 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2732 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3718 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2481 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2145 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2075 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3080 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2075 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3099 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2479 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.602978 Pyrography-1.0.0/pyrography/methods/messages/
--rw-r--r--   0 lelzin    (1000) users      (985)     4104 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/methods/messages/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     6111 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/copy_media_group.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5339 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/copy_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3294 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/delete_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     7682 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/download_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2421 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_inline_caption.py
--rw-r--r--   0 lelzin    (1000) users      (985)    10535 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_inline_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2618 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3269 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_inline_text.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3132 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_message_caption.py
--rw-r--r--   0 lelzin    (1000) users      (985)    13182 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_message_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3130 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4064 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/edit_message_text.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4716 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/forward_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4191 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_chat_history.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2535 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_chat_history_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2132 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2377 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_discussion_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2954 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_discussion_replies.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2096 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3094 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_media_group.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4895 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/get_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2327 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/inline_session.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2673 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/read_chat_history.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2274 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/retract_vote.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4318 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/search_global.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2306 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/search_global_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5503 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/search_messages.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3353 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/search_messages_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)    12756 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_animation.py
--rw-r--r--   0 lelzin    (1000) users      (985)    11292 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_audio.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5643 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_cached_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2967 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_chat_action.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5025 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_contact.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4999 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_dice.py
--rw-r--r--   0 lelzin    (1000) users      (985)    10640 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_document.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4734 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_location.py
--rw-r--r--   0 lelzin    (1000) users      (985)    20070 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_media_group.py
--rw-r--r--   0 lelzin    (1000) users      (985)     7429 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     9610 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8241 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_poll.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2507 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_reaction.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8506 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_sticker.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5555 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_venue.py
--rw-r--r--   0 lelzin    (1000) users      (985)    12126 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_video.py
--rw-r--r--   0 lelzin    (1000) users      (985)     9480 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_video_note.py
--rw-r--r--   0 lelzin    (1000) users      (985)     9600 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/send_voice.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2971 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/stop_poll.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4087 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/stream_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2654 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/messages/vote_poll.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3249 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/methods/messages/wait_for.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.602978 Pyrography-1.0.0/pyrography/methods/password/
--rw-r--r--   0 lelzin    (1000) users      (985)     1228 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/password/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2945 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/password/change_cloud_password.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3154 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/password/enable_cloud_password.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2291 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.606311 Pyrography-1.0.0/pyrography/methods/users/
--rw-r--r--   0 lelzin    (1000) users      (985)     1799 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1917 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/block_user.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2389 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/delete_profile_photos.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4569 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_chat_photos.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2655 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_chat_photos_count.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2509 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_common_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1814 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1715 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_me.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2714 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/get_users.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2032 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/set_emoji_status.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2864 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/set_profile_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2024 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/set_username.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1927 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/unblock_user.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2522 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/users/update_profile.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.609645 Pyrography-1.0.0/pyrography/methods/utilities/
--rw-r--r--   0 lelzin    (1000) users      (985)     1393 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2498 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/add_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2382 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/compose.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1701 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/export_session_string.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4406 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/methods/utilities/idle.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2364 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/remove_handler.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2446 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/restart.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3015 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/run.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2514 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/start.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2265 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/stop.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1854 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/methods/utilities/stop_transmission.py
--rw-r--r--   0 lelzin    (1000) users      (985)    62055 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/mime_types.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.609645 Pyrography-1.0.0/pyrography/parser/
--rw-r--r--   0 lelzin    (1000) users      (985)      986 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/parser/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8836 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/parser/html.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5916 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/parser/markdown.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2223 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/parser/parser.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1685 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/parser/utils.py
--rw-r--r--   0 lelzin    (1000) users      (985)        0 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/py.typed
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.609645 Pyrography-1.0.0/pyrography/raw/
--rw-r--r--   0 lelzin    (1000) users      (985)     1180 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.612978 Pyrography-1.0.0/pyrography/raw/core/
--rw-r--r--   0 lelzin    (1000) users      (985)     1452 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1832 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/future_salt.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2031 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/future_salts.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1954 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/gzip_packed.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1190 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/list.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1991 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1754 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/msg_container.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.612978 Pyrography-1.0.0/pyrography/raw/core/primitives/
--rw-r--r--   0 lelzin    (1000) users      (985)     1152 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1637 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/bool.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1899 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/bytes.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1333 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/double.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1498 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/int.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1334 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/string.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2162 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/primitives/vector.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2637 2023-06-28 17:44:58.000000 Pyrography-1.0.0/pyrography/raw/core/tl_object.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.612978 Pyrography-1.0.0/pyrography/session/
--rw-r--r--   0 lelzin    (1000) users      (985)     1011 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)    11600 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/auth.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.616311 Pyrography-1.0.0/pyrography/session/internals/
--rw-r--r--   0 lelzin    (1000) users      (985)     1057 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/internals/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2592 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/internals/data_center.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1520 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/internals/msg_factory.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1296 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/internals/msg_id.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1302 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/internals/seq_no.py
--rw-r--r--   0 lelzin    (1000) users      (985)    13579 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/session/session.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.616311 Pyrography-1.0.0/pyrography/storage/
--rw-r--r--   0 lelzin    (1000) users      (985)     1068 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/storage/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2099 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/storage/file_storage.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2890 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/storage/memory_storage.py
--rw-r--r--   0 lelzin    (1000) users      (985)     6366 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/storage/sqlite_storage.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2921 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/storage/storage.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3885 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/sync.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.616311 Pyrography-1.0.0/pyrography/types/
--rw-r--r--   0 lelzin    (1000) users      (985)     1249 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.616311 Pyrography-1.0.0/pyrography/types/authorization/
--rw-r--r--   0 lelzin    (1000) users      (985)     1078 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/authorization/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2442 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/authorization/sent_code.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2078 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/authorization/terms_of_service.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.622978 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/
--rw-r--r--   0 lelzin    (1000) users      (985)     2970 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1880 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2948 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1439 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1404 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1395 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1708 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1785 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1963 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1454 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1169 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 lelzin    (1000) users      (985)    12985 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2529 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2366 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8276 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2610 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3658 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3854 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1757 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1355 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1358 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1959 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4725 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2485 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1706 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1453 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.629644 Pyrography-1.0.0/pyrography/types/inline_mode/
--rw-r--r--   0 lelzin    (1000) users      (985)     2895 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3814 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 lelzin    (1000) users      (985)     7458 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2591 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5930 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3456 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4659 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4399 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4183 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4542 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4466 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3181 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4548 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4356 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4282 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5394 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4769 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5415 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4904 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5628 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4514 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.629644 Pyrography-1.0.0/pyrography/types/input_media/
--rw-r--r--   0 lelzin    (1000) users      (985)     1454 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1788 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3572 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media_animation.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3428 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media_audio.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2915 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media_document.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2831 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3766 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_media_video.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1883 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.632978 Pyrography-1.0.0/pyrography/types/input_message_content/
--rw-r--r--   0 lelzin    (1000) users      (985)     1146 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_message_content/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1565 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_message_content/input_message_content.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2788 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1235 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/list.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.636311 Pyrography-1.0.0/pyrography/types/messages_and_media/
--rw-r--r--   0 lelzin    (1000) users      (985)     1976 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4196 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/animation.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4221 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/audio.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2355 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/contact.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1733 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/dice.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3561 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/document.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3196 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/game.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1806 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/location.py
--rw-r--r--   0 lelzin    (1000) users      (985)   150975 2023-06-28 17:45:01.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/message.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4512 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/message_entity.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1950 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/message_reactions.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4461 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     7191 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/poll.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1676 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/poll_option.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2767 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/reaction.py
--rw-r--r--   0 lelzin    (1000) users      (985)     7063 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/sticker.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1577 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3903 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/thumbnail.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2441 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/venue.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4541 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/video.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3753 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/video_note.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3352 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/voice.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1707 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/web_app_data.py
--rw-r--r--   0 lelzin    (1000) users      (985)     6509 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/messages_and_media/web_page.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4012 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/object.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1148 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/update.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.642978 Pyrography-1.0.0/pyrography/types/user_and_chats/
--rw-r--r--   0 lelzin    (1000) users      (985)     2437 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)    32809 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2386 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 lelzin    (1000) users      (985)    20059 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_event.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5656 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4729 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4405 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2716 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 lelzin    (1000) users      (985)     9608 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_member.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3834 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4524 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 lelzin    (1000) users      (985)     4115 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_photo.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2744 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_preview.py
--rw-r--r--   0 lelzin    (1000) users      (985)     5093 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2504 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2834 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/dialog.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2570 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/emoji_status.py
--rw-r--r--   0 lelzin    (1000) users      (985)     2097 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1805 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/restriction.py
--rw-r--r--   0 lelzin    (1000) users      (985)    13008 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/user.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1488 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1754 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1673 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 lelzin    (1000) users      (985)     1183 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 lelzin    (1000) users      (985)    10722 2023-06-28 17:44:59.000000 Pyrography-1.0.0/pyrography/utils.py
--rw-r--r--   0 lelzin    (1000) users      (985)       56 2023-06-28 17:45:00.000000 Pyrography-1.0.0/requirements.txt
--rw-r--r--   0 lelzin    (1000) users      (985)       38 2023-06-28 18:14:11.642978 Pyrography-1.0.0/setup.cfg
--rw-r--r--   0 lelzin    (1000) users      (985)     3720 2023-06-28 17:44:59.000000 Pyrography-1.0.0/setup.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.642978 Pyrography-1.0.0/tests/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.0/tests/__init__.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.642978 Pyrography-1.0.0/tests/filters/
--rw-r--r--   0 lelzin    (1000) users      (985)     1341 2023-06-28 17:44:58.000000 Pyrography-1.0.0/tests/filters/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     3514 2023-06-28 17:44:59.000000 Pyrography-1.0.0/tests/filters/test_command.py
-drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-06-28 18:14:11.642978 Pyrography-1.0.0/tests/parser/
--rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.0/tests/parser/__init__.py
--rw-r--r--   0 lelzin    (1000) users      (985)     6518 2023-06-28 17:44:59.000000 Pyrography-1.0.0/tests/parser/test_html.py
--rw-r--r--   0 lelzin    (1000) users      (985)     8350 2023-06-28 17:44:59.000000 Pyrography-1.0.0/tests/test_file_id.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.645255 Pyrography-1.0.2/
+-rw-r--r--   0 lelzin    (1000) users      (985)    35148 2023-06-25 15:16:49.000000 Pyrography-1.0.2/COPYING
+-rw-r--r--   0 lelzin    (1000) users      (985)     7651 2023-06-25 15:16:49.000000 Pyrography-1.0.2/COPYING.lesser
+-rw-r--r--   0 lelzin    (1000) users      (985)      305 2023-06-25 15:16:49.000000 Pyrography-1.0.2/MANIFEST.in
+-rw-r--r--   0 lelzin    (1000) users      (985)      949 2023-06-28 17:44:57.000000 Pyrography-1.0.2/NOTICE
+-rw-r--r--   0 lelzin    (1000) users      (985)     5657 2023-07-12 06:12:45.645255 Pyrography-1.0.2/PKG-INFO
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.408588 Pyrography-1.0.2/Pyrography.egg-info/
+-rw-r--r--   0 lelzin    (1000) users      (985)     5657 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/PKG-INFO
+-rw-r--r--   0 lelzin    (1000) users      (985)    19638 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/SOURCES.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)        1 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/dependency_links.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)        1 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/not-zip-safe
+-rw-r--r--   0 lelzin    (1000) users      (985)       57 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/requires.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)       11 2023-07-12 06:12:45.000000 Pyrography-1.0.2/Pyrography.egg-info/top_level.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)     3766 2023-07-12 05:49:26.000000 Pyrography-1.0.2/README.md
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.411921 Pyrography-1.0.2/compiler/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.2/compiler/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.411921 Pyrography-1.0.2/compiler/api/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.2/compiler/api/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    22578 2023-06-28 17:44:58.000000 Pyrography-1.0.2/compiler/api/compiler.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.411921 Pyrography-1.0.2/compiler/api/source/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2233 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/api/source/auth_key.tl
+-rw-r--r--   0 lelzin    (1000) users      (985)   168867 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/api/source/main_api.tl
+-rw-r--r--   0 lelzin    (1000) users      (985)     3425 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.411921 Pyrography-1.0.2/compiler/api/template/
+-rw-r--r--   0 lelzin    (1000) users      (985)      749 2023-06-28 17:44:58.000000 Pyrography-1.0.2/compiler/api/template/combinator.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)      641 2023-06-28 17:44:58.000000 Pyrography-1.0.2/compiler/api/template/type.txt
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.431921 Pyrography-1.0.2/compiler/docs/
+-rw-r--r--   0 lelzin    (1000) users      (985)      957 2023-07-02 17:03:56.000000 Pyrography-1.0.2/compiler/docs/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    19488 2023-07-02 17:04:08.000000 Pyrography-1.0.2/compiler/docs/compiler.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.465255 Pyrography-1.0.2/compiler/docs/template/
+-rw-r--r--   0 lelzin    (1000) users      (985)       73 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/docs/template/page.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)       91 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.468588 Pyrography-1.0.2/compiler/errors/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:57.000000 Pyrography-1.0.2/compiler/errors/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5061 2023-06-28 17:44:58.000000 Pyrography-1.0.2/compiler/errors/compiler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1403 2023-06-28 17:44:57.000000 Pyrography-1.0.2/compiler/errors/sort.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.475255 Pyrography-1.0.2/compiler/errors/source/
+-rw-r--r--   0 lelzin    (1000) users      (985)      470 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)    22642 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)      678 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)     2000 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)     1177 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)      470 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)     4219 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 lelzin    (1000) users      (985)      155 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.475255 Pyrography-1.0.2/compiler/errors/template/
+-rw-r--r--   0 lelzin    (1000) users      (985)      178 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/template/class.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)      120 2023-06-25 15:16:49.000000 Pyrography-1.0.2/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.488588 Pyrography-1.0.2/pyrography/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1796 2023-07-12 05:49:26.000000 Pyrography-1.0.2/pyrography/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    42533 2023-06-28 17:45:00.000000 Pyrography-1.0.2/pyrography/client.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.488588 Pyrography-1.0.2/pyrography/connection/
+-rw-r--r--   0 lelzin    (1000) users      (985)      994 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2682 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/connection.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.488588 Pyrography-1.0.2/pyrography/connection/transport/
+-rw-r--r--   0 lelzin    (1000) users      (985)      978 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.491922 Pyrography-1.0.2/pyrography/connection/transport/tcp/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1184 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4229 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1908 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2978 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2046 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1651 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2595 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.495255 Pyrography-1.0.2/pyrography/crypto/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/crypto/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4153 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/crypto/aes.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4162 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/crypto/mtproto.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2586 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/crypto/prime.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    13577 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/crypto/rsa.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    12151 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/dispatcher.py
+-rw-r--r--   0 lelzin    (1000) users      (985)   208161 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/emoji.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.498588 Pyrography-1.0.2/pyrography/enums/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1876 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1144 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/auto_name.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2451 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/chat_action.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4345 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/chat_event_action.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1407 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/chat_member_status.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1590 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/chat_members_filter.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1380 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/chat_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2608 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/message_entity_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1741 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/message_media_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2042 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/message_service_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2552 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/messages_filter.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1665 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/next_code_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1328 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/parse_mode.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1189 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/poll_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1867 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/sent_code_type.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1441 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/enums/user_status.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.498588 Pyrography-1.0.2/pyrography/errors/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2745 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/errors/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3463 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/errors/rpc_error.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    15296 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/file_id.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    26783 2023-06-28 17:45:00.000000 Pyrography-1.0.2/pyrography/filters.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.505255 Pyrography-1.0.2/pyrography/handlers/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1615 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2174 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/callback_query_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2159 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/chat_join_request_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2194 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2249 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2699 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/deleted_messages_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1848 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/disconnect_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2127 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/edited_message_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1698 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2132 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/inline_query_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2083 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/message_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2062 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/poll_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3104 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/raw_update_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2137 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/handlers/user_status_handler.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.505255 Pyrography-1.0.2/pyrography/methods/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1460 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.505255 Pyrography-1.0.2/pyrography/methods/advanced/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1128 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/advanced/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3289 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/advanced/invoke.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4712 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/advanced/resolve_peer.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8573 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/advanced/save_file.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.511922 Pyrography-1.0.2/pyrography/methods/auth/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1795 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1614 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2094 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/check_password.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1895 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/connect.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1648 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/disconnect.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1453 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/get_password_hint.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1906 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/initialize.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1772 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/log_out.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1981 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/recover_password.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2302 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/resend_code.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2940 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/send_code.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1619 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/send_recovery_code.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3241 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/sign_in.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2877 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/sign_in_bot.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2507 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/sign_up.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2190 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/auth/terminate.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.515255 Pyrography-1.0.2/pyrography/methods/bots/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2181 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3457 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/answer_callback_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5142 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/answer_inline_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2141 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2510 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2725 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/get_bot_commands.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2199 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2467 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2948 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3517 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2993 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/request_callback_answer.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4108 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/send_game.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2976 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2866 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/set_bot_commands.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3338 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2200 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4096 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/bots/set_game_score.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.528588 Pyrography-1.0.2/pyrography/methods/chats/
+-rw-r--r--   0 lelzin    (1000) users      (985)     3579 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3510 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/add_chat_members.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2362 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/archive_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4770 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/ban_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1967 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/create_channel.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2433 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/create_group.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2107 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/create_supergroup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1731 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/delete_channel.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2453 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1749 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/delete_supergroup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2115 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/delete_user_history.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3436 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4184 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3490 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5442 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat_members.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2410 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1869 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3508 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_dialogs.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2242 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2553 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2286 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2844 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/join_chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2751 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/leave_chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1674 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3305 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/pin_chat_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4009 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/promote_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4466 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3282 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_administrator_title.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2393 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_description.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3569 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4755 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1873 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2718 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_title.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2444 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_chat_username.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2130 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2229 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/set_slow_mode.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2376 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/unarchive_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2451 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/unban_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2086 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2285 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.528588 Pyrography-1.0.2/pyrography/methods/contacts/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1294 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2716 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/add_contact.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2598 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/delete_contacts.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1755 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/get_contacts.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1568 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2086 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/contacts/import_contacts.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.531922 Pyrography-1.0.2/pyrography/methods/decorators/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1764 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2337 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_callback_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2325 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2346 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2373 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2339 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1705 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_disconnect.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2328 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_edited_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2323 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_inline_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2294 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2276 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_poll.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1970 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_raw_update.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2310 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/decorators/on_user_status.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.538588 Pyrography-1.0.2/pyrography/methods/invite_links/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2575 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2040 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2070 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3521 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2041 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2071 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2177 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1897 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3683 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2732 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3718 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2481 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2145 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2075 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3080 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2075 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3099 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2479 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.551922 Pyrography-1.0.2/pyrography/methods/messages/
+-rw-r--r--   0 lelzin    (1000) users      (985)     4104 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/methods/messages/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     6111 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/copy_media_group.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5339 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/copy_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3294 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/delete_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     7682 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/download_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2421 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    10535 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_inline_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2618 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3269 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_inline_text.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3132 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_message_caption.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    13182 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_message_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3130 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4064 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/edit_message_text.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4716 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/forward_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4191 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_chat_history.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2535 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2132 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2377 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_discussion_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2954 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2096 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3094 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_media_group.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4895 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/get_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2327 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/inline_session.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2673 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/read_chat_history.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2274 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/retract_vote.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4318 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/search_global.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2306 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/search_global_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5503 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/search_messages.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3353 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/search_messages_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    12756 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_animation.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    11292 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_audio.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5643 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_cached_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2967 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_chat_action.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5025 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_contact.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4999 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_dice.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    10640 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_document.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4734 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_location.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    20070 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_media_group.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     7429 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     9610 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8241 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_poll.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2507 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_reaction.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8506 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_sticker.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5555 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_venue.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    12126 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_video.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     9480 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_video_note.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     9600 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/send_voice.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2971 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/stop_poll.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4087 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/stream_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2654 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/messages/vote_poll.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3249 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/methods/messages/wait_for.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.555255 Pyrography-1.0.2/pyrography/methods/password/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1228 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/password/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2945 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/password/change_cloud_password.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3154 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/password/enable_cloud_password.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2291 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.561922 Pyrography-1.0.2/pyrography/methods/users/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1799 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1917 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/block_user.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2389 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/delete_profile_photos.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4569 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_chat_photos.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2655 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2509 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_common_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1814 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1715 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_me.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2714 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/get_users.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2032 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/set_emoji_status.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2864 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/set_profile_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2024 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/set_username.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1927 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/unblock_user.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2522 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/users/update_profile.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.565255 Pyrography-1.0.2/pyrography/methods/utilities/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1393 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2498 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/add_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2382 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/compose.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1701 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/export_session_string.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4406 2023-07-07 06:20:25.000000 Pyrography-1.0.2/pyrography/methods/utilities/idle.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2364 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/remove_handler.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2446 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/restart.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3228 2023-07-12 05:49:26.000000 Pyrography-1.0.2/pyrography/methods/utilities/run.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2514 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/start.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2265 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/stop.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1854 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/methods/utilities/stop_transmission.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    62055 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/mime_types.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.565255 Pyrography-1.0.2/pyrography/parser/
+-rw-r--r--   0 lelzin    (1000) users      (985)      986 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/parser/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8836 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/parser/html.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5916 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/parser/markdown.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2223 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/parser/parser.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1685 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/parser/utils.py
+-rw-r--r--   0 lelzin    (1000) users      (985)        0 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/py.typed
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.565255 Pyrography-1.0.2/pyrography/raw/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1180 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.568589 Pyrography-1.0.2/pyrography/raw/core/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1452 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1832 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/future_salt.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2031 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/future_salts.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1954 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/gzip_packed.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1190 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/list.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1991 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1754 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/msg_container.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.568589 Pyrography-1.0.2/pyrography/raw/core/primitives/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1152 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1637 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/bool.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1899 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/bytes.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1333 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/double.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1498 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/int.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1334 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/string.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2162 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/primitives/vector.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2637 2023-06-28 17:44:58.000000 Pyrography-1.0.2/pyrography/raw/core/tl_object.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.571922 Pyrography-1.0.2/pyrography/session/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1011 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    11600 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/auth.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.571922 Pyrography-1.0.2/pyrography/session/internals/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1057 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/internals/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2592 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/internals/data_center.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1520 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/internals/msg_factory.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1296 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/internals/msg_id.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1302 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/internals/seq_no.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    13579 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/session/session.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.575255 Pyrography-1.0.2/pyrography/storage/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1068 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/storage/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2099 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/storage/file_storage.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2890 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/storage/memory_storage.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     6366 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/storage/sqlite_storage.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2921 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/storage/storage.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3885 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/sync.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.578589 Pyrography-1.0.2/pyrography/types/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1249 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.581922 Pyrography-1.0.2/pyrography/types/authorization/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1078 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/authorization/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2442 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/authorization/sent_code.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2078 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/authorization/terms_of_service.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.601922 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2970 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1880 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2948 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1439 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1404 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1395 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1708 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1785 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1963 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1454 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1169 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    12985 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2529 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2366 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8276 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2610 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3658 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3854 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1757 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1355 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1358 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1959 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4725 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2485 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1706 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1453 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.618589 Pyrography-1.0.2/pyrography/types/inline_mode/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2895 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3814 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     7458 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2591 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5930 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3456 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4659 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4399 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4183 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4542 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4466 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3181 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4548 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4356 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4282 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5394 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4769 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5415 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4904 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5628 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4514 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.621922 Pyrography-1.0.2/pyrography/types/input_media/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1454 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1788 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3572 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media_animation.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3428 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media_audio.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2915 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media_document.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2831 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3766 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_media_video.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1883 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.621922 Pyrography-1.0.2/pyrography/types/input_message_content/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1146 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_message_content/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1565 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_message_content/input_message_content.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2788 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1235 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/list.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.628589 Pyrography-1.0.2/pyrography/types/messages_and_media/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1976 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4196 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/animation.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4221 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/audio.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2355 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/contact.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1733 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/dice.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3561 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/document.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3196 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/game.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1806 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/location.py
+-rw-r--r--   0 lelzin    (1000) users      (985)   150975 2023-06-28 17:45:01.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/message.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4512 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/message_entity.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1950 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4461 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     7191 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/poll.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1676 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/poll_option.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2767 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/reaction.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     7063 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/sticker.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1577 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3903 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2441 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/venue.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4541 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/video.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3753 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/video_note.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3352 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/voice.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1707 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     6509 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/messages_and_media/web_page.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4012 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/object.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1148 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/update.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.641922 Pyrography-1.0.2/pyrography/types/user_and_chats/
+-rw-r--r--   0 lelzin    (1000) users      (985)     2437 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    32809 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2386 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    20059 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_event.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5656 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4729 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4405 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2716 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     9608 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_member.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3834 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4524 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     4115 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2744 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     5093 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2504 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2834 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/dialog.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2570 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     2097 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1805 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/restriction.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    13008 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/user.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1488 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1754 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1673 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     1183 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 lelzin    (1000) users      (985)    10722 2023-06-28 17:44:59.000000 Pyrography-1.0.2/pyrography/utils.py
+-rw-r--r--   0 lelzin    (1000) users      (985)       56 2023-06-28 17:45:00.000000 Pyrography-1.0.2/requirements.txt
+-rw-r--r--   0 lelzin    (1000) users      (985)       38 2023-07-12 06:12:45.645255 Pyrography-1.0.2/setup.cfg
+-rw-r--r--   0 lelzin    (1000) users      (985)     3720 2023-06-28 17:44:59.000000 Pyrography-1.0.2/setup.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.641922 Pyrography-1.0.2/tests/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.2/tests/__init__.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.645255 Pyrography-1.0.2/tests/filters/
+-rw-r--r--   0 lelzin    (1000) users      (985)     1341 2023-06-28 17:44:58.000000 Pyrography-1.0.2/tests/filters/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     3514 2023-06-28 17:44:59.000000 Pyrography-1.0.2/tests/filters/test_command.py
+drwxr-xr-x   0 lelzin    (1000) users      (985)        0 2023-07-12 06:12:45.645255 Pyrography-1.0.2/tests/parser/
+-rw-r--r--   0 lelzin    (1000) users      (985)      958 2023-06-28 17:44:58.000000 Pyrography-1.0.2/tests/parser/__init__.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     6518 2023-06-28 17:44:59.000000 Pyrography-1.0.2/tests/parser/test_html.py
+-rw-r--r--   0 lelzin    (1000) users      (985)     8350 2023-06-28 17:44:59.000000 Pyrography-1.0.2/tests/test_file_id.py
```

### Comparing `Pyrography-1.0.0/COPYING` & `Pyrography-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/COPYING.lesser` & `Pyrography-1.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/NOTICE` & `Pyrography-1.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/PKG-INFO` & `Pyrography-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyrography
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram.
 Home-page: https://github.com/d3cryptofc/pyrography
 Download-URL: https://github.com/d3cryptofc/pyrography/releases/latest
 Author: Lelzin λ
 Author-email: d3cryptofc@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/d3cryptofc/pyrography/issues
@@ -43,139 +43,103 @@
     <a href="https://github.com/pyrogram/pyrogram">
         <img src="https://github.com/d3cryptofc/pyrography/assets/47941854/0eb90a78-5054-497e-8c86-b5f6bbb70822" alt="Pyrogram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br/>A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram
     <br>
-    <a href="https://pyrogram.org">
-        Homepage
-    </a>
-    •
-    <a href="https://docs.pyrogram.org">
-        Documentation
-    </a>
-    •
-    <a href="https://docs.pyrogram.org/releases">
+    <a href="https://github.com/d3cryptofc/pyrography/releases">
         Releases
     </a>
     •
-    <a href="https://t.me/pyrogram">
+    <a href="https://t.me/forkpyrography">
         News
     </a>
 </p>
 
 ## Pyrography
 
 > Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 
 ```python3
-import asyncio
-from pyrography import Client, filters, idle
+from pyrography import Client, filters
+
 
 # Creating a client instance to control your bot.
-# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org
+# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org.
+# (optional `bot_token` parameter)
 client = Client(
     name='your_session_name',
     api_id=...,
     api_hash=...
 )
 
 
 @client.on_message(filters.command('start'))
 async def ask_user_name(client, message):
     # Ask the user age.
-    asking = message.ask("What's your name?")
+    asking = message.ask("What's your name?", quote=True)
 
     # Getting ask message and answer message.
     # TIP: you can to use `async for` too!
     ask, answer = await anext(asking)
 
     # Getting message text.
     user_name = answer.text
 
-    # Replying message.
-    await answer.reply(f'Nice name, {user_name}!')
+    # Replying message, without quote.
+    await answer.reply(f'Nice name, {user_name}!', quote=False)
 
 
-async def main():
-    # Start MTProto connection.
-    await client.start()
-
-    # Listen all command handlers.
-    await idle(client)
-
-    # When idle() is terminated, stop the client.
-    await client.stop()
-
 if __name__ == '__main__':
-    # Getting asyncio event loop.
-    loop = asyncio.get_event_loop()
-
-    # Run main() function until complete it.
-    loop.run_until_complete(main())
+    # Starting client and listening for updates.
+    client.run()
 ```
 
 **Pyrography** is a modern, elegant and asynchronous [MTProto API](https://docs.pyrogram.org/topics/mtproto-vs-botapi)
 framework. It enables you to easily interact with the main Telegram API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 #### Why should you use Pyrography?
 
 ##### 1. Stop safety
-Pyrography is the only mtproto library currently that when pressing `CTRL + C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
+Pyrography is the only mtproto library currently that when pressing `CTRL` + `C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
 
-#### To most performance and others
+### To most performance and others
 
-##### [TgCrypto](https://pypi.org/project/TgCrypto/)
+##### 1. Fast cryptography ([TgCrypto](https://pypi.org/project/TgCrypto/))
 A Cryptography Library written in C as a Python extension. It is designed to be portable, fast, easy to install and use. TgCrypto is intended for Pyrogram and implements the cryptographic algorithms Telegram requires.
 
 Automatically installed, ignore it.
 
-##### [Uvloop](https://pypi.org/project/uvloop/)
+##### 2. Fast event loop ([Uvloop](https://pypi.org/project/uvloop/))
 A fast, drop-in replacement of the built-in asyncio event loop. uvloop is implemented in Cython and uses libuv under the hood.
 
-Install it with `pip install uvloop`, import it and call `uvloop.install()` in your main script.
-
-##### Latency
-On hosting, choose an region close to Miami to your machine.
-
-##### Wonderful logging
-Use the `rich` library to have pretty logs.
-
-Automatically installed and default setted on `log_level` client parameter, set with `logging.NOTSET` to disable it.
-
-```python3
-import logging
-from rich.logging import RichHandler
+Install it, import it and call `uvloop.install()` in your main script.
 
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[RichHandler()]
-)
-
-log = logging.getLogger(__name__)
-log.info("Hello, World!")
-```
+##### 3. Wonderful logging ([Rich](https://pypi.org/project/rich/))
+Enabled by default, but you can to disable it setting **log_level** parameter to `logging.NOTSET`.
 
 [Read more here](https://rich.readthedocs.io/en/stable/logging.html).
 
+##### 4. Low latency
+On hosting, choose an region close to Miami to your machine.
+
 ### Installing
 
 #### Pypi
 
 ```
-pip install pyrography
+python3 -m pip install pyrography
 ```
 
 #### Github
 
 ```
-pip3 install git+https://github.com/d3cryptofc/pyrography
+python3 -m pip install git+https://github.com/d3cryptofc/pyrography
 ```
 
 ### Support Official Pyrogram
 
 If you'd like to support the official Pyrogram, you can consider:
 
 - [Become a GitHub sponsor](https://github.com/sponsors/delivrance).
```

### Comparing `Pyrography-1.0.0/Pyrography.egg-info/PKG-INFO` & `Pyrography-1.0.2/Pyrography.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyrography
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram.
 Home-page: https://github.com/d3cryptofc/pyrography
 Download-URL: https://github.com/d3cryptofc/pyrography/releases/latest
 Author: Lelzin λ
 Author-email: d3cryptofc@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/d3cryptofc/pyrography/issues
@@ -43,139 +43,103 @@
     <a href="https://github.com/pyrogram/pyrogram">
         <img src="https://github.com/d3cryptofc/pyrography/assets/47941854/0eb90a78-5054-497e-8c86-b5f6bbb70822" alt="Pyrogram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br/>A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram
     <br>
-    <a href="https://pyrogram.org">
-        Homepage
-    </a>
-    •
-    <a href="https://docs.pyrogram.org">
-        Documentation
-    </a>
-    •
-    <a href="https://docs.pyrogram.org/releases">
+    <a href="https://github.com/d3cryptofc/pyrography/releases">
         Releases
     </a>
     •
-    <a href="https://t.me/pyrogram">
+    <a href="https://t.me/forkpyrography">
         News
     </a>
 </p>
 
 ## Pyrography
 
 > Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 
 ```python3
-import asyncio
-from pyrography import Client, filters, idle
+from pyrography import Client, filters
+
 
 # Creating a client instance to control your bot.
-# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org
+# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org.
+# (optional `bot_token` parameter)
 client = Client(
     name='your_session_name',
     api_id=...,
     api_hash=...
 )
 
 
 @client.on_message(filters.command('start'))
 async def ask_user_name(client, message):
     # Ask the user age.
-    asking = message.ask("What's your name?")
+    asking = message.ask("What's your name?", quote=True)
 
     # Getting ask message and answer message.
     # TIP: you can to use `async for` too!
     ask, answer = await anext(asking)
 
     # Getting message text.
     user_name = answer.text
 
-    # Replying message.
-    await answer.reply(f'Nice name, {user_name}!')
+    # Replying message, without quote.
+    await answer.reply(f'Nice name, {user_name}!', quote=False)
 
 
-async def main():
-    # Start MTProto connection.
-    await client.start()
-
-    # Listen all command handlers.
-    await idle(client)
-
-    # When idle() is terminated, stop the client.
-    await client.stop()
-
 if __name__ == '__main__':
-    # Getting asyncio event loop.
-    loop = asyncio.get_event_loop()
-
-    # Run main() function until complete it.
-    loop.run_until_complete(main())
+    # Starting client and listening for updates.
+    client.run()
 ```
 
 **Pyrography** is a modern, elegant and asynchronous [MTProto API](https://docs.pyrogram.org/topics/mtproto-vs-botapi)
 framework. It enables you to easily interact with the main Telegram API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 #### Why should you use Pyrography?
 
 ##### 1. Stop safety
-Pyrography is the only mtproto library currently that when pressing `CTRL + C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
+Pyrography is the only mtproto library currently that when pressing `CTRL` + `C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
 
-#### To most performance and others
+### To most performance and others
 
-##### [TgCrypto](https://pypi.org/project/TgCrypto/)
+##### 1. Fast cryptography ([TgCrypto](https://pypi.org/project/TgCrypto/))
 A Cryptography Library written in C as a Python extension. It is designed to be portable, fast, easy to install and use. TgCrypto is intended for Pyrogram and implements the cryptographic algorithms Telegram requires.
 
 Automatically installed, ignore it.
 
-##### [Uvloop](https://pypi.org/project/uvloop/)
+##### 2. Fast event loop ([Uvloop](https://pypi.org/project/uvloop/))
 A fast, drop-in replacement of the built-in asyncio event loop. uvloop is implemented in Cython and uses libuv under the hood.
 
-Install it with `pip install uvloop`, import it and call `uvloop.install()` in your main script.
-
-##### Latency
-On hosting, choose an region close to Miami to your machine.
-
-##### Wonderful logging
-Use the `rich` library to have pretty logs.
-
-Automatically installed and default setted on `log_level` client parameter, set with `logging.NOTSET` to disable it.
-
-```python3
-import logging
-from rich.logging import RichHandler
+Install it, import it and call `uvloop.install()` in your main script.
 
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[RichHandler()]
-)
-
-log = logging.getLogger(__name__)
-log.info("Hello, World!")
-```
+##### 3. Wonderful logging ([Rich](https://pypi.org/project/rich/))
+Enabled by default, but you can to disable it setting **log_level** parameter to `logging.NOTSET`.
 
 [Read more here](https://rich.readthedocs.io/en/stable/logging.html).
 
+##### 4. Low latency
+On hosting, choose an region close to Miami to your machine.
+
 ### Installing
 
 #### Pypi
 
 ```
-pip install pyrography
+python3 -m pip install pyrography
 ```
 
 #### Github
 
 ```
-pip3 install git+https://github.com/d3cryptofc/pyrography
+python3 -m pip install git+https://github.com/d3cryptofc/pyrography
 ```
 
 ### Support Official Pyrogram
 
 If you'd like to support the official Pyrogram, you can consider:
 
 - [Become a GitHub sponsor](https://github.com/sponsors/delivrance).
```

### Comparing `Pyrography-1.0.0/Pyrography.egg-info/SOURCES.txt` & `Pyrography-1.0.2/Pyrography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/README.md` & `Pyrography-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,139 +2,103 @@
     <a href="https://github.com/pyrogram/pyrogram">
         <img src="https://github.com/d3cryptofc/pyrography/assets/47941854/0eb90a78-5054-497e-8c86-b5f6bbb70822" alt="Pyrogram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br/>A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram
     <br>
-    <a href="https://pyrogram.org">
-        Homepage
-    </a>
-    •
-    <a href="https://docs.pyrogram.org">
-        Documentation
-    </a>
-    •
-    <a href="https://docs.pyrogram.org/releases">
+    <a href="https://github.com/d3cryptofc/pyrography/releases">
         Releases
     </a>
     •
-    <a href="https://t.me/pyrogram">
+    <a href="https://t.me/forkpyrography">
         News
     </a>
 </p>
 
 ## Pyrography
 
 > Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 
 ```python3
-import asyncio
-from pyrography import Client, filters, idle
+from pyrography import Client, filters
+
 
 # Creating a client instance to control your bot.
-# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org
+# NOTE: Get your `api_id` and `api_hash` credentials on: my.telegram.org.
+# (optional `bot_token` parameter)
 client = Client(
     name='your_session_name',
     api_id=...,
     api_hash=...
 )
 
 
 @client.on_message(filters.command('start'))
 async def ask_user_name(client, message):
     # Ask the user age.
-    asking = message.ask("What's your name?")
+    asking = message.ask("What's your name?", quote=True)
 
     # Getting ask message and answer message.
     # TIP: you can to use `async for` too!
     ask, answer = await anext(asking)
 
     # Getting message text.
     user_name = answer.text
 
-    # Replying message.
-    await answer.reply(f'Nice name, {user_name}!')
+    # Replying message, without quote.
+    await answer.reply(f'Nice name, {user_name}!', quote=False)
 
 
-async def main():
-    # Start MTProto connection.
-    await client.start()
-
-    # Listen all command handlers.
-    await idle(client)
-
-    # When idle() is terminated, stop the client.
-    await client.stop()
-
 if __name__ == '__main__':
-    # Getting asyncio event loop.
-    loop = asyncio.get_event_loop()
-
-    # Run main() function until complete it.
-    loop.run_until_complete(main())
+    # Starting client and listening for updates.
+    client.run()
 ```
 
 **Pyrography** is a modern, elegant and asynchronous [MTProto API](https://docs.pyrogram.org/topics/mtproto-vs-botapi)
 framework. It enables you to easily interact with the main Telegram API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 #### Why should you use Pyrography?
 
 ##### 1. Stop safety
-Pyrography is the only mtproto library currently that when pressing `CTRL + C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
+Pyrography is the only mtproto library currently that when pressing `CTRL` + `C` to interrupt the program, it will wait for pending commands to finish, preventing anything from being incomplete.
 
-#### To most performance and others
+### To most performance and others
 
-##### [TgCrypto](https://pypi.org/project/TgCrypto/)
+##### 1. Fast cryptography ([TgCrypto](https://pypi.org/project/TgCrypto/))
 A Cryptography Library written in C as a Python extension. It is designed to be portable, fast, easy to install and use. TgCrypto is intended for Pyrogram and implements the cryptographic algorithms Telegram requires.
 
 Automatically installed, ignore it.
 
-##### [Uvloop](https://pypi.org/project/uvloop/)
+##### 2. Fast event loop ([Uvloop](https://pypi.org/project/uvloop/))
 A fast, drop-in replacement of the built-in asyncio event loop. uvloop is implemented in Cython and uses libuv under the hood.
 
-Install it with `pip install uvloop`, import it and call `uvloop.install()` in your main script.
-
-##### Latency
-On hosting, choose an region close to Miami to your machine.
-
-##### Wonderful logging
-Use the `rich` library to have pretty logs.
-
-Automatically installed and default setted on `log_level` client parameter, set with `logging.NOTSET` to disable it.
-
-```python3
-import logging
-from rich.logging import RichHandler
+Install it, import it and call `uvloop.install()` in your main script.
 
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[RichHandler()]
-)
-
-log = logging.getLogger(__name__)
-log.info("Hello, World!")
-```
+##### 3. Wonderful logging ([Rich](https://pypi.org/project/rich/))
+Enabled by default, but you can to disable it setting **log_level** parameter to `logging.NOTSET`.
 
 [Read more here](https://rich.readthedocs.io/en/stable/logging.html).
 
+##### 4. Low latency
+On hosting, choose an region close to Miami to your machine.
+
 ### Installing
 
 #### Pypi
 
 ```
-pip install pyrography
+python3 -m pip install pyrography
 ```
 
 #### Github
 
 ```
-pip3 install git+https://github.com/d3cryptofc/pyrography
+python3 -m pip install git+https://github.com/d3cryptofc/pyrography
 ```
 
 ### Support Official Pyrogram
 
 If you'd like to support the official Pyrogram, you can consider:
 
 - [Become a GitHub sponsor](https://github.com/sponsors/delivrance).
```

### Comparing `Pyrography-1.0.0/compiler/__init__.py` & `Pyrography-1.0.2/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/__init__.py` & `Pyrography-1.0.2/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/compiler.py` & `Pyrography-1.0.2/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/source/auth_key.tl` & `Pyrography-1.0.2/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/source/main_api.tl` & `Pyrography-1.0.2/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/source/sys_msgs.tl` & `Pyrography-1.0.2/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/template/combinator.txt` & `Pyrography-1.0.2/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/api/template/type.txt` & `Pyrography-1.0.2/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/docs/__init__.py` & `Pyrography-1.0.2/compiler/docs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-#  Pyrogram - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
-#
-#  This file is part of Pyrogram.
-#
-#  Pyrogram is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  Pyrogram is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+"""
+Pyrography - A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram.
+Copyright (C) 2023-present Lelzin λ <https://github.com/d3cryptofc>
+
+Forked from Pyrogram <https://github.com/pyrogram/pyrogram>,
+originally copyright (C) 2017-present Dan <https://github.com/delivrance>
+
+This file is part of Pyrography.
+
+Pyrography is is free software: you can redistribute it and/or modify it under
+the terms of the GNU Lesser General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version.
+
+Pyrography is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License
+for more details.
+
+You should have received a copy of the GNU Lesser General Public License along
+with Pyrography. If not, see <http://www.gnu.org/licenses/>.
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pyrography-1.0.0/compiler/docs/compiler.py` & `Pyrography-1.0.2/compiler/docs/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-#  Pyrogram - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
-#
-#  This file is part of Pyrogram.
-#
-#  Pyrogram is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  Pyrogram is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+"""
+Pyrography - A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram.
+Copyright (C) 2023-present Lelzin λ <https://github.com/d3cryptofc>
+
+Forked from Pyrogram <https://github.com/pyrogram/pyrogram>,
+originally copyright (C) 2017-present Dan <https://github.com/delivrance>
+
+This file is part of Pyrography.
+
+Pyrography is is free software: you can redistribute it and/or modify it under
+the terms of the GNU Lesser General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version.
+
+Pyrography is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License
+for more details.
+
+You should have received a copy of the GNU Lesser General Public License along
+with Pyrography. If not, see <http://www.gnu.org/licenses/>.
+"""
 
 import ast
 import os
 import re
 import shutil
 
 HOME = "compiler/docs"
 DESTINATION = "docs/source/telegram"
 PYROGRAM_API_DEST = "docs/source/api"
 
-FUNCTIONS_PATH = "pyrogram/raw/functions"
-TYPES_PATH = "pyrogram/raw/types"
-BASE_PATH = "pyrogram/raw/base"
+FUNCTIONS_PATH = "pyrography/raw/functions"
+TYPES_PATH = "pyrography/raw/types"
+BASE_PATH = "pyrography/raw/base"
 
 FUNCTIONS_BASE = "functions"
 TYPES_BASE = "types"
 BASE_BASE = "base"
 
 
 def snek(s: str):
@@ -125,14 +130,18 @@
 
             f.write("\n")
 
 
 def pyrogram_api():
     def get_title_list(s: str) -> list:
         return [i.strip() for i in [j.strip() for j in s.split("\n") if j] if i]
+    
+    if not os.path.exists(PYROGRAM_API_DEST):
+        os.mkdir(PYROGRAM_API_DEST)
+    
 
     # Methods
 
     categories = dict(
         utilities="""
         Utilities
             start
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pyrography-1.0.0/compiler/errors/__init__.py` & `Pyrography-1.0.2/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/compiler.py` & `Pyrography-1.0.2/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/sort.py` & `Pyrography-1.0.2/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/source/400_BAD_REQUEST.tsv` & `Pyrography-1.0.2/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv` & `Pyrography-1.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/source/403_FORBIDDEN.tsv` & `Pyrography-1.0.2/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `Pyrography-1.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `Pyrography-1.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/__init__.py` & `Pyrography-1.0.2/pyrography/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License
 for more details.
 
 You should have received a copy of the GNU Lesser General Public License along
 with Pyrography. If not, see <http://www.gnu.org/licenses/>.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.2"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = (
     'Pyrography - A wonderful Pyrogram fork inspired by Pyromod & AmanoTeam/Pyrogram.\n'
     'Copyright (C) 2023-present Lelzin λ <https://github.com/d3cryptofc>\n\n'
 
     'Forked from Pyrogram <https://github.com/pyrogram/pyrogram>,\n'
     'originally copyright (C) 2017-present Dan <https://github.com/delivrance>'
```

### Comparing `Pyrography-1.0.0/pyrography/client.py` & `Pyrography-1.0.2/pyrography/client.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/__init__.py` & `Pyrography-1.0.2/pyrography/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/connection.py` & `Pyrography-1.0.2/pyrography/connection/connection.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/__init__.py` & `Pyrography-1.0.2/pyrography/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/__init__.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_abridged.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_abridged_o.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_full.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_intermediate.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/connection/transport/tcp/tcp_intermediate_o.py` & `Pyrography-1.0.2/pyrography/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/crypto/__init__.py` & `Pyrography-1.0.2/pyrography/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/crypto/aes.py` & `Pyrography-1.0.2/pyrography/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/crypto/mtproto.py` & `Pyrography-1.0.2/pyrography/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/crypto/prime.py` & `Pyrography-1.0.2/pyrography/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/crypto/rsa.py` & `Pyrography-1.0.2/pyrography/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/dispatcher.py` & `Pyrography-1.0.2/pyrography/dispatcher.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/emoji.py` & `Pyrography-1.0.2/pyrography/emoji.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/__init__.py` & `Pyrography-1.0.2/pyrography/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/auto_name.py` & `Pyrography-1.0.2/pyrography/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/chat_action.py` & `Pyrography-1.0.2/pyrography/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/chat_event_action.py` & `Pyrography-1.0.2/pyrography/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/chat_member_status.py` & `Pyrography-1.0.2/pyrography/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/chat_members_filter.py` & `Pyrography-1.0.2/pyrography/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/chat_type.py` & `Pyrography-1.0.2/pyrography/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/message_entity_type.py` & `Pyrography-1.0.2/pyrography/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/message_media_type.py` & `Pyrography-1.0.2/pyrography/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/message_service_type.py` & `Pyrography-1.0.2/pyrography/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/messages_filter.py` & `Pyrography-1.0.2/pyrography/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/next_code_type.py` & `Pyrography-1.0.2/pyrography/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/parse_mode.py` & `Pyrography-1.0.2/pyrography/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/poll_type.py` & `Pyrography-1.0.2/pyrography/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/sent_code_type.py` & `Pyrography-1.0.2/pyrography/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/enums/user_status.py` & `Pyrography-1.0.2/pyrography/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/errors/__init__.py` & `Pyrography-1.0.2/pyrography/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/errors/rpc_error.py` & `Pyrography-1.0.2/pyrography/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/file_id.py` & `Pyrography-1.0.2/pyrography/file_id.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/filters.py` & `Pyrography-1.0.2/pyrography/filters.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/__init__.py` & `Pyrography-1.0.2/pyrography/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/callback_query_handler.py` & `Pyrography-1.0.2/pyrography/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/chat_join_request_handler.py` & `Pyrography-1.0.2/pyrography/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/chat_member_updated_handler.py` & `Pyrography-1.0.2/pyrography/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/chosen_inline_result_handler.py` & `Pyrography-1.0.2/pyrography/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/deleted_messages_handler.py` & `Pyrography-1.0.2/pyrography/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/disconnect_handler.py` & `Pyrography-1.0.2/pyrography/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/edited_message_handler.py` & `Pyrography-1.0.2/pyrography/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/handler.py` & `Pyrography-1.0.2/pyrography/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/inline_query_handler.py` & `Pyrography-1.0.2/pyrography/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/message_handler.py` & `Pyrography-1.0.2/pyrography/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/poll_handler.py` & `Pyrography-1.0.2/pyrography/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/raw_update_handler.py` & `Pyrography-1.0.2/pyrography/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/handlers/user_status_handler.py` & `Pyrography-1.0.2/pyrography/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/__init__.py` & `Pyrography-1.0.2/pyrography/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/advanced/__init__.py` & `Pyrography-1.0.2/pyrography/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/advanced/invoke.py` & `Pyrography-1.0.2/pyrography/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/advanced/resolve_peer.py` & `Pyrography-1.0.2/pyrography/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/advanced/save_file.py` & `Pyrography-1.0.2/pyrography/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/__init__.py` & `Pyrography-1.0.2/pyrography/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/accept_terms_of_service.py` & `Pyrography-1.0.2/pyrography/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/check_password.py` & `Pyrography-1.0.2/pyrography/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/connect.py` & `Pyrography-1.0.2/pyrography/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/disconnect.py` & `Pyrography-1.0.2/pyrography/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/get_password_hint.py` & `Pyrography-1.0.2/pyrography/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/initialize.py` & `Pyrography-1.0.2/pyrography/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/log_out.py` & `Pyrography-1.0.2/pyrography/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/recover_password.py` & `Pyrography-1.0.2/pyrography/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/resend_code.py` & `Pyrography-1.0.2/pyrography/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/send_code.py` & `Pyrography-1.0.2/pyrography/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/send_recovery_code.py` & `Pyrography-1.0.2/pyrography/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/sign_in.py` & `Pyrography-1.0.2/pyrography/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/sign_in_bot.py` & `Pyrography-1.0.2/pyrography/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/sign_up.py` & `Pyrography-1.0.2/pyrography/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/auth/terminate.py` & `Pyrography-1.0.2/pyrography/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/__init__.py` & `Pyrography-1.0.2/pyrography/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/answer_callback_query.py` & `Pyrography-1.0.2/pyrography/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/answer_inline_query.py` & `Pyrography-1.0.2/pyrography/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/answer_web_app_query.py` & `Pyrography-1.0.2/pyrography/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/delete_bot_commands.py` & `Pyrography-1.0.2/pyrography/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/get_bot_commands.py` & `Pyrography-1.0.2/pyrography/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/get_bot_default_privileges.py` & `Pyrography-1.0.2/pyrography/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/get_chat_menu_button.py` & `Pyrography-1.0.2/pyrography/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/get_game_high_scores.py` & `Pyrography-1.0.2/pyrography/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/get_inline_bot_results.py` & `Pyrography-1.0.2/pyrography/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/request_callback_answer.py` & `Pyrography-1.0.2/pyrography/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/send_game.py` & `Pyrography-1.0.2/pyrography/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/send_inline_bot_result.py` & `Pyrography-1.0.2/pyrography/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/set_bot_commands.py` & `Pyrography-1.0.2/pyrography/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/set_bot_default_privileges.py` & `Pyrography-1.0.2/pyrography/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/set_chat_menu_button.py` & `Pyrography-1.0.2/pyrography/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/bots/set_game_score.py` & `Pyrography-1.0.2/pyrography/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/__init__.py` & `Pyrography-1.0.2/pyrography/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/add_chat_members.py` & `Pyrography-1.0.2/pyrography/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/archive_chats.py` & `Pyrography-1.0.2/pyrography/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/ban_chat_member.py` & `Pyrography-1.0.2/pyrography/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/create_channel.py` & `Pyrography-1.0.2/pyrography/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/create_group.py` & `Pyrography-1.0.2/pyrography/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/create_supergroup.py` & `Pyrography-1.0.2/pyrography/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/delete_channel.py` & `Pyrography-1.0.2/pyrography/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/delete_chat_photo.py` & `Pyrography-1.0.2/pyrography/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/delete_supergroup.py` & `Pyrography-1.0.2/pyrography/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/delete_user_history.py` & `Pyrography-1.0.2/pyrography/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat_event_log.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat_member.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat_members.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat_members_count.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_chat_online_count.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_dialogs.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_dialogs_count.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_nearby_chats.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/get_send_as_chats.py` & `Pyrography-1.0.2/pyrography/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/join_chat.py` & `Pyrography-1.0.2/pyrography/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/leave_chat.py` & `Pyrography-1.0.2/pyrography/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/mark_chat_unread.py` & `Pyrography-1.0.2/pyrography/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/pin_chat_message.py` & `Pyrography-1.0.2/pyrography/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/promote_chat_member.py` & `Pyrography-1.0.2/pyrography/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/restrict_chat_member.py` & `Pyrography-1.0.2/pyrography/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_administrator_title.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_description.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_permissions.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_photo.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_protected_content.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_title.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_chat_username.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_send_as_chat.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/set_slow_mode.py` & `Pyrography-1.0.2/pyrography/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/unarchive_chats.py` & `Pyrography-1.0.2/pyrography/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/unban_chat_member.py` & `Pyrography-1.0.2/pyrography/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/unpin_all_chat_messages.py` & `Pyrography-1.0.2/pyrography/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/chats/unpin_chat_message.py` & `Pyrography-1.0.2/pyrography/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/__init__.py` & `Pyrography-1.0.2/pyrography/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/add_contact.py` & `Pyrography-1.0.2/pyrography/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/delete_contacts.py` & `Pyrography-1.0.2/pyrography/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/get_contacts.py` & `Pyrography-1.0.2/pyrography/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/get_contacts_count.py` & `Pyrography-1.0.2/pyrography/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/contacts/import_contacts.py` & `Pyrography-1.0.2/pyrography/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/__init__.py` & `Pyrography-1.0.2/pyrography/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_callback_query.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_chat_join_request.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_chat_member_updated.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_chosen_inline_result.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_deleted_messages.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_disconnect.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_edited_message.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_inline_query.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_message.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_poll.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_raw_update.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/decorators/on_user_status.py` & `Pyrography-1.0.2/pyrography/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/__init__.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/approve_all_chat_join_requests.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/approve_chat_join_request.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/create_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/decline_all_chat_join_requests.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/decline_chat_join_request.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/delete_chat_admin_invite_links.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/delete_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/edit_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/export_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admin_invite_links.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admin_invite_links_count.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_admins_with_invite_links.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link_joiners.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_invite_link_joiners_count.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/get_chat_join_requests.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/invite_links/revoke_chat_invite_link.py` & `Pyrography-1.0.2/pyrography/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/__init__.py` & `Pyrography-1.0.2/pyrography/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/copy_media_group.py` & `Pyrography-1.0.2/pyrography/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/copy_message.py` & `Pyrography-1.0.2/pyrography/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/delete_messages.py` & `Pyrography-1.0.2/pyrography/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/download_media.py` & `Pyrography-1.0.2/pyrography/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_inline_caption.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_inline_media.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_inline_reply_markup.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_inline_text.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_message_caption.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_message_media.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_message_reply_markup.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/edit_message_text.py` & `Pyrography-1.0.2/pyrography/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/forward_messages.py` & `Pyrography-1.0.2/pyrography/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_chat_history.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_chat_history_count.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_custom_emoji_stickers.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_discussion_message.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_discussion_replies.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_discussion_replies_count.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_media_group.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/get_messages.py` & `Pyrography-1.0.2/pyrography/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/inline_session.py` & `Pyrography-1.0.2/pyrography/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/read_chat_history.py` & `Pyrography-1.0.2/pyrography/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/retract_vote.py` & `Pyrography-1.0.2/pyrography/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/search_global.py` & `Pyrography-1.0.2/pyrography/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/search_global_count.py` & `Pyrography-1.0.2/pyrography/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/search_messages.py` & `Pyrography-1.0.2/pyrography/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/search_messages_count.py` & `Pyrography-1.0.2/pyrography/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_animation.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_audio.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_cached_media.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_chat_action.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_contact.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_dice.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_document.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_location.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_media_group.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_message.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_photo.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_poll.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_reaction.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_sticker.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_venue.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_video.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_video_note.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/send_voice.py` & `Pyrography-1.0.2/pyrography/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/stop_poll.py` & `Pyrography-1.0.2/pyrography/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/stream_media.py` & `Pyrography-1.0.2/pyrography/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/vote_poll.py` & `Pyrography-1.0.2/pyrography/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/messages/wait_for.py` & `Pyrography-1.0.2/pyrography/methods/messages/wait_for.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/password/__init__.py` & `Pyrography-1.0.2/pyrography/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/password/change_cloud_password.py` & `Pyrography-1.0.2/pyrography/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/password/enable_cloud_password.py` & `Pyrography-1.0.2/pyrography/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/password/remove_cloud_password.py` & `Pyrography-1.0.2/pyrography/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/__init__.py` & `Pyrography-1.0.2/pyrography/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/block_user.py` & `Pyrography-1.0.2/pyrography/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/delete_profile_photos.py` & `Pyrography-1.0.2/pyrography/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_chat_photos.py` & `Pyrography-1.0.2/pyrography/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_chat_photos_count.py` & `Pyrography-1.0.2/pyrography/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_common_chats.py` & `Pyrography-1.0.2/pyrography/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_default_emoji_statuses.py` & `Pyrography-1.0.2/pyrography/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_me.py` & `Pyrography-1.0.2/pyrography/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/get_users.py` & `Pyrography-1.0.2/pyrography/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/set_emoji_status.py` & `Pyrography-1.0.2/pyrography/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/set_profile_photo.py` & `Pyrography-1.0.2/pyrography/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/set_username.py` & `Pyrography-1.0.2/pyrography/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/unblock_user.py` & `Pyrography-1.0.2/pyrography/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/users/update_profile.py` & `Pyrography-1.0.2/pyrography/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/__init__.py` & `Pyrography-1.0.2/pyrography/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/add_handler.py` & `Pyrography-1.0.2/pyrography/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/compose.py` & `Pyrography-1.0.2/pyrography/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/export_session_string.py` & `Pyrography-1.0.2/pyrography/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/idle.py` & `Pyrography-1.0.2/pyrography/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/remove_handler.py` & `Pyrography-1.0.2/pyrography/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/restart.py` & `Pyrography-1.0.2/pyrography/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/run.py` & `Pyrography-1.0.2/pyrography/methods/utilities/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,20 @@
         """
         loop = asyncio.get_event_loop()
         run = loop.run_until_complete
 
         if coroutine is not None:
             run(coroutine)
         else:
-            if inspect.iscoroutinefunction(self.start):
-                run(self.start())
-                run(idle())
-                run(self.stop())
-            else:
-                self.start()
-                run(idle())
-                self.stop()
+            if loop.is_running():
+                raise RuntimeError(
+                    'You must call client.run() method out of asyncio event loop. '
+                    'Otherwise you can to use client.start() and pyrography.idle() after.')
+
+            # Start MTProto connection.
+            self.start()
+
+            # Blocking execution and listening updates.
+            run(idle(self))
+
+            # Disconnect MTProto connection.
+            self.stop()
```

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/start.py` & `Pyrography-1.0.2/pyrography/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/stop.py` & `Pyrography-1.0.2/pyrography/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/methods/utilities/stop_transmission.py` & `Pyrography-1.0.2/pyrography/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/mime_types.py` & `Pyrography-1.0.2/pyrography/mime_types.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/parser/__init__.py` & `Pyrography-1.0.2/pyrography/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/parser/html.py` & `Pyrography-1.0.2/pyrography/parser/html.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/parser/markdown.py` & `Pyrography-1.0.2/pyrography/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/parser/parser.py` & `Pyrography-1.0.2/pyrography/parser/parser.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/parser/utils.py` & `Pyrography-1.0.2/pyrography/parser/utils.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/__init__.py` & `Pyrography-1.0.2/pyrography/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/__init__.py` & `Pyrography-1.0.2/pyrography/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/future_salt.py` & `Pyrography-1.0.2/pyrography/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/future_salts.py` & `Pyrography-1.0.2/pyrography/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/gzip_packed.py` & `Pyrography-1.0.2/pyrography/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/list.py` & `Pyrography-1.0.2/pyrography/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/message.py` & `Pyrography-1.0.2/pyrography/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/msg_container.py` & `Pyrography-1.0.2/pyrography/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/__init__.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/bool.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/bytes.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/double.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/int.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/string.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/primitives/vector.py` & `Pyrography-1.0.2/pyrography/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/raw/core/tl_object.py` & `Pyrography-1.0.2/pyrography/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/__init__.py` & `Pyrography-1.0.2/pyrography/session/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/auth.py` & `Pyrography-1.0.2/pyrography/session/auth.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/internals/__init__.py` & `Pyrography-1.0.2/pyrography/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/internals/data_center.py` & `Pyrography-1.0.2/pyrography/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/internals/msg_factory.py` & `Pyrography-1.0.2/pyrography/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/internals/msg_id.py` & `Pyrography-1.0.2/pyrography/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/internals/seq_no.py` & `Pyrography-1.0.2/pyrography/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/session/session.py` & `Pyrography-1.0.2/pyrography/session/session.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/storage/__init__.py` & `Pyrography-1.0.2/pyrography/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/storage/file_storage.py` & `Pyrography-1.0.2/pyrography/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/storage/memory_storage.py` & `Pyrography-1.0.2/pyrography/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/storage/sqlite_storage.py` & `Pyrography-1.0.2/pyrography/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/storage/storage.py` & `Pyrography-1.0.2/pyrography/storage/storage.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/sync.py` & `Pyrography-1.0.2/pyrography/sync.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/__init__.py` & `Pyrography-1.0.2/pyrography/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/authorization/__init__.py` & `Pyrography-1.0.2/pyrography/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/authorization/sent_code.py` & `Pyrography-1.0.2/pyrography/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/authorization/terms_of_service.py` & `Pyrography-1.0.2/pyrography/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/__init__.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/bot_command_scope_default.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/callback_game.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/callback_query.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/force_reply.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/game_high_score.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/inline_keyboard_button.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/inline_keyboard_markup.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/keyboard_button.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/login_url.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_commands.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_default.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/menu_button_web_app.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/reply_keyboard_markup.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/reply_keyboard_remove.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/sent_web_app_message.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/bots_and_keyboards/web_app_info.py` & `Pyrography-1.0.2/pyrography/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/__init__.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/chosen_inline_result.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_animation.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_article.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_audio.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_animation.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_audio.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_document.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_photo.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_sticker.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_video.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_cached_voice.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_contact.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_document.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_location.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_photo.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_venue.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_video.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/inline_mode/inline_query_result_voice.py` & `Pyrography-1.0.2/pyrography/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/__init__.py` & `Pyrography-1.0.2/pyrography/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media_animation.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media_audio.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media_document.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media_photo.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_media_video.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_media/input_phone_contact.py` & `Pyrography-1.0.2/pyrography/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_message_content/__init__.py` & `Pyrography-1.0.2/pyrography/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_message_content/input_message_content.py` & `Pyrography-1.0.2/pyrography/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/input_message_content/input_text_message_content.py` & `Pyrography-1.0.2/pyrography/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/list.py` & `Pyrography-1.0.2/pyrography/types/list.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/__init__.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/animation.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/audio.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/contact.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/dice.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/document.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/game.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/location.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/message.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/message_entity.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/message_reactions.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/photo.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/poll.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/poll_option.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/reaction.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/sticker.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/stripped_thumbnail.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/thumbnail.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/venue.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/video.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/video_note.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/voice.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/web_app_data.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/messages_and_media/web_page.py` & `Pyrography-1.0.2/pyrography/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/object.py` & `Pyrography-1.0.2/pyrography/types/object.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/update.py` & `Pyrography-1.0.2/pyrography/types/update.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/__init__.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_admin_with_invite_links.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_event.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_event_filter.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_invite_link.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_join_request.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_joiner.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_member.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_member_updated.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_permissions.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_photo.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_preview.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_privileges.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/chat_reactions.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/dialog.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/emoji_status.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/invite_link_importer.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/restriction.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/user.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_ended.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_members_invited.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_scheduled.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/types/user_and_chats/video_chat_started.py` & `Pyrography-1.0.2/pyrography/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/pyrography/utils.py` & `Pyrography-1.0.2/pyrography/utils.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/setup.py` & `Pyrography-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/__init__.py` & `Pyrography-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/filters/__init__.py` & `Pyrography-1.0.2/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/filters/test_command.py` & `Pyrography-1.0.2/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/parser/__init__.py` & `Pyrography-1.0.2/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/parser/test_html.py` & `Pyrography-1.0.2/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `Pyrography-1.0.0/tests/test_file_id.py` & `Pyrography-1.0.2/tests/test_file_id.py`

 * *Files identical despite different names*

