# Comparing `tmp/kutil_jakubaugustyn-0.0.5.tar.gz` & `tmp/kutil_jakubaugustyn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kutil_jakubaugustyn-0.0.5.tar", last modified: Tue Apr 16 11:20:33 2024, max compression
+gzip compressed data, was "kutil_jakubaugustyn-0.0.6.tar", last modified: Sat Apr 20 12:58:30 2024, max compression
```

## Comparing `kutil_jakubaugustyn-0.0.5.tar` & `kutil_jakubaugustyn-0.0.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:33.117306 kutil_jakubaugustyn-0.0.5/
--rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 kutil_jakubaugustyn-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1374 2024-04-16 11:20:33.117306 kutil_jakubaugustyn-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-02-28 16:16:37.000000 kutil_jakubaugustyn-0.0.5/README.md
--rw-rw-rw-   0        0        0      824 2024-04-16 11:10:31.000000 kutil_jakubaugustyn-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 11:20:33.117306 kutil_jakubaugustyn-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.664207 kutil_jakubaugustyn-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:33.101686 kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/
--rw-rw-rw-   0        0        0     1374 2024-04-16 11:20:32.000000 kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3719 2024-04-16 11:20:32.000000 kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:20:32.000000 kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-16 11:20:32.000000 kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.695464 kutil_jakubaugustyn-0.0.5/src/kutil/
--rw-rw-rw-   0        0        0      302 2024-02-28 19:22:19.000000 kutil_jakubaugustyn-0.0.5/src/kutil/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.711089 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/
--rw-rw-rw-   0        0        0     2401 2023-12-18 18:55:31.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/BidirectionalByteArray.py
--rw-rw-rw-   0        0        0     4303 2024-03-25 17:59:57.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/ByteBuffer.py
--rw-rw-rw-   0        0        0     5333 2024-03-02 12:29:40.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/DataBuffer.py
--rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/Serializable.py
--rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/TextOutput.py
--rw-rw-rw-   0        0        0      335 2024-03-02 12:31:14.000000 kutil_jakubaugustyn-0.0.5/src/kutil/buffer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.726711 kutil_jakubaugustyn-0.0.5/src/kutil/io/
--rw-rw-rw-   0        0        0      262 2024-04-16 09:37:01.000000 kutil_jakubaugustyn-0.0.5/src/kutil/io/__init__.py
--rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 kutil_jakubaugustyn-0.0.5/src/kutil/io/directory.py
--rw-rw-rw-   0        0        0     3568 2024-04-16 09:35:52.000000 kutil_jakubaugustyn-0.0.5/src/kutil/io/file.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.757960 kutil_jakubaugustyn-0.0.5/src/kutil/language/
--rw-rw-rw-   0        0        0     4560 2024-02-28 19:21:38.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/AST.py
--rw-rw-rw-   0        0        0     5769 2024-01-13 18:03:43.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/BytecodeFile.py
--rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Compiler.py
--rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Error.py
--rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Interpreter.py
--rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Language.py
--rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Lexer.py
--rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Options.py
--rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Parser.py
--rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Stack.py
--rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/Token.py
--rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.757960 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/
--rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/BrainFuck.py
--rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.789207 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/
--rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSLexer.py
--rw-rw-rw-   0        0        0     1565 2024-01-22 17:04:30.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSOptions.py
--rw-rw-rw-   0        0        0   142027 2024-02-11 14:35:27.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSParser.py
--rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/Javascript.py
--rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/__init__.py
--rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/character.py
--rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/error_handler.py
--rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/messages.py
--rw-rw-rw-   0        0        0    42770 2024-02-21 12:59:35.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/nodes.py
--rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/syntax.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.804831 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/
--rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/Canvas.py
--rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/Employee.py
--rw-rw-rw-   0        0        0    11803 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTCompiler.py
--rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
--rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTLexer.py
--rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTParser.py
--rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
--rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.820455 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/
--rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
--rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/boss.py
--rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
--rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/painter.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.851703 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/
--rw-rw-rw-   0        0        0     1378 2024-03-02 14:21:02.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/AbstractProtocol.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.867317 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/
--rw-rw-rw-   0        0        0     1216 2024-03-02 10:37:15.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPHeaders.py
--rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPMethod.py
--rw-rw-rw-   0        0        0     3822 2024-03-02 10:54:44.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPRequest.py
--rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPResponse.py
--rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/__init__.py
--rw-rw-rw-   0        0        0     1261 2024-03-02 13:51:31.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPConnection.py
--rw-rw-rw-   0        0        0    12459 2024-03-31 19:30:22.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPSConnection.py
--rw-rw-rw-   0        0        0     5991 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPServer.py
--rw-rw-rw-   0        0        0     7923 2024-03-28 17:23:06.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/ProtocolConnection.py
--rw-rw-rw-   0        0        0     2589 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/ProtocolServer.py
--rw-rw-rw-   0        0        0      944 2024-03-02 10:48:15.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TCPConnection.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.929861 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/
--rw-rw-rw-   0        0        0     2388 2024-03-28 17:36:36.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/AlertCause.py
--rw-rw-rw-   0        0        0     4694 2024-03-29 11:04:02.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/CipherSuite.py
--rw-rw-rw-   0        0        0     5969 2024-03-29 12:13:33.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/ConnectionState.py
--rw-rw-rw-   0        0        0     4200 2024-03-28 16:44:17.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/RawTLSRecord.py
--rw-rw-rw-   0        0        0       65 2024-03-02 10:25:01.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/__init__.py
--rw-rw-rw-   0        0        0     1851 2024-03-29 08:57:18.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/certificate_verifier.py
--rw-rw-rw-   0        0        0     6240 2024-03-28 06:30:56.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/extensions.py
--rw-rw-rw-   0        0        0    12644 2024-03-29 11:00:58.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/messages.py
--rw-rw-rw-   0        0        0     5135 2024-03-28 05:52:47.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/records.py
--rw-rw-rw-   0        0        0    13034 2024-03-28 11:30:36.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/tls_cryptography.py
--rw-rw-rw-   0        0        0      918 2024-04-15 18:08:31.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/URLSearchParams.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.945449 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WS/
--rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WS/WSMessage.py
--rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WS/__init__.py
--rw-rw-rw-   0        0        0     2753 2024-03-02 14:32:31.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WSConnection.py
--rw-rw-rw-   0        0        0      628 2024-03-02 10:33:58.000000 kutil_jakubaugustyn-0.0.5/src/kutil/protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.961080 kutil_jakubaugustyn-0.0.5/src/kutil/storage/
--rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/Cache.py
--rw-rw-rw-   0        0        0     6611 2024-03-01 16:41:47.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/Config.py
--rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:32.992334 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/
--rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/__init__.py
--rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/bon.py
--rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/converter.py
--rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/decoder.py
--rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/encoder.py
--rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/shared.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:33.007932 kutil_jakubaugustyn-0.0.5/src/kutil/threads/
--rw-rw-rw-   0        0        0     1721 2023-12-26 07:13:22.000000 kutil_jakubaugustyn-0.0.5/src/kutil/threads/ThreadWaiter.py
--rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 kutil_jakubaugustyn-0.0.5/src/kutil/threads/__init__.py
--rw-rw-rw-   0        0        0    15510 2024-03-02 11:13:45.000000 kutil_jakubaugustyn-0.0.5/src/kutil/typing_help.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:33.054803 kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/
--rw-rw-rw-   0        0        0    24555 2024-04-16 09:56:15.000000 kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/MapyCZServer.py
--rw-rw-rw-   0        0        0     3167 2024-04-16 08:53:51.000000 kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/WebScraperServer.py
--rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:20:33.101686 kutil_jakubaugustyn-0.0.5/tests/
--rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 kutil_jakubaugustyn-0.0.5/tests/test_bon.py
--rw-rw-rw-   0        0        0      756 2024-03-02 10:48:38.000000 kutil_jakubaugustyn-0.0.5/tests/test_bytebuffer.py
--rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 kutil_jakubaugustyn-0.0.5/tests/test_js.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 kutil_jakubaugustyn-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1374 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-02-28 16:16:37.000000 kutil_jakubaugustyn-0.0.6/README.md
+-rw-rw-rw-   0        0        0      824 2024-04-20 12:58:01.000000 kutil_jakubaugustyn-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.878123 kutil_jakubaugustyn-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/
+-rw-rw-rw-   0        0        0     1374 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3719 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.915879 kutil_jakubaugustyn-0.0.6/src/kutil/
+-rw-rw-rw-   0        0        0      302 2024-02-28 19:22:19.000000 kutil_jakubaugustyn-0.0.6/src/kutil/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.947132 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/
+-rw-rw-rw-   0        0        0     2401 2023-12-18 18:55:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/BidirectionalByteArray.py
+-rw-rw-rw-   0        0        0     4303 2024-03-25 17:59:57.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/ByteBuffer.py
+-rw-rw-rw-   0        0        0     5333 2024-03-02 12:29:40.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/DataBuffer.py
+-rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/Serializable.py
+-rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/TextOutput.py
+-rw-rw-rw-   0        0        0      335 2024-03-02 12:31:14.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.962756 kutil_jakubaugustyn-0.0.6/src/kutil/io/
+-rw-rw-rw-   0        0        0      262 2024-04-16 09:37:01.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/directory.py
+-rw-rw-rw-   0        0        0     3568 2024-04-16 09:35:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/file.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.016150 kutil_jakubaugustyn-0.0.6/src/kutil/language/
+-rw-rw-rw-   0        0        0     4560 2024-02-28 19:21:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/AST.py
+-rw-rw-rw-   0        0        0     5769 2024-01-13 18:03:43.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/BytecodeFile.py
+-rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Compiler.py
+-rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Error.py
+-rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Interpreter.py
+-rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Language.py
+-rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Lexer.py
+-rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Options.py
+-rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Parser.py
+-rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Stack.py
+-rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Token.py
+-rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.031779 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/
+-rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/BrainFuck.py
+-rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.078649 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/
+-rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSLexer.py
+-rw-rw-rw-   0        0        0     1565 2024-01-22 17:04:30.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSOptions.py
+-rw-rw-rw-   0        0        0   142027 2024-02-11 14:35:27.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSParser.py
+-rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/Javascript.py
+-rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/__init__.py
+-rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/character.py
+-rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/error_handler.py
+-rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/messages.py
+-rw-rw-rw-   0        0        0    42770 2024-02-21 12:59:35.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/nodes.py
+-rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.116414 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/
+-rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Canvas.py
+-rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Employee.py
+-rw-rw-rw-   0        0        0    11803 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTCompiler.py
+-rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
+-rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTLexer.py
+-rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTParser.py
+-rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
+-rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.147670 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/
+-rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
+-rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/boss.py
+-rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
+-rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/painter.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.178915 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/
+-rw-rw-rw-   0        0        0     1378 2024-03-02 14:21:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/AbstractProtocol.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.263549 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/
+-rw-rw-rw-   0        0        0     1216 2024-03-02 10:37:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPHeaders.py
+-rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPMethod.py
+-rw-rw-rw-   0        0        0     3822 2024-03-02 10:54:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPRequest.py
+-rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPResponse.py
+-rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/__init__.py
+-rw-rw-rw-   0        0        0     1261 2024-03-02 13:51:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPConnection.py
+-rw-rw-rw-   0        0        0    12459 2024-03-31 19:30:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPSConnection.py
+-rw-rw-rw-   0        0        0     5991 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPServer.py
+-rw-rw-rw-   0        0        0     7923 2024-03-28 17:23:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolConnection.py
+-rw-rw-rw-   0        0        0     2589 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolServer.py
+-rw-rw-rw-   0        0        0      944 2024-03-02 10:48:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TCPConnection.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.464097 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/
+-rw-rw-rw-   0        0        0     2388 2024-03-28 17:36:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/AlertCause.py
+-rw-rw-rw-   0        0        0     4694 2024-03-29 11:04:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/CipherSuite.py
+-rw-rw-rw-   0        0        0     5969 2024-03-29 12:13:33.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/ConnectionState.py
+-rw-rw-rw-   0        0        0     4200 2024-03-28 16:44:17.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/RawTLSRecord.py
+-rw-rw-rw-   0        0        0       65 2024-03-02 10:25:01.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/__init__.py
+-rw-rw-rw-   0        0        0     1851 2024-03-29 08:57:18.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/certificate_verifier.py
+-rw-rw-rw-   0        0        0     6240 2024-03-28 06:30:56.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/extensions.py
+-rw-rw-rw-   0        0        0    12644 2024-03-29 11:00:58.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/messages.py
+-rw-rw-rw-   0        0        0     5135 2024-03-28 05:52:47.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/records.py
+-rw-rw-rw-   0        0        0    13034 2024-03-28 11:30:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/tls_cryptography.py
+-rw-rw-rw-   0        0        0      918 2024-04-15 18:08:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/URLSearchParams.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.464097 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/
+-rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/WSMessage.py
+-rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-03-02 14:32:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WSConnection.py
+-rw-rw-rw-   0        0        0      628 2024-03-02 10:33:58.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.533115 kutil_jakubaugustyn-0.0.6/src/kutil/storage/
+-rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/Cache.py
+-rw-rw-rw-   0        0        0     6611 2024-03-01 16:41:47.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/Config.py
+-rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.680264 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/
+-rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/__init__.py
+-rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/bon.py
+-rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/converter.py
+-rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/decoder.py
+-rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/encoder.py
+-rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/shared.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.764908 kutil_jakubaugustyn-0.0.6/src/kutil/threads/
+-rw-rw-rw-   0        0        0     1721 2023-12-26 07:13:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/threads/ThreadWaiter.py
+-rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 kutil_jakubaugustyn-0.0.6/src/kutil/threads/__init__.py
+-rw-rw-rw-   0        0        0    15510 2024-03-02 11:13:45.000000 kutil_jakubaugustyn-0.0.6/src/kutil/typing_help.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.818300 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/
+-rw-rw-rw-   0        0        0    27300 2024-04-20 12:54:07.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/MapyCZServer.py
+-rw-rw-rw-   0        0        0     3167 2024-04-16 08:53:51.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/WebScraperServer.py
+-rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 kutil_jakubaugustyn-0.0.6/tests/test_bon.py
+-rw-rw-rw-   0        0        0      756 2024-03-02 10:48:38.000000 kutil_jakubaugustyn-0.0.6/tests/test_bytebuffer.py
+-rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 kutil_jakubaugustyn-0.0.6/tests/test_js.py
```

### Comparing `kutil_jakubaugustyn-0.0.5/LICENSE` & `kutil_jakubaugustyn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/PKG-INFO` & `kutil_jakubaugustyn-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.5
+Version: 0.0.6
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kutil_jakubaugustyn-0.0.5/README.md` & `kutil_jakubaugustyn-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/pyproject.toml` & `kutil_jakubaugustyn-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copied that from https://github.com/Kronuz/esprima-python/blob/master/pyproject.toml
 requires = ["setuptools>=61.0", "wheel", "setuptools_scm[toml]>=8.0"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools_scm]
 
 [project]
 name = "KUtil-jakubaugustyn"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Jakub Augustýn", email = "kubik.augustyn@post.cz" },
     { name = "Radek Augustýn", email = "raugustyn@post.cz" },
 ]
 description = "Kuba's Python Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/PKG-INFO` & `kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.5
+Version: 0.0.6
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kutil_jakubaugustyn-0.0.5/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt` & `kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/buffer/BidirectionalByteArray.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/BidirectionalByteArray.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/buffer/ByteBuffer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/ByteBuffer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/buffer/DataBuffer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/DataBuffer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/buffer/TextOutput.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/TextOutput.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/io/directory.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/io/directory.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/io/file.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/io/file.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/AST.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/AST.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/BytecodeFile.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/BytecodeFile.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Compiler.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Compiler.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Error.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Error.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Interpreter.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Interpreter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Language.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Language.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Lexer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Lexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Options.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Options.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Parser.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Parser.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Stack.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Stack.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/Token.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/Token.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/BrainFuck.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/BrainFuck.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSLexer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSLexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSOptions.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSOptions.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/JSParser.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSParser.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/Javascript.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/Javascript.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/__init__.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/character.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/character.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/error_handler.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/error_handler.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/messages.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/messages.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/nodes.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/nodes.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/javascript/syntax.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/syntax.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/Canvas.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Canvas.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/Employee.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Employee.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTCompiler.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTCompiler.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTInterpreter.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTInterpreter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTLexer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTLexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PTParser.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTParser.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/PaintTryhard.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PaintTryhard.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/__init__.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/boss.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/boss.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/language/languages/paint_tryhard/jobs/painter.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/painter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/AbstractProtocol.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/AbstractProtocol.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPHeaders.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPHeaders.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPRequest.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTP/HTTPResponse.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPResponse.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPConnection.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPSConnection.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPSConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/HTTPServer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPServer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/ProtocolConnection.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/ProtocolServer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolServer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TCPConnection.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TCPConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/AlertCause.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/AlertCause.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/CipherSuite.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/CipherSuite.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/ConnectionState.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/ConnectionState.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/RawTLSRecord.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/RawTLSRecord.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/certificate_verifier.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/certificate_verifier.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/extensions.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/extensions.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/messages.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/messages.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/records.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/records.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/TLS/tls_cryptography.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/tls_cryptography.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/URLSearchParams.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WS/WSMessage.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/WSMessage.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/WSConnection.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WSConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/protocol/__init__.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/Config.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/Config.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/bon.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/bon.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/converter.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/converter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/decoder.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/decoder.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/encoder.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/encoder.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/storage/bon/shared.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/shared.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/threads/ThreadWaiter.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/threads/ThreadWaiter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/typing_help.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/typing_help.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/MapyCZServer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/MapyCZServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,29 @@
     ZAKLADNI = "basic"
     TURISTICKA = "outdoor"
     LETECKA = "aerial"
     POPISKY_A_HRANICE = "names-overlay"
     ZIMNI = "winter"
 
 
+imageTypes: Final[dict[MapSet, str]] = {
+    MapSet.ZAKLADNI: "png",
+    MapSet.TURISTICKA: "png",
+    MapSet.LETECKA: "jpg",
+    MapSet.POPISKY_A_HRANICE: "png",
+    MapSet.ZIMNI: "png"
+}
+
+
 class MapyCZServer(WebScraperServer):
     usageHTMLTemplate: Optional[bytes] = None
     usageQGIS: Optional[bytes] = None
     cacheControl: Final[str] = "max-age=3600, public"
+    languages: Final[set[str]] = {"cs", "de", "el", "en", "es", "fr", "it", "nl", "pl", "pt",
+                                  "ru", "sk", "tr", "uk"}
 
     __scrapeAroundArgs: list[tuple]
     __cachedAPIKey: Optional[str]
     # Path to a cache directory, should be shared between users and not contain any sensitive data
     __cachePath: Optional[str]
     # Maximum size in images count stored
     __maxCacheSize: Optional[int]
@@ -143,61 +154,86 @@
                 body = HTTPResponse.enc(f'<h1>Too many requests.</h1>'
                                         f'Currently actively handling {len(self.__workingConnections)} '
                                         f'out of {len(self.server.connections)} requests.')
                 return HTTPResponse(429, "Too many requests", headers, body)
 
         if req.requestURI.startswith("/tile/"):
             mapSetStr = uriWithoutQuery[6:]
-            try:
-                mapSet = MapSet(mapSetStr)
-            except (KeyError, TypeError, ValueError):
-                resp = WebScraperServer.badRequest()
-                resp.body = HTTPResponse.enc(
-                    f'<h1>Bad request - unknown layer kind: {mapSetStr}</h1>'
-                    f'<a href="https://developer.mapy.cz/rest-api/funkce/mapove-dlazdice/">'
-                    f'Visit this page for more info</a><br>'
-                    f'Possible kinds:<br>{"<br>".join(map(lambda item: f"{item.name}: <b>{item.value}</b>", MapSet))}')
-                print(f"Bad request: unknown layer kind while requesting {req.requestURI}")
-                return resp
+            mapSet = self.__parseMapSet(mapSetStr, req.requestURI)
+            if isinstance(mapSet, HTTPResponse):
+                return mapSet
             try:
                 x = int(params["x"])
                 y = int(params["y"])
                 zoom = int(params["z"])
                 tileSize = params.get("tileSize", "256")
                 lang = params.get("lang", "cs")
                 # https://api.mapy.cz/v1/docs/maptiles/#/tiles/get_v1_maptiles__mapset___tileSize___z___x___y_
                 assert tileSize in ("256", "256@2x"), "Invalid tile size"
                 if tileSize == "256@2x":
                     assert mapSet in (MapSet.ZAKLADNI, MapSet.TURISTICKA, MapSet.ZIMNI), \
                         "Invalid tile size - used 256@2x in other mapSet than ZAKLADNI, TURISTICKA, ZIMNI"
-                assert lang in ("cs", "de", "el", "en", "es", "fr", "it", "nl", "pl", "pt",
-                                "ru", "sk", "tr", "uk"), "Invalid language"
+                assert lang in MapyCZServer.languages, "Invalid language"
             except (ValueError, KeyError, AssertionError) as e:
                 resp = WebScraperServer.badRequest()
                 resp.body = (b'<h1>Bad request - bad params</h1>'
-                             b'Required params: x, y, z (zoom), tileSize ("256" or "256@2x", by default "256"), lang '
-                             b'(language - one of: cs - default, de, el, en, es, fr, it, nl, pl, pt, ru, sk, tr, uk)' +
-                             HTTPResponse.enc("<br>Caused by error: " + str(e)))
+                             b'Required params: x, y, z (zoom), tileSize ("256" or "256@2x", '
+                             b'by default "256"), lang ' +
+                             HTTPResponse.enc(f"(language (default: cs) - one "
+                                              f"of: {', '.join(MapyCZServer.languages)})"
+                                              f"<br>Caused by error: {str(e)}"))
                 print(f"Bad request: bad params while requesting {req.requestURI}")
                 return resp
             # Scrape for the image
             try:
                 self.pushWorkingConnection(conn)
                 image: bytes = self.__scrape(x, y, zoom, tileSize, mapSet, lang)
             except Exception as e:
                 print("Unexpected error:", e)
                 return WebScraperServer.internalError()
             finally:
                 self.popWorkingConnection(conn)
             # Form a response
             headers: HTTPHeaders = HTTPHeaders()
-            headers["Content-Type"] = "image/png"
+            headers["Content-Type"] = f"image/{imageTypes[mapSet]}"
             headers["Cache-Control"] = MapyCZServer.cacheControl
             resp: HTTPResponse = HTTPResponse(200, "OK", headers, image)
             return resp
+        elif uriWithoutQuery == "/tiles.json":
+            try:
+                mapSetStr = params["mapSet"]
+                lang = params.get("lang", "cs")
+                assert lang in MapyCZServer.languages, "Invalid language"
+            except KeyError as e:
+                resp = WebScraperServer.badRequest()
+                resp.body = HTTPResponse.enc(
+                    f'<h1>Bad request - bad params</h1>'
+                    f'Required params: mapSet, lang (language (default: cs) - one of: '
+                    f'{", ".join(MapyCZServer.languages)})<br>Caused by error: {str(e)}'
+                )
+                print(f"Bad request: bad params while requesting {req.requestURI}")
+                return resp
+            mapSet = self.__parseMapSet(mapSetStr, req.requestURI)
+            if isinstance(mapSet, HTTPResponse):
+                return mapSet
+            # Scrape for the tiles.json file
+            try:
+                self.pushWorkingConnection(conn)
+                tilesJson: bytes = self.__scrapeTilesJson(mapSet, lang)
+            except Exception as e:
+                print("Unexpected error:", e)
+                return WebScraperServer.internalError()
+            finally:
+                self.popWorkingConnection(conn)
+            # Form a response
+            headers: HTTPHeaders = HTTPHeaders()
+            headers["Content-Type"] = "application/json"
+            headers["Cache-Control"] = MapyCZServer.cacheControl
+            resp: HTTPResponse = HTTPResponse(200, "OK", headers, tilesJson)
+            return resp
         elif req.requestURI == "/api_key.txt":
             self.pushWorkingConnection(conn)
             headers: HTTPHeaders = HTTPHeaders()
             headers["Content-Type"] = "text/plain"
             resp: HTTPResponse = HTTPResponse(200, "OK", headers,
                                               HTTPResponse.enc(self.__obtainAPIKey()))
             self.popWorkingConnection(conn)
@@ -227,14 +263,28 @@
         elif req.requestURI == "/qgis.png":
             return self.__getQgis()
         else:
             # If a bad endpoint is requested, show the usage page
             return self.__getUsage()
         return self.__performRequest(uri, conn)
 
+    def __parseMapSet(self, mapSetName: str, requestURI: str) -> MapSet | HTTPResponse:
+        try:
+            mapSet = MapSet(mapSetName)
+            return mapSet
+        except (KeyError, TypeError, ValueError):
+            resp = WebScraperServer.badRequest()
+            resp.body = HTTPResponse.enc(
+                f'<h1>Bad request - unknown layer kind: {mapSetName}</h1>'
+                f'<a href="https://developer.mapy.cz/rest-api/funkce/mapove-dlazdice/">'
+                f'Visit this page for more info</a><br>'
+                f'Possible kinds:<br>{"<br>".join(map(lambda item: f"{item.name}: <b>{item.value}</b>", MapSet))}')
+            print(f"Bad request: unknown layer kind while requesting {requestURI}")
+            return resp
+
     def __getUsage(self) -> HTTPResponse:
         html: bytes = MapyCZServer.__getUsageHTMLTemplate()
         html = html.replace(b'${HOST}', HTTPResponse.enc(self.host))
         html = html.replace(b'${PORT}', HTTPResponse.enc(str(self.port)))
         headers: HTTPHeaders = HTTPHeaders()
         headers["Content-Type"] = "text/html"
         resp: HTTPResponse = HTTPResponse(200, "OK", headers, html)
@@ -264,22 +314,32 @@
             return self.__cachedAPIKey
         r = self.getSession().get("https://api.mapy.cz/virtual-key.js")
         assert r.status_code == 200, f"Bad status code ({r.status_code}) - __scrape failed - API key obtaining"
         self.__cachedAPIKey = re.match('Loader\\.apiKey = "(\\S+)"', r.text).group(1)
         return self.__cachedAPIKey
 
     def __authorizedGetRequest(self, uri: str, force200: bool = True) -> requests.Response:
+        if "API" not in uri:
+            raise ValueError("Invalid authorized request URI - no authorization present")
         r = self.getSession().get(uri.replace("API", self.__obtainAPIKey()))
         # print(r.url)
         if r.status_code != 200:
+            if r.status_code == 401:
+                print("Scrape failed - invalid API key (re-obtaining)")
             r = self.getSession().get(uri.replace("API", self.__obtainAPIKey(True)))
         if force200:
-            assert r.status_code == 200, f"Bad status code ({r.status_code}) - scrape failed - response obtaining"
+            assert r.status_code == 200, \
+                f"Bad status code ({r.status_code}) - scrape failed - response obtaining"
         return r
 
+    def __scrapeTilesJson(self, mapSet: MapSet, lang: str) -> bytes:
+        uri: str = f"https://api.mapy.cz/v1/maptiles/{mapSet.value}/tiles.json?apikey=API&lang={lang}"
+        r = self.__authorizedGetRequest(uri)
+        return r.content
+
     def __scrape(self, x: int, y: int, zoom: int, tileSize: str, mapSet: MapSet, lang: str,
                  canScrapeAround: bool = True) -> bytes:
         # print(f'X: {x}, Y: {y}, Zoom: {zoom}, tile size: {tileSize}, kind: {mapSet.name}, language: {lang}')
         cachedValue: bytes | None = self.__obtainFromCache(x, y, zoom, tileSize, mapSet, lang)
         if cachedValue is not None:
             return cachedValue
         # https://api.mapy.cz/v1/maptiles/outdoor/tiles.json?apikey=virtual-
@@ -410,16 +470,16 @@
                 continue
             toLeaveCount = int(self.__maxCacheSize * .9)
             files: dict[str, float] = {}  # File name: file last edited
             for dirEntry in os.scandir(self.__cachePath):
                 if dirEntry.is_dir():
                     continue
                 ext = getFileExtension(dirEntry.name)
-                if ext != ".png":
-                    # Do not delete non-png files
+                if ext != ".png" and ext != ".jpg":
+                    # Do not delete non-png and non-jpg files
                     continue
                 try:
                     theTime = dirEntry.stat().st_birthtime
                 except AttributeError:
                     theTime = dirEntry.stat().st_mtime
                 files[dirEntry.name] = theTime
             fileNames: list[str] = list(files.keys())
@@ -434,16 +494,16 @@
                 if not os.path.exists(path):
                     continue
                 os.remove(path)
 
     def __getCacheKey(self, x: int, y: int, zoom: int, tileSize: str, mapSet: MapSet,
                       lang: str) -> str:
         if zoom <= 6:
-            return f"{x}_{y}_{zoom}_{tileSize}_{mapSet.value}_{lang}.png"
-        return f"{x}_{y}_{zoom}_{tileSize}_{mapSet.value}.png"
+            return f"{x}_{y}_{zoom}_{tileSize}_{mapSet.value}_{lang}.{imageTypes[mapSet]}"
+        return f"{x}_{y}_{zoom}_{tileSize}_{mapSet.value}.{imageTypes[mapSet]}"
 
     def __getCacheFilePath(self, x: int, y: int, zoom: int, tileSize: str, mapSet: MapSet,
                            lang: str) -> str:
         return os.path.join(self.__cachePath,
                             self.__getCacheKey(x, y, zoom, tileSize, mapSet, lang))
 
     @staticmethod
```

### Comparing `kutil_jakubaugustyn-0.0.5/src/kutil/webscraper/WebScraperServer.py` & `kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/WebScraperServer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/tests/test_bon.py` & `kutil_jakubaugustyn-0.0.6/tests/test_bon.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/tests/test_bytebuffer.py` & `kutil_jakubaugustyn-0.0.6/tests/test_bytebuffer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.5/tests/test_js.py` & `kutil_jakubaugustyn-0.0.6/tests/test_js.py`

 * *Files identical despite different names*

