# Comparing `tmp/Netfoll-TL-2.0.0.tar.gz` & `tmp/Netfoll-TL-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Netfoll-TL-2.0.0.tar", last modified: Fri Apr 14 14:22:33 2023, max compression
+gzip compressed data, was "Netfoll-TL-2.0.1.tar", last modified: Sun Apr 30 12:34:08 2023, max compression
```

## Comparing `Netfoll-TL-2.0.0.tar` & `Netfoll-TL-2.0.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:33.876895 Netfoll-TL-2.0.0/
--rw-rw-rw-   0        0        0     1096 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:31.138540 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/
--rw-rw-rw-   0        0        0     3168 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/Netfoll_TL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3168 2023-04-14 14:22:33.872897 Netfoll-TL-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:31.350747 Netfoll-TL-2.0.0/netfoll_tl/
--rw-rw-rw-   0        0        0      420 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:31.507178 Netfoll-TL-2.0.0/netfoll_tl/_updates/
--rw-rw-rw-   0        0        0      173 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/_updates/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/_updates/entitycache.py
--rw-rw-rw-   0        0        0    34827 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/_updates/messagebox.py
--rw-rw-rw-   0        0        0     6363 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/_updates/session.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:31.917573 Netfoll-TL-2.0.0/netfoll_tl/client/
--rw-rw-rw-   0        0        0     1225 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/__init__.py
--rw-rw-rw-   0        0        0     9815 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/account.py
--rw-rw-rw-   0        0        0    25488 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/auth.py
--rw-rw-rw-   0        0        0     2525 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/bots.py
--rw-rw-rw-   0        0        0     3376 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/buttons.py
--rw-rw-rw-   0        0        0    53320 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/chats.py
--rw-rw-rw-   0        0        0    23618 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/dialogs.py
--rw-rw-rw-   0        0        0    40727 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/downloads.py
--rw-rw-rw-   0        0        0     9620 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/messageparse.py
--rw-rw-rw-   0        0        0    63451 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/messages.py
--rw-rw-rw-   0        0        0    39473 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/telegrambaseclient.py
--rw-rw-rw-   0        0        0      491 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/telegramclient.py
--rw-rw-rw-   0        0        0    29176 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/updates.py
--rw-rw-rw-   0        0        0    33752 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/uploads.py
--rw-rw-rw-   0        0        0    25348 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/client/users.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.050069 Netfoll-TL-2.0.0/netfoll_tl/crypto/
--rw-rw-rw-   0        0        0      359 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/aes.py
--rw-rw-rw-   0        0        0     1258 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/aesctr.py
--rw-rw-rw-   0        0        0     1950 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/authkey.py
--rw-rw-rw-   0        0        0     3949 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/cdndecrypter.py
--rw-rw-rw-   0        0        0     1700 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/factorization.py
--rw-rw-rw-   0        0        0     4668 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/libssl.py
--rw-rw-rw-   0        0        0     6690 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/crypto/rsa.py
--rw-rw-rw-   0        0        0       26 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/custom.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.115074 Netfoll-TL-2.0.0/netfoll_tl/errors/
--rw-rw-rw-   0        0        0     1705 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/errors/__init__.py
--rw-rw-rw-   0        0        0     6665 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/errors/common.py
--rw-rw-rw-   0        0        0     3601 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/errors/rpcbaseerrors.py
--rw-rw-rw-   0        0        0   196260 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/netfoll_tl/errors/rpcerrorlist.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.327760 Netfoll-TL-2.0.0/netfoll_tl/events/
--rw-rw-rw-   0        0        0     4415 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/__init__.py
--rw-rw-rw-   0        0        0    13233 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/album.py
--rw-rw-rw-   0        0        0    13768 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/callbackquery.py
--rw-rw-rw-   0        0        0    18424 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/chataction.py
--rw-rw-rw-   0        0        0     6501 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/common.py
--rw-rw-rw-   0        0        0     9221 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/inlinequery.py
--rw-rw-rw-   0        0        0     2185 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/messagedeleted.py
--rw-rw-rw-   0        0        0     1938 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/messageedited.py
--rw-rw-rw-   0        0        0     5613 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/messageread.py
--rw-rw-rw-   0        0        0     9384 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/newmessage.py
--rw-rw-rw-   0        0        0     1704 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/raw.py
--rw-rw-rw-   0        0        0    10930 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/events/userupdate.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.436763 Netfoll-TL-2.0.0/netfoll_tl/extensions/
--rw-rw-rw-   0        0        0      286 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/extensions/__init__.py
--rw-rw-rw-   0        0        0     5930 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/extensions/binaryreader.py
--rw-rw-rw-   0        0        0    11261 2023-04-14 14:19:00.000000 Netfoll-TL-2.0.0/netfoll_tl/extensions/html.py
--rw-rw-rw-   0        0        0     7050 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/extensions/markdown.py
--rw-rw-rw-   0        0        0     4186 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/extensions/messagepacker.py
--rw-rw-rw-   0        0        0       29 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/functions.py
--rw-rw-rw-   0        0        0    15159 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/helpers.py
--rw-rw-rw-   0        0        0     1629 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/hints.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.538765 Netfoll-TL-2.0.0/netfoll_tl/network/
--rw-rw-rw-   0        0        0      599 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/__init__.py
--rw-rw-rw-   0        0        0     8081 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/authenticator.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.730774 Netfoll-TL-2.0.0/netfoll_tl/network/connection/
--rw-rw-rw-   0        0        0      435 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/__init__.py
--rw-rw-rw-   0        0        0    16132 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/connection.py
--rw-rw-rw-   0        0        0     1259 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/http.py
--rw-rw-rw-   0        0        0      994 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpabridged.py
--rw-rw-rw-   0        0        0     1785 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpfull.py
--rw-rw-rw-   0        0        0     1420 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpintermediate.py
--rw-rw-rw-   0        0        0     5431 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpmtproxy.py
--rw-rw-rw-   0        0        0     2065 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpobfuscated.py
--rw-rw-rw-   0        0        0     2075 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/mtprotoplainsender.py
--rw-rw-rw-   0        0        0    39048 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/mtprotosender.py
--rw-rw-rw-   0        0        0    11247 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/mtprotostate.py
--rw-rw-rw-   0        0        0      663 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/network/requeststate.py
--rw-rw-rw-   0        0        0     7388 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/password.py
--rw-rw-rw-   0        0        0     4520 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/requestiter.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.812776 Netfoll-TL-2.0.0/netfoll_tl/sessions/
--rw-rw-rw-   0        0        0      136 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/sessions/__init__.py
--rw-rw-rw-   0        0        0     5263 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/sessions/abstract.py
--rw-rw-rw-   0        0        0     8567 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/sessions/memory.py
--rw-rw-rw-   0        0        0    12952 2023-04-14 13:49:00.000000 Netfoll-TL-2.0.0/netfoll_tl/sessions/sqlite.py
--rw-rw-rw-   0        0        0     2053 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/sessions/string.py
--rw-rw-rw-   0        0        0     2683 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.878780 Netfoll-TL-2.0.0/netfoll_tl/tl/
--rw-rw-rw-   0        0        0       43 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/__init__.py
--rw-rw-rw-   0        0        0    82964 2023-04-14 14:22:30.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/alltlobjects.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:32.955778 Netfoll-TL-2.0.0/netfoll_tl/tl/core/
--rw-rw-rw-   0        0        0     1130 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/core/__init__.py
--rw-rw-rw-   0        0        0     1361 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/core/gzippacked.py
--rw-rw-rw-   0        0        0     1810 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/core/messagecontainer.py
--rw-rw-rw-   0        0        0     1192 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/core/rpcresult.py
--rw-rw-rw-   0        0        0     1104 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/core/tlmessage.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:33.236823 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/
--rw-rw-rw-   0        0        0      524 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/__init__.py
--rw-rw-rw-   0        0        0    16703 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/adminlogevent.py
--rw-rw-rw-   0        0        0    12677 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/button.py
--rw-rw-rw-   0        0        0     5426 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/chatgetter.py
--rw-rw-rw-   0        0        0    19932 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/conversation.py
--rw-rw-rw-   0        0        0     5791 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/dialog.py
--rw-rw-rw-   0        0        0     6036 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/draft.py
--rw-rw-rw-   0        0        0     4375 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/file.py
--rw-rw-rw-   0        0        0     2180 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/forward.py
--rw-rw-rw-   0        0        0    17461 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlinebuilder.py
--rw-rw-rw-   0        0        0     6430 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlineresult.py
--rw-rw-rw-   0        0        0     2837 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlineresults.py
--rw-rw-rw-   0        0        0      319 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inputsizedfile.py
--rw-rw-rw-   0        0        0    44249 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/message.py
--rw-rw-rw-   0        0        0     6151 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/messagebutton.py
--rw-rw-rw-   0        0        0     4269 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/participantpermissions.py
--rw-rw-rw-   0        0        0     4324 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/qrlogin.py
--rw-rw-rw-   0        0        0     3956 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/custom/sendergetter.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:33.524829 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/
--rw-rw-rw-   0        0        0    17874 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/__init__.py
--rw-rw-rw-   0        0        0    85184 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/account.py
--rw-rw-rw-   0        0        0    22894 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/auth.py
--rw-rw-rw-   0        0        0    11698 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/bots.py
--rw-rw-rw-   0        0        0    76376 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/channels.py
--rw-rw-rw-   0        0        0    23340 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/contacts.py
--rw-rw-rw-   0        0        0     2290 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/folders.py
--rw-rw-rw-   0        0        0    16224 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/help.py
--rw-rw-rw-   0        0        0     5283 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/langpack.py
--rw-rw-rw-   0        0        0   279802 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/messages.py
--rw-rw-rw-   0        0        0    13062 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/payments.py
--rw-rw-rw-   0        0        0    44284 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/phone.py
--rw-rw-rw-   0        0        0    10350 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/photos.py
--rw-rw-rw-   0        0        0     7218 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/stats.py
--rw-rw-rw-   0        0        0    14907 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/stickers.py
--rw-rw-rw-   0        0        0     4188 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/updates.py
--rw-rw-rw-   0        0        0     9471 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/upload.py
--rw-rw-rw-   0        0        0     3716 2023-04-14 14:22:28.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/functions/users.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:33.540829 Netfoll-TL-2.0.0/netfoll_tl/tl/patched/
--rw-rw-rw-   0        0        0      572 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/patched/__init__.py
--rw-rw-rw-   0        0        0     7612 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/tlobject.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:22:33.854896 Netfoll-TL-2.0.0/netfoll_tl/tl/types/
--rw-rw-rw-   0        0        0  1641699 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/__init__.py
--rw-rw-rw-   0        0        0    39178 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/account.py
--rw-rw-rw-   0        0        0    26952 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/auth.py
--rw-rw-rw-   0        0        0     8527 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/channels.py
--rw-rw-rw-   0        0        0    15797 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/contacts.py
--rw-rw-rw-   0        0        0    33242 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/help.py
--rw-rw-rw-   0        0        0   101414 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/messages.py
--rw-rw-rw-   0        0        0    19156 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/payments.py
--rw-rw-rw-   0        0        0    11163 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/phone.py
--rw-rw-rw-   0        0        0     4464 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/photos.py
--rw-rw-rw-   0        0        0    14330 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/stats.py
--rw-rw-rw-   0        0        0      958 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/stickers.py
--rw-rw-rw-   0        0        0     3741 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/storage.py
--rw-rw-rw-   0        0        0    18123 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/updates.py
--rw-rw-rw-   0        0        0     6337 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/upload.py
--rw-rw-rw-   0        0        0     1979 2023-04-14 14:22:29.000000 Netfoll-TL-2.0.0/netfoll_tl/tl/types/users.py
--rw-rw-rw-   0        0        0       25 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/types.py
--rw-rw-rw-   0        0        0    56448 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/netfoll_tl/utils.py
--rw-rw-rw-   0        0        0       98 2023-04-14 14:22:08.000000 Netfoll-TL-2.0.0/netfoll_tl/version.py
--rw-rw-rw-   0        0        0     1202 2023-04-14 13:43:17.000000 Netfoll-TL-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:22:33.882898 Netfoll-TL-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     9116 2023-04-14 14:05:16.000000 Netfoll-TL-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:08.565979 Netfoll-TL-2.0.1/
+-rw-rw-rw-   0        0        0     1096 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:05.949464 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-04-30 12:34:04.000000 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4691 2023-04-30 12:34:04.000000 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:34:04.000000 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 12:34:04.000000 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 12:34:04.000000 Netfoll-TL-2.0.1/Netfoll_TL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      945 2023-04-30 12:34:08.562982 Netfoll-TL-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-04-30 12:22:52.000000 Netfoll-TL-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:06.135509 Netfoll-TL-2.0.1/netfoll_tl/
+-rw-rw-rw-   0        0        0      420 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:06.198512 Netfoll-TL-2.0.1/netfoll_tl/_updates/
+-rw-rw-rw-   0        0        0      173 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/_updates/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/_updates/entitycache.py
+-rw-rw-rw-   0        0        0    34827 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/_updates/messagebox.py
+-rw-rw-rw-   0        0        0     6363 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/_updates/session.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:06.499609 Netfoll-TL-2.0.1/netfoll_tl/client/
+-rw-rw-rw-   0        0        0     1225 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/__init__.py
+-rw-rw-rw-   0        0        0     9815 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/account.py
+-rw-rw-rw-   0        0        0    25488 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/auth.py
+-rw-rw-rw-   0        0        0     2525 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/bots.py
+-rw-rw-rw-   0        0        0     3376 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/buttons.py
+-rw-rw-rw-   0        0        0    53320 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/chats.py
+-rw-rw-rw-   0        0        0    23618 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/dialogs.py
+-rw-rw-rw-   0        0        0    40727 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/downloads.py
+-rw-rw-rw-   0        0        0     9620 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/messageparse.py
+-rw-rw-rw-   0        0        0    63451 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/messages.py
+-rw-rw-rw-   0        0        0    39473 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/telegrambaseclient.py
+-rw-rw-rw-   0        0        0      491 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/telegramclient.py
+-rw-rw-rw-   0        0        0    29176 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/updates.py
+-rw-rw-rw-   0        0        0    33752 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/uploads.py
+-rw-rw-rw-   0        0        0    25348 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/client/users.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:06.647581 Netfoll-TL-2.0.1/netfoll_tl/crypto/
+-rw-rw-rw-   0        0        0      359 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/aes.py
+-rw-rw-rw-   0        0        0     1258 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/aesctr.py
+-rw-rw-rw-   0        0        0     1950 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/authkey.py
+-rw-rw-rw-   0        0        0     3949 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/cdndecrypter.py
+-rw-rw-rw-   0        0        0     1700 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/factorization.py
+-rw-rw-rw-   0        0        0     4668 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/libssl.py
+-rw-rw-rw-   0        0        0     6690 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/crypto/rsa.py
+-rw-rw-rw-   0        0        0       26 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/custom.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:06.782587 Netfoll-TL-2.0.1/netfoll_tl/errors/
+-rw-rw-rw-   0        0        0     1705 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/errors/__init__.py
+-rw-rw-rw-   0        0        0     6665 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/errors/common.py
+-rw-rw-rw-   0        0        0     3601 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/errors/rpcbaseerrors.py
+-rw-rw-rw-   0        0        0   196260 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/errors/rpcerrorlist.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.011709 Netfoll-TL-2.0.1/netfoll_tl/events/
+-rw-rw-rw-   0        0        0     4415 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/__init__.py
+-rw-rw-rw-   0        0        0    13233 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/album.py
+-rw-rw-rw-   0        0        0    13768 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/callbackquery.py
+-rw-rw-rw-   0        0        0    18424 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/chataction.py
+-rw-rw-rw-   0        0        0     6501 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/common.py
+-rw-rw-rw-   0        0        0     9221 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/inlinequery.py
+-rw-rw-rw-   0        0        0     2185 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/messagedeleted.py
+-rw-rw-rw-   0        0        0     1938 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/messageedited.py
+-rw-rw-rw-   0        0        0     5613 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/messageread.py
+-rw-rw-rw-   0        0        0     9384 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/newmessage.py
+-rw-rw-rw-   0        0        0     1704 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/raw.py
+-rw-rw-rw-   0        0        0    10930 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/events/userupdate.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.096710 Netfoll-TL-2.0.1/netfoll_tl/extensions/
+-rw-rw-rw-   0        0        0      286 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/extensions/__init__.py
+-rw-rw-rw-   0        0        0     5930 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/extensions/binaryreader.py
+-rw-rw-rw-   0        0        0    11261 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/extensions/html.py
+-rw-rw-rw-   0        0        0     7050 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/extensions/markdown.py
+-rw-rw-rw-   0        0        0     4186 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/extensions/messagepacker.py
+-rw-rw-rw-   0        0        0       29 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/functions.py
+-rw-rw-rw-   0        0        0    15159 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/helpers.py
+-rw-rw-rw-   0        0        0     1629 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/hints.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.210719 Netfoll-TL-2.0.1/netfoll_tl/network/
+-rw-rw-rw-   0        0        0      599 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/__init__.py
+-rw-rw-rw-   0        0        0     8081 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/authenticator.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.359115 Netfoll-TL-2.0.1/netfoll_tl/network/connection/
+-rw-rw-rw-   0        0        0      435 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/__init__.py
+-rw-rw-rw-   0        0        0    16132 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/connection.py
+-rw-rw-rw-   0        0        0     1259 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/http.py
+-rw-rw-rw-   0        0        0      994 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpabridged.py
+-rw-rw-rw-   0        0        0     1785 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpfull.py
+-rw-rw-rw-   0        0        0     1420 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpintermediate.py
+-rw-rw-rw-   0        0        0     5431 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpmtproxy.py
+-rw-rw-rw-   0        0        0     2065 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpobfuscated.py
+-rw-rw-rw-   0        0        0     2075 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/mtprotoplainsender.py
+-rw-rw-rw-   0        0        0    39048 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/mtprotosender.py
+-rw-rw-rw-   0        0        0    11247 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/mtprotostate.py
+-rw-rw-rw-   0        0        0      663 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/network/requeststate.py
+-rw-rw-rw-   0        0        0     7388 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/password.py
+-rw-rw-rw-   0        0        0     4520 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/requestiter.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.453548 Netfoll-TL-2.0.1/netfoll_tl/sessions/
+-rw-rw-rw-   0        0        0      136 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sessions/__init__.py
+-rw-rw-rw-   0        0        0     5263 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sessions/abstract.py
+-rw-rw-rw-   0        0        0     8567 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sessions/memory.py
+-rw-rw-rw-   0        0        0    12952 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sessions/sqlite.py
+-rw-rw-rw-   0        0        0     2053 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sessions/string.py
+-rw-rw-rw-   0        0        0     2683 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.486302 Netfoll-TL-2.0.1/netfoll_tl/tl/
+-rw-rw-rw-   0        0        0       43 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/__init__.py
+-rw-rw-rw-   0        0        0    82964 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/alltlobjects.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.562069 Netfoll-TL-2.0.1/netfoll_tl/tl/core/
+-rw-rw-rw-   0        0        0     1130 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/core/__init__.py
+-rw-rw-rw-   0        0        0     1361 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/core/gzippacked.py
+-rw-rw-rw-   0        0        0     1810 2023-04-30 12:18:30.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/core/messagecontainer.py
+-rw-rw-rw-   0        0        0     1192 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/core/rpcresult.py
+-rw-rw-rw-   0        0        0     1104 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/core/tlmessage.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:07.939081 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/
+-rw-rw-rw-   0        0        0      524 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/__init__.py
+-rw-rw-rw-   0        0        0    16703 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/adminlogevent.py
+-rw-rw-rw-   0        0        0    12677 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/button.py
+-rw-rw-rw-   0        0        0     5426 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/chatgetter.py
+-rw-rw-rw-   0        0        0    19932 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/conversation.py
+-rw-rw-rw-   0        0        0     5791 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/dialog.py
+-rw-rw-rw-   0        0        0     6036 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/draft.py
+-rw-rw-rw-   0        0        0     4375 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/file.py
+-rw-rw-rw-   0        0        0     2180 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/forward.py
+-rw-rw-rw-   0        0        0    17461 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlinebuilder.py
+-rw-rw-rw-   0        0        0     6430 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlineresult.py
+-rw-rw-rw-   0        0        0     2837 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlineresults.py
+-rw-rw-rw-   0        0        0      319 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inputsizedfile.py
+-rw-rw-rw-   0        0        0    44249 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/message.py
+-rw-rw-rw-   0        0        0     6151 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/messagebutton.py
+-rw-rw-rw-   0        0        0     4269 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/participantpermissions.py
+-rw-rw-rw-   0        0        0     4324 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/qrlogin.py
+-rw-rw-rw-   0        0        0     3956 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/custom/sendergetter.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:08.201967 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/
+-rw-rw-rw-   0        0        0    17874 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/__init__.py
+-rw-rw-rw-   0        0        0    85184 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/account.py
+-rw-rw-rw-   0        0        0    22894 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/auth.py
+-rw-rw-rw-   0        0        0    11698 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/bots.py
+-rw-rw-rw-   0        0        0    76376 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/channels.py
+-rw-rw-rw-   0        0        0    23340 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/contacts.py
+-rw-rw-rw-   0        0        0     2290 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/folders.py
+-rw-rw-rw-   0        0        0    16224 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/help.py
+-rw-rw-rw-   0        0        0     5283 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/langpack.py
+-rw-rw-rw-   0        0        0   279802 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/messages.py
+-rw-rw-rw-   0        0        0    13062 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/payments.py
+-rw-rw-rw-   0        0        0    44284 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/phone.py
+-rw-rw-rw-   0        0        0    10350 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/photos.py
+-rw-rw-rw-   0        0        0     7218 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/stats.py
+-rw-rw-rw-   0        0        0    14907 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/stickers.py
+-rw-rw-rw-   0        0        0     4188 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/updates.py
+-rw-rw-rw-   0        0        0     9471 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/upload.py
+-rw-rw-rw-   0        0        0     3716 2023-04-30 12:34:02.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/functions/users.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:08.217971 Netfoll-TL-2.0.1/netfoll_tl/tl/patched/
+-rw-rw-rw-   0        0        0      572 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/patched/__init__.py
+-rw-rw-rw-   0        0        0     7612 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/tlobject.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:34:08.555978 Netfoll-TL-2.0.1/netfoll_tl/tl/types/
+-rw-rw-rw-   0        0        0  1641699 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/__init__.py
+-rw-rw-rw-   0        0        0    39178 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/account.py
+-rw-rw-rw-   0        0        0    26952 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/auth.py
+-rw-rw-rw-   0        0        0     8527 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/channels.py
+-rw-rw-rw-   0        0        0    15797 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/contacts.py
+-rw-rw-rw-   0        0        0    33242 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/help.py
+-rw-rw-rw-   0        0        0   101414 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/messages.py
+-rw-rw-rw-   0        0        0    19156 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/payments.py
+-rw-rw-rw-   0        0        0    11163 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/phone.py
+-rw-rw-rw-   0        0        0     4464 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/photos.py
+-rw-rw-rw-   0        0        0    14330 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/stats.py
+-rw-rw-rw-   0        0        0      958 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/stickers.py
+-rw-rw-rw-   0        0        0     3741 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/storage.py
+-rw-rw-rw-   0        0        0    18123 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/updates.py
+-rw-rw-rw-   0        0        0     6337 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/upload.py
+-rw-rw-rw-   0        0        0     1979 2023-04-30 12:34:03.000000 Netfoll-TL-2.0.1/netfoll_tl/tl/types/users.py
+-rw-rw-rw-   0        0        0       25 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/types.py
+-rw-rw-rw-   0        0        0    56448 2023-04-30 12:18:31.000000 Netfoll-TL-2.0.1/netfoll_tl/utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-30 12:33:35.000000 Netfoll-TL-2.0.1/netfoll_tl/version.py
+-rw-rw-rw-   0        0        0     1202 2023-04-30 12:28:24.000000 Netfoll-TL-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 12:34:08.566980 Netfoll-TL-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     9085 2023-04-30 12:33:50.000000 Netfoll-TL-2.0.1/setup.py
```

### Comparing `Netfoll-TL-2.0.0/LICENSE` & `Netfoll-TL-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/Netfoll_TL.egg-info/SOURCES.txt` & `Netfoll-TL-2.0.1/Netfoll_TL.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 pyproject.toml
 setup.py
 Netfoll_TL.egg-info/PKG-INFO
 Netfoll_TL.egg-info/SOURCES.txt
 Netfoll_TL.egg-info/dependency_links.txt
 Netfoll_TL.egg-info/requires.txt
 Netfoll_TL.egg-info/top_level.txt
```

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/_updates/entitycache.py` & `Netfoll-TL-2.0.1/netfoll_tl/_updates/entitycache.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/_updates/messagebox.py` & `Netfoll-TL-2.0.1/netfoll_tl/_updates/messagebox.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/_updates/session.py` & `Netfoll-TL-2.0.1/netfoll_tl/_updates/session.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/account.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/account.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/auth.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/auth.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/bots.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/bots.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/buttons.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/buttons.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/chats.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/chats.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/dialogs.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/dialogs.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/downloads.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/downloads.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/messageparse.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/messageparse.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/messages.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/messages.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/telegrambaseclient.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/telegrambaseclient.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/updates.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/updates.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/uploads.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/uploads.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/client/users.py` & `Netfoll-TL-2.0.1/netfoll_tl/client/users.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/aes.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/aesctr.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/aesctr.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/authkey.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/authkey.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/cdndecrypter.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/cdndecrypter.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/factorization.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/factorization.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/libssl.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/libssl.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/crypto/rsa.py` & `Netfoll-TL-2.0.1/netfoll_tl/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/errors/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/errors/common.py` & `Netfoll-TL-2.0.1/netfoll_tl/errors/common.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/errors/rpcbaseerrors.py` & `Netfoll-TL-2.0.1/netfoll_tl/errors/rpcbaseerrors.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/errors/rpcerrorlist.py` & `Netfoll-TL-2.0.1/netfoll_tl/errors/rpcerrorlist.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/album.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/album.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/callbackquery.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/callbackquery.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/chataction.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/chataction.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/common.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/common.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/inlinequery.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/inlinequery.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/messagedeleted.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/messagedeleted.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/messageedited.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/messageedited.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/messageread.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/messageread.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/newmessage.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/raw.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/raw.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/events/userupdate.py` & `Netfoll-TL-2.0.1/netfoll_tl/events/userupdate.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/extensions/binaryreader.py` & `Netfoll-TL-2.0.1/netfoll_tl/extensions/binaryreader.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/extensions/html.py` & `Netfoll-TL-2.0.1/netfoll_tl/extensions/html.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/extensions/markdown.py` & `Netfoll-TL-2.0.1/netfoll_tl/extensions/markdown.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/extensions/messagepacker.py` & `Netfoll-TL-2.0.1/netfoll_tl/extensions/messagepacker.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/helpers.py` & `Netfoll-TL-2.0.1/netfoll_tl/helpers.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/hints.py` & `Netfoll-TL-2.0.1/netfoll_tl/hints.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/authenticator.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/authenticator.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/connection.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/connection.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/http.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/http.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpabridged.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpabridged.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpfull.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpfull.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpintermediate.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpintermediate.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpmtproxy.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpmtproxy.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/connection/tcpobfuscated.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/connection/tcpobfuscated.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/mtprotoplainsender.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/mtprotoplainsender.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/mtprotosender.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/mtprotosender.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/mtprotostate.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/mtprotostate.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/network/requeststate.py` & `Netfoll-TL-2.0.1/netfoll_tl/network/requeststate.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/password.py` & `Netfoll-TL-2.0.1/netfoll_tl/password.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/requestiter.py` & `Netfoll-TL-2.0.1/netfoll_tl/requestiter.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/sessions/abstract.py` & `Netfoll-TL-2.0.1/netfoll_tl/sessions/abstract.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/sessions/memory.py` & `Netfoll-TL-2.0.1/netfoll_tl/sessions/memory.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/sessions/sqlite.py` & `Netfoll-TL-2.0.1/netfoll_tl/sessions/sqlite.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/sessions/string.py` & `Netfoll-TL-2.0.1/netfoll_tl/sessions/string.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/sync.py` & `Netfoll-TL-2.0.1/netfoll_tl/sync.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/alltlobjects.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/alltlobjects.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/core/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/core/gzippacked.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/core/gzippacked.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/core/messagecontainer.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/core/messagecontainer.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/core/rpcresult.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/core/rpcresult.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/core/tlmessage.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/core/tlmessage.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/adminlogevent.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/adminlogevent.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/button.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/button.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/chatgetter.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/chatgetter.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/conversation.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/conversation.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/dialog.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/dialog.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/draft.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/draft.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/file.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/file.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/forward.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/forward.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlinebuilder.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlinebuilder.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlineresult.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlineresult.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/inlineresults.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/inlineresults.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/message.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/message.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/messagebutton.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/messagebutton.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/participantpermissions.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/participantpermissions.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/qrlogin.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/qrlogin.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/custom/sendergetter.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/custom/sendergetter.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/account.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/account.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/auth.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/auth.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/bots.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/bots.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/channels.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/channels.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/contacts.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/contacts.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/folders.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/folders.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/help.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/help.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/langpack.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/langpack.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/messages.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/messages.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/payments.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/payments.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/phone.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/phone.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/photos.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/photos.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/stats.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/stats.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/stickers.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/stickers.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/updates.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/updates.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/upload.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/upload.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/functions/users.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/functions/users.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/patched/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/patched/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/tlobject.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/tlobject.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/__init__.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/account.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/account.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/auth.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/auth.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/channels.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/channels.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/contacts.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/contacts.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/help.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/help.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/messages.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/messages.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/payments.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/payments.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/phone.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/phone.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/photos.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/photos.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/stats.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/stats.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/stickers.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/stickers.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/storage.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/storage.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/updates.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/updates.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/upload.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/upload.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/tl/types/users.py` & `Netfoll-TL-2.0.1/netfoll_tl/tl/types/users.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/netfoll_tl/utils.py` & `Netfoll-TL-2.0.1/netfoll_tl/utils.py`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/pyproject.toml` & `Netfoll-TL-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Netfoll-TL-2.0.0/setup.py` & `Netfoll-TL-2.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,243 +21,252 @@
 from subprocess import run
 
 from setuptools import find_packages, setup
 
 # Needed since we're importing local files
 sys.path.insert(0, os.path.dirname(__file__))
 
+
 class TempWorkDir:
     """Switches the working directory to be the one on which this file lives,
-       while within the 'with' block.
+    while within the 'with' block.
     """
+
     def __init__(self, new=None):
         self.original = None
         self.new = new or str(Path(__file__).parent.resolve())
 
     def __enter__(self):
         # os.chdir does not work with Path in Python 3.5.x
-        self.original = str(Path('.').resolve())
+        self.original = str(Path(".").resolve())
         os.makedirs(self.new, exist_ok=True)
         os.chdir(self.new)
         return self
 
     def __exit__(self, *args):
         os.chdir(self.original)
 
 
-API_REF_URL = 'https://tl.telethon.dev/'
+API_REF_URL = "https://tl.telethon.dev/"
 
-GENERATOR_DIR = Path('telethon_generator')
-LIBRARY_DIR = Path('netfoll_tl')
+GENERATOR_DIR = Path("telethon_generator")
+LIBRARY_DIR = Path("netfoll_tl")
 
-ERRORS_IN = GENERATOR_DIR / 'data/errors.csv'
-ERRORS_OUT = LIBRARY_DIR / 'errors/rpcerrorlist.py'
+ERRORS_IN = GENERATOR_DIR / "data/errors.csv"
+ERRORS_OUT = LIBRARY_DIR / "errors/rpcerrorlist.py"
 
-METHODS_IN = GENERATOR_DIR / 'data/methods.csv'
+METHODS_IN = GENERATOR_DIR / "data/methods.csv"
 
 # Which raw API methods are covered by *friendly* methods in the client?
-FRIENDLY_IN = GENERATOR_DIR / 'data/friendly.csv'
+FRIENDLY_IN = GENERATOR_DIR / "data/friendly.csv"
 
-TLOBJECT_IN_TLS = [Path(x) for x in GENERATOR_DIR.glob('data/*.tl')]
-TLOBJECT_OUT = LIBRARY_DIR / 'tl'
+TLOBJECT_IN_TLS = [Path(x) for x in GENERATOR_DIR.glob("data/*.tl")]
+TLOBJECT_OUT = LIBRARY_DIR / "tl"
 IMPORT_DEPTH = 2
 
-DOCS_IN_RES = GENERATOR_DIR / 'data/html'
-DOCS_OUT = Path('docs')
+DOCS_IN_RES = GENERATOR_DIR / "data/html"
+DOCS_OUT = Path("docs")
 
 
-def generate(which, action='gen'):
-    from telethon_generator.parsers import\
-        parse_errors, parse_methods, parse_tl, find_layer
-
-    from telethon_generator.generators import\
-        generate_errors, generate_tlobjects, generate_docs, clean_tlobjects
+def generate(which, action="gen"):
+    from telethon_generator.parsers import (
+        parse_errors,
+        parse_methods,
+        parse_tl,
+        find_layer,
+    )
+
+    from telethon_generator.generators import (
+        generate_errors,
+        generate_tlobjects,
+        generate_docs,
+        clean_tlobjects,
+    )
 
     layer = next(filter(None, map(find_layer, TLOBJECT_IN_TLS)))
     errors = list(parse_errors(ERRORS_IN))
-    methods = list(parse_methods(METHODS_IN, FRIENDLY_IN, {e.str_code: e for e in errors}))
-
-    tlobjects = list(itertools.chain(*(
-        parse_tl(file, layer, methods) for file in TLOBJECT_IN_TLS)))
+    methods = list(
+        parse_methods(METHODS_IN, FRIENDLY_IN, {e.str_code: e for e in errors})
+    )
+
+    tlobjects = list(
+        itertools.chain(*(parse_tl(file, layer, methods) for file in TLOBJECT_IN_TLS))
+    )
 
     if not which:
-        which.extend(('tl', 'errors'))
+        which.extend(("tl", "errors"))
 
-    clean = action == 'clean'
-    action = 'Cleaning' if clean else 'Generating'
+    clean = action == "clean"
+    action = "Cleaning" if clean else "Generating"
 
-    if 'all' in which:
-        which.remove('all')
-        for x in ('tl', 'errors', 'docs'):
+    if "all" in which:
+        which.remove("all")
+        for x in ("tl", "errors", "docs"):
             if x not in which:
                 which.append(x)
 
-    if 'tl' in which:
-        which.remove('tl')
-        print(action, 'TLObjects...')
+    if "tl" in which:
+        which.remove("tl")
+        print(action, "TLObjects...")
         if clean:
             clean_tlobjects(TLOBJECT_OUT)
         else:
             generate_tlobjects(tlobjects, layer, IMPORT_DEPTH, TLOBJECT_OUT)
 
-    if 'errors' in which:
-        which.remove('errors')
-        print(action, 'RPCErrors...')
+    if "errors" in which:
+        which.remove("errors")
+        print(action, "RPCErrors...")
         if clean:
             if ERRORS_OUT.is_file():
                 ERRORS_OUT.unlink()
         else:
-            with ERRORS_OUT.open('w') as file:
+            with ERRORS_OUT.open("w") as file:
                 generate_errors(errors, file)
 
-    if 'docs' in which:
-        which.remove('docs')
-        print(action, 'documentation...')
+    if "docs" in which:
+        which.remove("docs")
+        print(action, "documentation...")
         if clean:
             if DOCS_OUT.is_dir():
                 shutil.rmtree(str(DOCS_OUT))
         else:
             in_path = DOCS_IN_RES.resolve()
             with TempWorkDir(DOCS_OUT):
                 generate_docs(tlobjects, methods, layer, in_path)
 
-    if 'json' in which:
-        which.remove('json')
-        print(action, 'JSON schema...')
-        json_files = [x.with_suffix('.json') for x in TLOBJECT_IN_TLS]
+    if "json" in which:
+        which.remove("json")
+        print(action, "JSON schema...")
+        json_files = [x.with_suffix(".json") for x in TLOBJECT_IN_TLS]
         if clean:
             for file in json_files:
                 if file.is_file():
                     file.unlink()
         else:
+
             def gen_json(fin, fout):
                 meths = []
                 constructors = []
                 for tl in parse_tl(fin, layer):
                     if tl.is_function:
                         meths.append(tl.to_dict())
                     else:
                         constructors.append(tl.to_dict())
-                what = {'constructors': constructors, 'methods': meths}
-                with open(fout, 'w') as f:
+                what = {"constructors": constructors, "methods": meths}
+                with open(fout, "w") as f:
                     json.dump(what, f, indent=2)
 
             for fs in zip(TLOBJECT_IN_TLS, json_files):
                 gen_json(*fs)
 
     if which:
         print(
-            'The following items were not understood:', which,
+            "The following items were not understood:",
+            which,
             '\n  Consider using only "tl", "errors" and/or "docs".'
             '\n  Using only "clean" will clean them. "all" to act on all.'
-            '\n  For instance "gen tl errors".'
+            '\n  For instance "gen tl errors".',
         )
 
 
 def main(argv):
-    if len(argv) >= 2 and argv[1] in ('gen', 'clean'):
+    if len(argv) >= 2 and argv[1] in ("gen", "clean"):
         generate(argv[2:], argv[1])
 
-    elif len(argv) >= 2 and argv[1] == 'pypi':
+    elif len(argv) >= 2 and argv[1] == "pypi":
         # Make sure tl.telethon.dev is up-to-date first
         with urllib.request.urlopen(API_REF_URL) as resp:
             html = resp.read()
-            m = re.search(br'layer\s+(\d+)', html)
+            m = re.search(rb"layer\s+(\d+)", html)
             if not m:
-                print('Failed to check that the API reference is up to date:', API_REF_URL)
+                print(
+                    "Failed to check that the API reference is up to date:", API_REF_URL
+                )
                 return
 
             from telethon_generator.parsers import find_layer
+
             layer = next(filter(None, map(find_layer, TLOBJECT_IN_TLS)))
             published_layer = int(m[1])
             if published_layer != layer:
-                print('Published layer', published_layer, 'does not match current layer', layer, '.')
-                print('Make sure to update the API reference site first:', API_REF_URL)
+                print(
+                    "Published layer",
+                    published_layer,
+                    "does not match current layer",
+                    layer,
+                    ".",
+                )
+                print("Make sure to update the API reference site first:", API_REF_URL)
                 return
 
         # (Re)generate the code to make sure we don't push without it
-        generate(['tl', 'errors'])
+        generate(["tl", "errors"])
 
         # Try importing the telethon module to assert it has no errors
         try:
             import netfoll_tl
         except:
-            print('Packaging for PyPi aborted, importing the module failed.')
+            print("Packaging for PyPi aborted, importing the module failed.")
             return
 
-        remove_dirs = ['__pycache__', 'build', 'dist', 'Netfoll_TL.egg-info']
+        remove_dirs = ["__pycache__", "build", "dist", "Netfoll_TL.egg-info"]
         for root, _dirs, _files in os.walk(LIBRARY_DIR, topdown=False):
             # setuptools is including __pycache__ for some reason (#1605)
-            if root.endswith('/__pycache__'):
+            if root.endswith("/__pycache__"):
                 remove_dirs.append(root)
         for x in remove_dirs:
             shutil.rmtree(x, ignore_errors=True)
 
-        run('python setup.py sdist', shell=True)
-        run('python setup.py bdist_wheel', shell=True)
-        run('twine upload dist/*', shell=True)
-        for x in ('build', 'dist', 'Netfoll_TL.egg-info'):
+        run("python setup.py sdist", shell=True)
+        run("python setup.py bdist_wheel", shell=True)
+        run("twine upload dist/*", shell=True)
+        for x in ("build", "dist", "Netfoll_TL.egg-info"):
             shutil.rmtree(x, ignore_errors=True)
 
     else:
         # e.g. install from GitHub
         if GENERATOR_DIR.is_dir():
-            generate(['tl', 'errors'])
+            generate(["tl", "errors"])
 
         # Get the long description from the README file
-        with open('README.rst', 'r', encoding='utf-8') as f:
+        with open("README.md", "r", encoding="utf-8") as f:
             long_description = f.read()
 
-        with open('netfoll_tl/version.py', 'r', encoding='utf-8') as f:
-            version = re.search(r"^__version__\s*=\s*'(.*)'.*$",
-                                f.read(), flags=re.MULTILINE).group(1)
+        version = "2.0.1"
         setup(
-            name='Netfoll-TL',
+            name="Netfoll-TL",
             version=version,
             description="Modified Telethon",
             long_description=long_description,
-
-            url='https://github.com/yaroslav1734/Netfoll-TL',
-            download_url='https://github.com/yaroslav1734/Netfoll-TL/releases',
-
-            author='Lonami Exo',
-            author_email='totufals@hotmail.com',
-
-            license='MIT',
-
+            url="https://github.com/Netfoll/Netfoll-TL",
+            download_url="https://github.com/Netfoll/Netfoll-TL/releases",
+            author="ASNCT",
+            license="MIT",
             # See https://stackoverflow.com/a/40300957/4759433
             # -> https://www.python.org/dev/peps/pep-0345/#requires-python
             # -> http://setuptools.readthedocs.io/en/latest/setuptools.html
-            python_requires='>=3.5',
-
+            python_requires=">=3.5",
             # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
             classifiers=[
                 #   3 - Alpha
                 #   4 - Beta
                 #   5 - Production/Stable
-                'Development Status :: 5 - Production/Stable',
-
-                'Intended Audience :: Developers',
-                'Topic :: Communications :: Chat',
-
-                'License :: OSI Approved :: MIT License',
-
-                'Programming Language :: Python :: 3',
-                'Programming Language :: Python :: 3.5',
-                'Programming Language :: Python :: 3.6',
-                'Programming Language :: Python :: 3.7',
-                'Programming Language :: Python :: 3.8',
+                "Development Status :: 5 - Production/Stable",
+                "Intended Audience :: Developers",
+                "Topic :: Communications :: Chat",
+                "License :: OSI Approved :: MIT License",
+                "Programming Language :: Python :: 3",
+                "Programming Language :: Python :: 3.5",
+                "Programming Language :: Python :: 3.6",
+                "Programming Language :: Python :: 3.7",
+                "Programming Language :: Python :: 3.8",
             ],
-            keywords='telegram api chat client library messaging mtproto',
-            packages=find_packages(exclude=[
-                'telethon_*', 'tests*'
-            ]),
-            install_requires=['pyaes', 'rsa'],
-            extras_require={
-                'cryptg': ['cryptg']
-            }
+            keywords="telegram api chat client library messaging mtproto netfoll telethon tl",
+            packages=find_packages(exclude=["telethon_*", "tests*"]),
+            install_requires=["pyaes", "rsa"],
+            extras_require={"cryptg": ["cryptg"]},
         )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     with TempWorkDir():
         main(sys.argv)
```

