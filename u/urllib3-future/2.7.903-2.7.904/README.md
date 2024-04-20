# Comparing `tmp/urllib3_future-2.7.903.tar.gz` & `tmp/urllib3_future-2.7.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr  4 07:01:03 2024, max compression
+gzip compressed data, last modified: Sat Apr 20 06:19:56 2024, max compression
```

## Comparing `urllib3_future-2.7.903.tar` & `urllib3_future-2.7.904.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0    86135 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/CHANGES.rst
--rw-r--r--   0        0        0      490 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/Makefile
--rw-r--r--   0        0        0    54247 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/advanced-usage.rst
--rw-r--r--   0        0        0     4297 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/async.rst
--rw-r--r--   0        0        0       59 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/changelog.rst
--rw-r--r--   0        0        0     5787 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/conf.py
--rw-r--r--   0        0        0     6749 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/contributing.rst
--rw-r--r--   0        0        0     1939 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/index.rst
--rw-r--r--   0        0        0     4513 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/make.bat
--rw-r--r--   0        0        0       92 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/requirements.txt
--rw-r--r--   0        0        0    16926 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/user-guide.rst
--rw-r--r--   0        0        0    15195 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0   307934 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/_static/logo.png
--rw-r--r--   0        0        0     7872 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/images/logo.png
--rw-r--r--   0        0        0      516 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/images/logo.svg
--rw-r--r--   0        0        0      245 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/index.rst
--rw-r--r--   0        0        0      457 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.backend.rst
--rw-r--r--   0        0        0      349 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      712 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      559 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      905 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      385 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      206 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      231 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/contrib/resolver.rst
--rw-r--r--   0        0        0      124 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0      142 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/docs/reference/contrib/ssa.rst
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/__init__.py
--rw-r--r--   0        0        0    13408 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     4582 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9813 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/server.py
--rw-r--r--   0        0        0    11213 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/dummyserver/certs/server.key
--rw-r--r--   0        0        0     6090 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/__init__.py
--rw-r--r--   0        0        0    15956 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_collections.py
--rw-r--r--   0        0        0     8092 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_constant.py
--rw-r--r--   0        0        0    21727 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_typing.py
--rw-r--r--   0        0        0      100 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_version.py
--rw-r--r--   0        0        0    38148 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/connection.py
--rw-r--r--   0        0        0    75605 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/exceptions.py
--rw-r--r--   0        0        0     9151 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/fields.py
--rw-r--r--   0        0        0     2202 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/filepost.py
--rw-r--r--   0        0        0    36048 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/py.typed
--rw-r--r--   0        0        0    35459 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/_async/response.py
--rw-r--r--   0        0        0      390 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/__init__.py
--rw-r--r--   0        0        0    16031 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/_base.py
--rw-r--r--   0        0        0    44426 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/hface.py
--rw-r--r--   0        0        0      225 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/_async/__init__.py
--rw-r--r--   0        0        0     6002 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/_async/_base.py
--rw-r--r--   0        0        0    42550 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0     1109 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1207 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      801 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/py.typed
--rw-r--r--   0        0        0     1085 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1003 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4327 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0     9935 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10446 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      704 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     8840 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      709 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    19359 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1145 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/request.py
--rw-r--r--   0        0        0     1329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/response.py
--rw-r--r--   0        0        0    19245 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    24783 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    21933 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/traffic_police.py
--rw-r--r--   0        0        0    15270 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/wait.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/_async/ssl_.py
--rw-r--r--   0        0        0    22050 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3/util/_async/traffic_police.py
--rw-r--r--   0        0        0     6090 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/__init__.py
--rw-r--r--   0        0        0    15956 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_collections.py
--rw-r--r--   0        0        0     8092 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_constant.py
--rw-r--r--   0        0        0    21727 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_typing.py
--rw-r--r--   0        0        0      100 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_version.py
--rw-r--r--   0        0        0    38148 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/connection.py
--rw-r--r--   0        0        0    75605 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/exceptions.py
--rw-r--r--   0        0        0     9151 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/fields.py
--rw-r--r--   0        0        0     2202 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/filepost.py
--rw-r--r--   0        0        0    36048 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/poolmanager.py
--rw-r--r--   0        0        0       93 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/py.typed
--rw-r--r--   0        0        0    35459 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/response.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/_async/response.py
--rw-r--r--   0        0        0      390 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/__init__.py
--rw-r--r--   0        0        0    16031 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/_base.py
--rw-r--r--   0        0        0    44426 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/hface.py
--rw-r--r--   0        0        0      225 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/_async/__init__.py
--rw-r--r--   0        0        0     6002 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/_async/_base.py
--rw-r--r--   0        0        0    42550 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/socks.py
--rw-r--r--   0        0        0     1109 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1207 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      801 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/py.typed
--rw-r--r--   0        0        0     1085 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1003 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4327 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0     9935 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10446 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      704 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     8840 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      709 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    19359 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/connection.py
--rw-r--r--   0        0        0     1145 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/request.py
--rw-r--r--   0        0        0     1329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/response.py
--rw-r--r--   0        0        0    19245 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/retry.py
--rw-r--r--   0        0        0    24783 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/timeout.py
--rw-r--r--   0        0        0    21933 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/traffic_police.py
--rw-r--r--   0        0        0    15270 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/url.py
--rw-r--r--   0        0        0     1146 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/util.py
--rw-r--r--   0        0        0     4423 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/wait.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/_async/ssl_.py
--rw-r--r--   0        0        0    22050 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/src/urllib3_future/util/_async/traffic_police.py
--rw-r--r--   0        0        0     9646 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/__init__.py
--rw-r--r--   0        0        0    11926 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/conftest.py
--rw-r--r--   0        0        0     6222 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/port_helpers.py
--rw-r--r--   0        0        0    12638 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_collections.py
--rw-r--r--   0        0        0      692 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_compatibility.py
--rw-r--r--   0        0        0    10288 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_connection.py
--rw-r--r--   0        0        0    22649 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_connectionpool.py
--rw-r--r--   0        0        0     1531 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_exceptions.py
--rw-r--r--   0        0        0     3882 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_fields.py
--rw-r--r--   0        0        0     3778 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_filepost.py
--rw-r--r--   0        0        0      978 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_no_ssl.py
--rw-r--r--   0        0        0    17951 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_proxymanager.py
--rw-r--r--   0        0        0    38863 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_response.py
--rw-r--r--   0        0        0    16640 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_retry.py
--rw-r--r--   0        0        0     6554 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_ssl.py
--rw-r--r--   0        0        0    16917 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_ssltransport.py
--rw-r--r--   0        0        0    43037 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_util.py
--rw-r--r--   0        0        0     5999 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/test_wait.py
--rw-r--r--   0        0        0     1187 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/tz_stub.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0    21281 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/test_resolver.py
--rw-r--r--   0        0        0    25922 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/asynchronous/__init__.py
--rw-r--r--   0        0        0    21291 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/asynchronous/test_resolver.py
--rw-r--r--   0        0        0    21728 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/asynchronous/test_socks.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/hface/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/contrib/hface/test_stream_matrix.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0     9840 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3702 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56059 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0     7756 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_happy_eyeballs.py
--rw-r--r--   0        0        0    43193 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    23853 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    32501 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    88179 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/asynchronous/__init__.py
--rw-r--r--   0        0        0    59408 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_connectionpool.py
--rw-r--r--   0        0        0     7329 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
--rw-r--r--   0        0        0    19562 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_poolmanager.py
--rw-r--r--   0        0        0     2837 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_conn_info.py
--rw-r--r--   0        0        0     3764 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_connection.py
--rw-r--r--   0        0        0     2821 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_connection_multiplexed.py
--rw-r--r--   0        0        0     5912 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     1924 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_protolevel.py
--rw-r--r--   0        0        0     3209 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_proxy.py
--rw-r--r--   0        0        0     5658 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_send_data.py
--rw-r--r--   0        0        0     1864 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_stream.py
--rw-r--r--   0        0        0     6683 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/test_svn.py
--rw-r--r--   0        0        0        0 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/__init__.py
--rw-r--r--   0        0        0     2217 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_conn_info.py
--rw-r--r--   0        0        0     4035 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connection.py
--rw-r--r--   0        0        0     3122 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connection_multiplexed.py
--rw-r--r--   0        0        0     6143 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     2003 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_protolevel.py
--rw-r--r--   0        0        0     3274 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_proxy.py
--rw-r--r--   0        0        0     5880 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_send_data.py
--rw-r--r--   0        0        0     1967 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_stream.py
--rw-r--r--   0        0        0     7217 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/test/with_traefik/asynchronous/test_svn.py
--rw-r--r--   0        0        0       85 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/.gitignore
--rw-r--r--   0        0        0     1093 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/LICENSE.txt
--rw-r--r--   0        0        0     4277 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/README.md
--rw-r--r--   0        0        0     1342 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/hatch_build.py
--rw-r--r--   0        0        0     5366 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/pyproject.toml
--rw-r--r--   0        0        0     6784 2024-04-04 07:01:03.000000 urllib3_future-2.7.903/PKG-INFO
+-rw-r--r--   0        0        0    86335 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/CHANGES.rst
+-rw-r--r--   0        0        0      490 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/Makefile
+-rw-r--r--   0        0        0    54247 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/advanced-usage.rst
+-rw-r--r--   0        0        0     4297 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/async.rst
+-rw-r--r--   0        0        0       59 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/changelog.rst
+-rw-r--r--   0        0        0     5787 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/conf.py
+-rw-r--r--   0        0        0     6749 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/contributing.rst
+-rw-r--r--   0        0        0     1939 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/index.rst
+-rw-r--r--   0        0        0     4513 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/make.bat
+-rw-r--r--   0        0        0       92 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/requirements.txt
+-rw-r--r--   0        0        0    17426 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/user-guide.rst
+-rw-r--r--   0        0        0    15195 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0   307934 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/_static/logo.png
+-rw-r--r--   0        0        0     7872 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/images/logo.svg
+-rw-r--r--   0        0        0      245 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/index.rst
+-rw-r--r--   0        0        0      457 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.backend.rst
+-rw-r--r--   0        0        0      349 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      712 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      559 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      905 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      385 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      206 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      231 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/contrib/resolver.rst
+-rw-r--r--   0        0        0      124 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0      142 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/docs/reference/contrib/ssa.rst
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13408 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     4582 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9813 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/server.py
+-rw-r--r--   0        0        0    11213 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     6090 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/__init__.py
+-rw-r--r--   0        0        0    15956 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     8092 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_constant.py
+-rw-r--r--   0        0        0    21727 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_typing.py
+-rw-r--r--   0        0        0      100 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_version.py
+-rw-r--r--   0        0        0    38148 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/connection.py
+-rw-r--r--   0        0        0    75605 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2202 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    36048 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/py.typed
+-rw-r--r--   0        0        0    35459 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_async/connection.py
+-rw-r--r--   0        0        0    77458 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/_async/response.py
+-rw-r--r--   0        0        0      390 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/__init__.py
+-rw-r--r--   0        0        0    16031 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/_base.py
+-rw-r--r--   0        0        0    44491 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/_async/__init__.py
+-rw-r--r--   0        0        0     6002 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/_async/_base.py
+-rw-r--r--   0        0        0    42615 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0     1109 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1699 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      801 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1085 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4421 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4327 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0     9935 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10446 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      704 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     8840 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      709 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    17220 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     1329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    19245 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    24783 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    21933 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/traffic_police.py
+-rw-r--r--   0        0        0    15270 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22050 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     6090 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/__init__.py
+-rw-r--r--   0        0        0    15956 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_collections.py
+-rw-r--r--   0        0        0     8092 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_constant.py
+-rw-r--r--   0        0        0    21727 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_typing.py
+-rw-r--r--   0        0        0      100 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_version.py
+-rw-r--r--   0        0        0    38148 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/connection.py
+-rw-r--r--   0        0        0    75605 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/fields.py
+-rw-r--r--   0        0        0     2202 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/filepost.py
+-rw-r--r--   0        0        0    36048 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/py.typed
+-rw-r--r--   0        0        0    35459 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/response.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_async/connection.py
+-rw-r--r--   0        0        0    77458 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/_async/response.py
+-rw-r--r--   0        0        0      390 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/__init__.py
+-rw-r--r--   0        0        0    16031 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/_base.py
+-rw-r--r--   0        0        0    44491 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/_async/__init__.py
+-rw-r--r--   0        0        0     6002 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/_async/_base.py
+-rw-r--r--   0        0        0    42615 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/socks.py
+-rw-r--r--   0        0        0     1109 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1699 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      801 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1085 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4421 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4327 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0     9935 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10446 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      704 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     8840 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      709 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    17220 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/request.py
+-rw-r--r--   0        0        0     1329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/response.py
+-rw-r--r--   0        0        0    19245 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/retry.py
+-rw-r--r--   0        0        0    24783 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/timeout.py
+-rw-r--r--   0        0        0    21933 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/traffic_police.py
+-rw-r--r--   0        0        0    15270 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/url.py
+-rw-r--r--   0        0        0     1146 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/util.py
+-rw-r--r--   0        0        0     4423 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/wait.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22050 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/src/urllib3_future/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     9646 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/__init__.py
+-rw-r--r--   0        0        0    11926 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/conftest.py
+-rw-r--r--   0        0        0     6222 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/port_helpers.py
+-rw-r--r--   0        0        0    12638 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_collections.py
+-rw-r--r--   0        0        0      692 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_compatibility.py
+-rw-r--r--   0        0        0    10288 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_connection.py
+-rw-r--r--   0        0        0    22649 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_connectionpool.py
+-rw-r--r--   0        0        0     1531 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_exceptions.py
+-rw-r--r--   0        0        0     3882 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_fields.py
+-rw-r--r--   0        0        0     3778 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17951 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_proxymanager.py
+-rw-r--r--   0        0        0    38863 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_response.py
+-rw-r--r--   0        0        0    16640 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_retry.py
+-rw-r--r--   0        0        0     6554 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_ssl.py
+-rw-r--r--   0        0        0    16917 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43037 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_util.py
+-rw-r--r--   0        0        0     5999 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/test_wait.py
+-rw-r--r--   0        0        0     1187 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0    21281 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/test_resolver.py
+-rw-r--r--   0        0        0    25922 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/asynchronous/__init__.py
+-rw-r--r--   0        0        0    21291 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/asynchronous/test_resolver.py
+-rw-r--r--   0        0        0    21728 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/asynchronous/test_socks.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/contrib/hface/test_stream_matrix.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0     9840 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3702 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56059 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0     7756 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    43193 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    23853 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    32501 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    88179 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/asynchronous/__init__.py
+-rw-r--r--   0        0        0    59408 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_connectionpool.py
+-rw-r--r--   0        0        0     7329 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    19562 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_poolmanager.py
+-rw-r--r--   0        0        0     2837 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/__init__.py
+-rw-r--r--   0        0        0     3069 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_conn_info.py
+-rw-r--r--   0        0        0     3764 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_connection.py
+-rw-r--r--   0        0        0     2821 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     5912 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     1924 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_protolevel.py
+-rw-r--r--   0        0        0     3209 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_proxy.py
+-rw-r--r--   0        0        0     5658 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_send_data.py
+-rw-r--r--   0        0        0     1864 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_stream.py
+-rw-r--r--   0        0        0     6683 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/test_svn.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2217 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_conn_info.py
+-rw-r--r--   0        0        0     4035 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connection.py
+-rw-r--r--   0        0        0     3122 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     6143 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     2003 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_protolevel.py
+-rw-r--r--   0        0        0     3274 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_proxy.py
+-rw-r--r--   0        0        0     5880 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_send_data.py
+-rw-r--r--   0        0        0     1967 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_stream.py
+-rw-r--r--   0        0        0     7217 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/test/with_traefik/asynchronous/test_svn.py
+-rw-r--r--   0        0        0       85 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/.gitignore
+-rw-r--r--   0        0        0     1093 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/LICENSE.txt
+-rw-r--r--   0        0        0     4277 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/README.md
+-rw-r--r--   0        0        0     1342 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/hatch_build.py
+-rw-r--r--   0        0        0     5594 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/pyproject.toml
+-rw-r--r--   0        0        0     7012 2024-04-20 06:19:56.000000 urllib3_future-2.7.904/PKG-INFO
```

### Comparing `urllib3_future-2.7.903/CHANGES.rst` & `urllib3_future-2.7.904/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.7.904 (2024-04-20)
+====================
+
+- Added support for qh3 version v1
+- **Security:** Fixed ignored DNS matching with its certificate in certain conditions while negotiating HTTP/3 over QUIC
+
 2.7.903 (2024-04-04)
 ====================
 
 - Removed warning about "unresponsive" pool of connection due to how it can confuse users.
 
 2.7.902 (2024-04-03)
 ====================
```

### Comparing `urllib3_future-2.7.903/docs/Makefile` & `urllib3_future-2.7.904/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/advanced-usage.rst` & `urllib3_future-2.7.904/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/async.rst` & `urllib3_future-2.7.904/docs/async.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/conf.py` & `urllib3_future-2.7.904/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/contributing.rst` & `urllib3_future-2.7.904/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/index.rst` & `urllib3_future-2.7.904/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/make.bat` & `urllib3_future-2.7.904/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/user-guide.rst` & `urllib3_future-2.7.904/docs/user-guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 .. code-block:: bash
 
   $ python -m pip install qh3
 
 This may require some external toolchain to be available (compilation).
 
+.. note:: HTTP/3 is automatically installed and ready-to-use if you fulfill theses requirements: Linux, Windows or MacOS using Python (or PyPy) 3.7 onward with one of the supported architecture (arm64/aarch64/s390x/x86_64/amd64/ppc64/ppc64le).
+
+.. caution:: If the requirements aren't fulfilled for HTTP/3, your package manager won't pick qh3 for installation when installing urllib3-future and it will be silently disabled. We choose not to impose compilation and keep a safe pure Python fallback.
+
 Making Requests
 ---------------
 
 First things first, import the urllib3 module:
 
 .. code-block:: python
```

### Comparing `urllib3_future-2.7.903/docs/v2-migration-guide.rst` & `urllib3_future-2.7.904/docs/v2-migration-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/_static/banner.svg` & `urllib3_future-2.7.904/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/_static/banner_github.svg` & `urllib3_future-2.7.904/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/_static/dark-logo.svg` & `urllib3_future-2.7.904/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/_static/logo.png` & `urllib3_future-2.7.904/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/images/demo-button.png` & `urllib3_future-2.7.904/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/images/favicon.png` & `urllib3_future-2.7.904/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/images/learn-more-button.png` & `urllib3_future-2.7.904/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/images/logo.png` & `urllib3_future-2.7.904/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/images/logo.svg` & `urllib3_future-2.7.904/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/reference/urllib3.connectionpool.rst` & `urllib3_future-2.7.904/docs/reference/urllib3.connectionpool.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/reference/urllib3.poolmanager.rst` & `urllib3_future-2.7.904/docs/reference/urllib3.poolmanager.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/docs/reference/urllib3.response.rst` & `urllib3_future-2.7.904/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/handlers.py` & `urllib3_future-2.7.904/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/https_proxy.py` & `urllib3_future-2.7.904/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/proxy.py` & `urllib3_future-2.7.904/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/server.py` & `urllib3_future-2.7.904/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/testcase.py` & `urllib3_future-2.7.904/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/certs/cacert.key` & `urllib3_future-2.7.904/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/certs/cacert.pem` & `urllib3_future-2.7.904/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/certs/server.crt` & `urllib3_future-2.7.904/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/dummyserver/certs/server.key` & `urllib3_future-2.7.904/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/__init__.py` & `urllib3_future-2.7.904/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_collections.py` & `urllib3_future-2.7.904/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_constant.py` & `urllib3_future-2.7.904/src/urllib3/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_request_methods.py` & `urllib3_future-2.7.904/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_typing.py` & `urllib3_future-2.7.904/src/urllib3/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/connection.py` & `urllib3_future-2.7.904/src/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/connectionpool.py` & `urllib3_future-2.7.904/src/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/exceptions.py` & `urllib3_future-2.7.904/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/fields.py` & `urllib3_future-2.7.904/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/filepost.py` & `urllib3_future-2.7.904/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/poolmanager.py` & `urllib3_future-2.7.904/src/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/response.py` & `urllib3_future-2.7.904/src/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_async/connection.py` & `urllib3_future-2.7.904/src/urllib3/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_async/connectionpool.py` & `urllib3_future-2.7.904/src/urllib3/_async/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_async/poolmanager.py` & `urllib3_future-2.7.904/src/urllib3/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/_async/response.py` & `urllib3_future-2.7.904/src/urllib3/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/backend/_base.py` & `urllib3_future-2.7.904/src/urllib3/backend/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/backend/hface.py` & `urllib3_future-2.7.904/src/urllib3/backend/hface.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,17 @@
             # mTLS start
             certfile=cert_file,
             keyfile=key_file,
             keypassword=key_password,
             # mTLS end
             cert_fingerprint=cert_fingerprint,
             cert_use_common_name=cert_use_common_name,
-            verify_hostname=bool(assert_hostname),
+            verify_hostname=assert_hostname
+            if isinstance(assert_hostname, bool)
+            else True,
             assert_hostname=assert_hostname
             if isinstance(assert_hostname, str)
             else None,
         )
 
         self.is_verified = not self.__custom_tls_settings.insecure
```

### Comparing `urllib3_future-2.7.903/src/urllib3/backend/_async/_base.py` & `urllib3_future-2.7.904/src/urllib3/backend/_async/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/backend/_async/hface.py` & `urllib3_future-2.7.904/src/urllib3/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,17 @@
             # mTLS start
             certfile=cert_file,
             keyfile=key_file,
             keypassword=key_password,
             # mTLS end
             cert_fingerprint=cert_fingerprint,
             cert_use_common_name=cert_use_common_name,
-            verify_hostname=bool(assert_hostname),
+            verify_hostname=assert_hostname
+            if isinstance(assert_hostname, bool)
+            else True,
             assert_hostname=assert_hostname
             if isinstance(assert_hostname, str)
             else None,
         )
 
         self.is_verified = not self.__custom_tls_settings.insecure
```

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/_socks_override.py` & `urllib3_future-2.7.904/src/urllib3/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/pyopenssl.py` & `urllib3_future-2.7.904/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/socks.py` & `urllib3_future-2.7.904/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/_configuration.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/_error_codes.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/_typing.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/events/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/events/_events.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.904/src/urllib3/contrib/hface/protocols/http3/_qh3.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,32 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import datetime
 import ssl
 import typing
 from collections import deque
 from os import environ
 from time import time as monotonic
 from typing import Any, Iterable, Sequence
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Literal
 
-import qh3.h3.events as h3_events
-import qh3.quic.events as quic_events
-from qh3.h3.connection import H3Connection, ProtocolError
-from qh3.h3.exceptions import H3Error
-from qh3.quic.configuration import QuicConfiguration
-from qh3.quic.connection import QuicConnection, QuicConnectionError
-from qh3.quic.logger import QuicFileLogger
-from qh3.tls import CipherSuite, SessionTicket
+from qh3 import (
+    CipherSuite,
+    H3Connection,
+    H3Error,
+    ProtocolError,
+    QuicConfiguration,
+    QuicConnection,
+    QuicConnectionError,
+    QuicFileLogger,
+    SessionTicket,
+    h3_events,
+    quic_events,
+)
 
 from ..._configuration import QuicTLSConfig
 from ..._stream_matrix import StreamMatrix
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
 from ...events import HeadersReceived, StreamResetReceived
@@ -63,15 +69,15 @@
             cadata=tls_config.cadata,
             alpn_protocols=["h3"],
             session_ticket=tls_config.session_ticket,
             server_name=server_name,
             hostname_checks_common_name=tls_config.cert_use_common_name,
             assert_fingerprint=tls_config.cert_fingerprint,
             verify_hostname=tls_config.verify_hostname,
-            secrets_log_file=open(keylogfile_path, "w+") if keylogfile_path else None,  # type: ignore[arg-type]
+            secrets_log_file=open(keylogfile_path, "w") if keylogfile_path else None,  # type: ignore[arg-type]
             quic_logger=QuicFileLogger(qlogdir_path) if qlogdir_path else None,
             idle_timeout=300.0,
         )
 
         if tls_config.ciphers:
             available_ciphers = {c.name: c for c in CipherSuite}
             chosen_ciphers: list[CipherSuite] = []
@@ -268,39 +274,32 @@
             raise ValueError("TLS handshake has not been done yet")
 
         if not self._quic.get_issuercerts():
             return None
 
         x509_certificate = self._quic.get_issuercerts()[0]
 
-        try:
-            from cryptography.hazmat.primitives._serialization import Encoding
-        except ImportError as e:
-            raise ValueError(
-                "Unable to generate a dict-form representation due to missing dependencies or sub-module"
-            ) from e
-
         if binary_form:
-            return x509_certificate.public_bytes(Encoding.DER)
+            return x509_certificate.public_bytes()
+
+        datetime.datetime.fromtimestamp(
+            x509_certificate.not_valid_before, tz=datetime.timezone.utc
+        )
 
         issuer_info = {
-            "version": x509_certificate.version.value + 1,
-            "serialNumber": ("%x" % x509_certificate.serial_number).upper(),
+            "version": x509_certificate.version + 1,
+            "serialNumber": x509_certificate.serial_number.upper(),
             "subject": [],
             "issuer": [],
-            "notBefore": (
-                x509_certificate.not_valid_before
-                if not hasattr(x509_certificate, "not_valid_before_utc")
-                else x509_certificate.not_valid_before_utc
+            "notBefore": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_before, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
-            "notAfter": (
-                x509_certificate.not_valid_after
-                if not hasattr(x509_certificate, "not_valid_after_utc")
-                else x509_certificate.not_valid_after_utc
+            "notAfter": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_after, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
         }
 
         _short_name_assoc = {
             "CN": "commonName",
             "L": "localityName",
@@ -308,40 +307,30 @@
             "O": "organizationName",
             "OU": "organizationalUnitName",
             "C": "countryName",
             "STREET": "streetAddress",
             "DC": "domainComponent",
         }
 
-        for item in x509_certificate.subject:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.subject:
             issuer_info["subject"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for item in x509_certificate.issuer:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.issuer:
             issuer_info["issuer"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
         return issuer_info
 
     @typing.overload
@@ -356,44 +345,28 @@
         self, *, binary_form: bool = False
     ) -> bytes | dict[str, typing.Any]:
         x509_certificate = self._quic.get_peercert()
 
         if x509_certificate is None:
             raise ValueError("TLS handshake has not been done yet")
 
-        try:
-            from cryptography import x509
-            from cryptography.hazmat._oid import (
-                AuthorityInformationAccessOID,
-                ExtensionOID,
-            )
-            from cryptography.hazmat.primitives._serialization import Encoding
-        except ImportError as e:
-            raise ValueError(
-                "Unable to generate a dict-form representation due to missing dependencies or sub-module"
-            ) from e
-
         if binary_form:
-            return x509_certificate.public_bytes(Encoding.DER)
+            return x509_certificate.public_bytes()
 
         peer_info = {
-            "version": x509_certificate.version.value + 1,
-            "serialNumber": ("%x" % x509_certificate.serial_number).upper(),
+            "version": x509_certificate.version + 1,
+            "serialNumber": x509_certificate.serial_number.upper(),
             "subject": [],
             "issuer": [],
-            "notBefore": (
-                x509_certificate.not_valid_before
-                if not hasattr(x509_certificate, "not_valid_before_utc")
-                else x509_certificate.not_valid_before_utc
+            "notBefore": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_before, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
-            "notAfter": (
-                x509_certificate.not_valid_after
-                if not hasattr(x509_certificate, "not_valid_after_utc")
-                else x509_certificate.not_valid_after_utc
+            "notAfter": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_after, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
             "subjectAltName": [],
             "OCSP": [],
             "caIssuers": [],
             "crlDistributionPoints": [],
         }
@@ -405,94 +378,68 @@
             "O": "organizationName",
             "OU": "organizationalUnitName",
             "C": "countryName",
             "STREET": "streetAddress",
             "DC": "domainComponent",
         }
 
-        for item in x509_certificate.subject:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.subject:
             peer_info["subject"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for item in x509_certificate.issuer:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.issuer:
             peer_info["issuer"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for ext in x509_certificate.extensions:
-            if isinstance(ext.value, x509.SubjectAlternativeName):
-                for name in ext.value:
-                    if isinstance(name, x509.DNSName):
-                        peer_info["subjectAltName"].append(("DNS", name.value))  # type: ignore[attr-defined]
-                    elif isinstance(name, x509.IPAddress):
-                        peer_info["subjectAltName"].append(  # type: ignore[attr-defined]
-                            ("IP Address", str(name.value))
-                        )
-
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.AUTHORITY_INFORMATION_ACCESS
-            ).value
-            ocsp_locations = [
-                ia for ia in aia if ia.access_method == AuthorityInformationAccessOID.OCSP  # type: ignore[attr-defined]
+        for alt_name in x509_certificate.get_subject_alt_names():
+            decoded_alt_name = alt_name.decode()
+            in_parenthesis = decoded_alt_name[
+                decoded_alt_name.index("(") + 1 : decoded_alt_name.index(")")
             ]
+            if decoded_alt_name.startswith("DNS"):
+                peer_info["subjectAltName"].append(("DNS", in_parenthesis))  # type: ignore[attr-defined]
+            else:
+                from ....resolver.utils import inet4_ntoa, inet6_ntoa
+
+                if len(in_parenthesis) == 11:
+                    ip_address_decoded = inet4_ntoa(
+                        bytes.fromhex(in_parenthesis.replace(":", ""))
+                    )
+                else:
+                    ip_address_decoded = inet6_ntoa(
+                        bytes.fromhex(in_parenthesis.replace(":", ""))
+                    )
+                peer_info["subjectAltName"].append(("IP Address", ip_address_decoded))  # type: ignore[attr-defined]
 
-            peer_info["OCSP"] = [e.access_location.value for e in ocsp_locations]
-        except x509.extensions.ExtensionNotFound:
-            pass
-
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.AUTHORITY_INFORMATION_ACCESS
-            ).value
-            ca_issuers_locations = [
-                ia
-                for ia in aia  # type: ignore[attr-defined]
-                if ia.access_method == AuthorityInformationAccessOID.CA_ISSUERS
-            ]
+        peer_info["OCSP"] = []
 
-            peer_info["caIssuers"] = [
-                e.access_location.value for e in ca_issuers_locations
-            ]
-        except x509.extensions.ExtensionNotFound:
-            pass
+        for endpoint in x509_certificate.get_ocsp_endpoints():
+            decoded_endpoint = endpoint.decode()
 
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.CRL_DISTRIBUTION_POINTS
-            ).value
-
-            peer_info["crlDistributionPoints"] = [
-                ia.full_name[0].value
-                for ia in aia  # type: ignore[attr-defined]
-                if hasattr(ia, "full_name")
-            ]
-        except x509.extensions.ExtensionNotFound:
-            pass
+            peer_info["OCSP"].append(decoded_endpoint[decoded_endpoint.index("(") + 1 : -1])  # type: ignore[attr-defined]
+
+        peer_info["caIssuers"] = []
+
+        for endpoint in x509_certificate.get_issuer_endpoints():
+            decoded_endpoint = endpoint.decode()
+            peer_info["caIssuers"].append(decoded_endpoint[decoded_endpoint.index("(") + 1 : -1])  # type: ignore[attr-defined]
+
+        peer_info["crlDistributionPoints"] = []
 
         pop_keys = []
 
         for k in peer_info:
             if isinstance(peer_info[k], list):
                 peer_info[k] = tuple(peer_info[k])  # type: ignore[arg-type]
                 if not peer_info[k]:
```

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/imcc/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/factories.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/protocols.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/utils.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.904/src/urllib3/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/contrib/ssa/__init__.py` & `urllib3_future-2.7.904/src/urllib3/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/__init__.py` & `urllib3_future-2.7.904/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/connection.py` & `urllib3_future-2.7.904/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/proxy.py` & `urllib3_future-2.7.904/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/request.py` & `urllib3_future-2.7.904/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/response.py` & `urllib3_future-2.7.904/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/retry.py` & `urllib3_future-2.7.904/src/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/ssl_.py` & `urllib3_future-2.7.904/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/ssl_match_hostname.py` & `urllib3_future-2.7.904/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/ssltransport.py` & `urllib3_future-2.7.904/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/timeout.py` & `urllib3_future-2.7.904/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/traffic_police.py` & `urllib3_future-2.7.904/src/urllib3/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/url.py` & `urllib3_future-2.7.904/src/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/util.py` & `urllib3_future-2.7.904/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/wait.py` & `urllib3_future-2.7.904/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/_async/ssl_.py` & `urllib3_future-2.7.904/src/urllib3/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3/util/_async/traffic_police.py` & `urllib3_future-2.7.904/src/urllib3/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_collections.py` & `urllib3_future-2.7.904/src/urllib3_future/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_constant.py` & `urllib3_future-2.7.904/src/urllib3_future/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_request_methods.py` & `urllib3_future-2.7.904/src/urllib3_future/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_typing.py` & `urllib3_future-2.7.904/src/urllib3_future/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/connection.py` & `urllib3_future-2.7.904/src/urllib3_future/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/connectionpool.py` & `urllib3_future-2.7.904/src/urllib3_future/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/exceptions.py` & `urllib3_future-2.7.904/src/urllib3_future/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/fields.py` & `urllib3_future-2.7.904/src/urllib3_future/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/filepost.py` & `urllib3_future-2.7.904/src/urllib3_future/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/poolmanager.py` & `urllib3_future-2.7.904/src/urllib3_future/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/response.py` & `urllib3_future-2.7.904/src/urllib3_future/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_async/connection.py` & `urllib3_future-2.7.904/src/urllib3_future/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_async/connectionpool.py` & `urllib3_future-2.7.904/src/urllib3_future/_async/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_async/poolmanager.py` & `urllib3_future-2.7.904/src/urllib3_future/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/_async/response.py` & `urllib3_future-2.7.904/src/urllib3_future/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/backend/_base.py` & `urllib3_future-2.7.904/src/urllib3_future/backend/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/backend/hface.py` & `urllib3_future-2.7.904/src/urllib3_future/backend/hface.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,17 @@
             # mTLS start
             certfile=cert_file,
             keyfile=key_file,
             keypassword=key_password,
             # mTLS end
             cert_fingerprint=cert_fingerprint,
             cert_use_common_name=cert_use_common_name,
-            verify_hostname=bool(assert_hostname),
+            verify_hostname=assert_hostname
+            if isinstance(assert_hostname, bool)
+            else True,
             assert_hostname=assert_hostname
             if isinstance(assert_hostname, str)
             else None,
         )
 
         self.is_verified = not self.__custom_tls_settings.insecure
```

### Comparing `urllib3_future-2.7.903/src/urllib3_future/backend/_async/_base.py` & `urllib3_future-2.7.904/src/urllib3_future/backend/_async/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/backend/_async/hface.py` & `urllib3_future-2.7.904/src/urllib3_future/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,17 @@
             # mTLS start
             certfile=cert_file,
             keyfile=key_file,
             keypassword=key_password,
             # mTLS end
             cert_fingerprint=cert_fingerprint,
             cert_use_common_name=cert_use_common_name,
-            verify_hostname=bool(assert_hostname),
+            verify_hostname=assert_hostname
+            if isinstance(assert_hostname, bool)
+            else True,
             assert_hostname=assert_hostname
             if isinstance(assert_hostname, str)
             else None,
         )
 
         self.is_verified = not self.__custom_tls_settings.insecure
```

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/_socks_override.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/pyopenssl.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/socks.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_configuration.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_error_codes.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/_typing.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/events/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/events/_events.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,32 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import datetime
 import ssl
 import typing
 from collections import deque
 from os import environ
 from time import time as monotonic
 from typing import Any, Iterable, Sequence
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Literal
 
-import qh3.h3.events as h3_events
-import qh3.quic.events as quic_events
-from qh3.h3.connection import H3Connection, ProtocolError
-from qh3.h3.exceptions import H3Error
-from qh3.quic.configuration import QuicConfiguration
-from qh3.quic.connection import QuicConnection, QuicConnectionError
-from qh3.quic.logger import QuicFileLogger
-from qh3.tls import CipherSuite, SessionTicket
+from qh3 import (
+    CipherSuite,
+    H3Connection,
+    H3Error,
+    ProtocolError,
+    QuicConfiguration,
+    QuicConnection,
+    QuicConnectionError,
+    QuicFileLogger,
+    SessionTicket,
+    h3_events,
+    quic_events,
+)
 
 from ..._configuration import QuicTLSConfig
 from ..._stream_matrix import StreamMatrix
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
 from ...events import HeadersReceived, StreamResetReceived
@@ -63,15 +69,15 @@
             cadata=tls_config.cadata,
             alpn_protocols=["h3"],
             session_ticket=tls_config.session_ticket,
             server_name=server_name,
             hostname_checks_common_name=tls_config.cert_use_common_name,
             assert_fingerprint=tls_config.cert_fingerprint,
             verify_hostname=tls_config.verify_hostname,
-            secrets_log_file=open(keylogfile_path, "w+") if keylogfile_path else None,  # type: ignore[arg-type]
+            secrets_log_file=open(keylogfile_path, "w") if keylogfile_path else None,  # type: ignore[arg-type]
             quic_logger=QuicFileLogger(qlogdir_path) if qlogdir_path else None,
             idle_timeout=300.0,
         )
 
         if tls_config.ciphers:
             available_ciphers = {c.name: c for c in CipherSuite}
             chosen_ciphers: list[CipherSuite] = []
@@ -268,39 +274,32 @@
             raise ValueError("TLS handshake has not been done yet")
 
         if not self._quic.get_issuercerts():
             return None
 
         x509_certificate = self._quic.get_issuercerts()[0]
 
-        try:
-            from cryptography.hazmat.primitives._serialization import Encoding
-        except ImportError as e:
-            raise ValueError(
-                "Unable to generate a dict-form representation due to missing dependencies or sub-module"
-            ) from e
-
         if binary_form:
-            return x509_certificate.public_bytes(Encoding.DER)
+            return x509_certificate.public_bytes()
+
+        datetime.datetime.fromtimestamp(
+            x509_certificate.not_valid_before, tz=datetime.timezone.utc
+        )
 
         issuer_info = {
-            "version": x509_certificate.version.value + 1,
-            "serialNumber": ("%x" % x509_certificate.serial_number).upper(),
+            "version": x509_certificate.version + 1,
+            "serialNumber": x509_certificate.serial_number.upper(),
             "subject": [],
             "issuer": [],
-            "notBefore": (
-                x509_certificate.not_valid_before
-                if not hasattr(x509_certificate, "not_valid_before_utc")
-                else x509_certificate.not_valid_before_utc
+            "notBefore": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_before, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
-            "notAfter": (
-                x509_certificate.not_valid_after
-                if not hasattr(x509_certificate, "not_valid_after_utc")
-                else x509_certificate.not_valid_after_utc
+            "notAfter": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_after, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
         }
 
         _short_name_assoc = {
             "CN": "commonName",
             "L": "localityName",
@@ -308,40 +307,30 @@
             "O": "organizationName",
             "OU": "organizationalUnitName",
             "C": "countryName",
             "STREET": "streetAddress",
             "DC": "domainComponent",
         }
 
-        for item in x509_certificate.subject:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.subject:
             issuer_info["subject"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for item in x509_certificate.issuer:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.issuer:
             issuer_info["issuer"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
         return issuer_info
 
     @typing.overload
@@ -356,44 +345,28 @@
         self, *, binary_form: bool = False
     ) -> bytes | dict[str, typing.Any]:
         x509_certificate = self._quic.get_peercert()
 
         if x509_certificate is None:
             raise ValueError("TLS handshake has not been done yet")
 
-        try:
-            from cryptography import x509
-            from cryptography.hazmat._oid import (
-                AuthorityInformationAccessOID,
-                ExtensionOID,
-            )
-            from cryptography.hazmat.primitives._serialization import Encoding
-        except ImportError as e:
-            raise ValueError(
-                "Unable to generate a dict-form representation due to missing dependencies or sub-module"
-            ) from e
-
         if binary_form:
-            return x509_certificate.public_bytes(Encoding.DER)
+            return x509_certificate.public_bytes()
 
         peer_info = {
-            "version": x509_certificate.version.value + 1,
-            "serialNumber": ("%x" % x509_certificate.serial_number).upper(),
+            "version": x509_certificate.version + 1,
+            "serialNumber": x509_certificate.serial_number.upper(),
             "subject": [],
             "issuer": [],
-            "notBefore": (
-                x509_certificate.not_valid_before
-                if not hasattr(x509_certificate, "not_valid_before_utc")
-                else x509_certificate.not_valid_before_utc
+            "notBefore": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_before, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
-            "notAfter": (
-                x509_certificate.not_valid_after
-                if not hasattr(x509_certificate, "not_valid_after_utc")
-                else x509_certificate.not_valid_after_utc
+            "notAfter": datetime.datetime.fromtimestamp(
+                x509_certificate.not_valid_after, tz=datetime.timezone.utc
             ).strftime("%b %d %H:%M:%S %Y")
             + " UTC",
             "subjectAltName": [],
             "OCSP": [],
             "caIssuers": [],
             "crlDistributionPoints": [],
         }
@@ -405,94 +378,68 @@
             "O": "organizationName",
             "OU": "organizationalUnitName",
             "C": "countryName",
             "STREET": "streetAddress",
             "DC": "domainComponent",
         }
 
-        for item in x509_certificate.subject:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.subject:
             peer_info["subject"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for item in x509_certificate.issuer:
-            name = (
-                item.rfc4514_attribute_name
-                if item.rfc4514_attribute_name not in _short_name_assoc
-                else _short_name_assoc[item.rfc4514_attribute_name]
-            )
+        for raw_oid, rfc4514_attribute_name, value in x509_certificate.issuer:
             peer_info["issuer"].append(  # type: ignore[attr-defined]
                 (
                     (
-                        name,
-                        item.value,
+                        _short_name_assoc[rfc4514_attribute_name],
+                        value.decode(),
                     ),
                 )
             )
 
-        for ext in x509_certificate.extensions:
-            if isinstance(ext.value, x509.SubjectAlternativeName):
-                for name in ext.value:
-                    if isinstance(name, x509.DNSName):
-                        peer_info["subjectAltName"].append(("DNS", name.value))  # type: ignore[attr-defined]
-                    elif isinstance(name, x509.IPAddress):
-                        peer_info["subjectAltName"].append(  # type: ignore[attr-defined]
-                            ("IP Address", str(name.value))
-                        )
-
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.AUTHORITY_INFORMATION_ACCESS
-            ).value
-            ocsp_locations = [
-                ia for ia in aia if ia.access_method == AuthorityInformationAccessOID.OCSP  # type: ignore[attr-defined]
+        for alt_name in x509_certificate.get_subject_alt_names():
+            decoded_alt_name = alt_name.decode()
+            in_parenthesis = decoded_alt_name[
+                decoded_alt_name.index("(") + 1 : decoded_alt_name.index(")")
             ]
+            if decoded_alt_name.startswith("DNS"):
+                peer_info["subjectAltName"].append(("DNS", in_parenthesis))  # type: ignore[attr-defined]
+            else:
+                from ....resolver.utils import inet4_ntoa, inet6_ntoa
+
+                if len(in_parenthesis) == 11:
+                    ip_address_decoded = inet4_ntoa(
+                        bytes.fromhex(in_parenthesis.replace(":", ""))
+                    )
+                else:
+                    ip_address_decoded = inet6_ntoa(
+                        bytes.fromhex(in_parenthesis.replace(":", ""))
+                    )
+                peer_info["subjectAltName"].append(("IP Address", ip_address_decoded))  # type: ignore[attr-defined]
 
-            peer_info["OCSP"] = [e.access_location.value for e in ocsp_locations]
-        except x509.extensions.ExtensionNotFound:
-            pass
-
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.AUTHORITY_INFORMATION_ACCESS
-            ).value
-            ca_issuers_locations = [
-                ia
-                for ia in aia  # type: ignore[attr-defined]
-                if ia.access_method == AuthorityInformationAccessOID.CA_ISSUERS
-            ]
+        peer_info["OCSP"] = []
 
-            peer_info["caIssuers"] = [
-                e.access_location.value for e in ca_issuers_locations
-            ]
-        except x509.extensions.ExtensionNotFound:
-            pass
+        for endpoint in x509_certificate.get_ocsp_endpoints():
+            decoded_endpoint = endpoint.decode()
 
-        try:
-            aia = x509_certificate.extensions.get_extension_for_oid(
-                ExtensionOID.CRL_DISTRIBUTION_POINTS
-            ).value
-
-            peer_info["crlDistributionPoints"] = [
-                ia.full_name[0].value
-                for ia in aia  # type: ignore[attr-defined]
-                if hasattr(ia, "full_name")
-            ]
-        except x509.extensions.ExtensionNotFound:
-            pass
+            peer_info["OCSP"].append(decoded_endpoint[decoded_endpoint.index("(") + 1 : -1])  # type: ignore[attr-defined]
+
+        peer_info["caIssuers"] = []
+
+        for endpoint in x509_certificate.get_issuer_endpoints():
+            decoded_endpoint = endpoint.decode()
+            peer_info["caIssuers"].append(decoded_endpoint[decoded_endpoint.index("(") + 1 : -1])  # type: ignore[attr-defined]
+
+        peer_info["crlDistributionPoints"] = []
 
         pop_keys = []
 
         for k in peer_info:
             if isinstance(peer_info[k], list):
                 peer_info[k] = tuple(peer_info[k])  # type: ignore[arg-type]
                 if not peer_info[k]:
```

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/imcc/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/factories.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/protocols.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/utils.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/contrib/ssa/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/__init__.py` & `urllib3_future-2.7.904/src/urllib3_future/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/connection.py` & `urllib3_future-2.7.904/src/urllib3_future/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/proxy.py` & `urllib3_future-2.7.904/src/urllib3_future/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/request.py` & `urllib3_future-2.7.904/src/urllib3_future/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/response.py` & `urllib3_future-2.7.904/src/urllib3_future/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/retry.py` & `urllib3_future-2.7.904/src/urllib3_future/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/ssl_.py` & `urllib3_future-2.7.904/src/urllib3_future/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/ssl_match_hostname.py` & `urllib3_future-2.7.904/src/urllib3_future/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/ssltransport.py` & `urllib3_future-2.7.904/src/urllib3_future/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/timeout.py` & `urllib3_future-2.7.904/src/urllib3_future/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/traffic_police.py` & `urllib3_future-2.7.904/src/urllib3_future/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/url.py` & `urllib3_future-2.7.904/src/urllib3_future/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/util.py` & `urllib3_future-2.7.904/src/urllib3_future/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/wait.py` & `urllib3_future-2.7.904/src/urllib3_future/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/_async/ssl_.py` & `urllib3_future-2.7.904/src/urllib3_future/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/src/urllib3_future/util/_async/traffic_police.py` & `urllib3_future-2.7.904/src/urllib3_future/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/__init__.py` & `urllib3_future-2.7.904/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/conftest.py` & `urllib3_future-2.7.904/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/port_helpers.py` & `urllib3_future-2.7.904/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_collections.py` & `urllib3_future-2.7.904/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_compatibility.py` & `urllib3_future-2.7.904/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_connection.py` & `urllib3_future-2.7.904/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_connectionpool.py` & `urllib3_future-2.7.904/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_exceptions.py` & `urllib3_future-2.7.904/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_fields.py` & `urllib3_future-2.7.904/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_filepost.py` & `urllib3_future-2.7.904/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_no_ssl.py` & `urllib3_future-2.7.904/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_poolmanager.py` & `urllib3_future-2.7.904/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_proxymanager.py` & `urllib3_future-2.7.904/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_response.py` & `urllib3_future-2.7.904/test/test_response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_retry.py` & `urllib3_future-2.7.904/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_ssl.py` & `urllib3_future-2.7.904/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_ssltransport.py` & `urllib3_future-2.7.904/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_util.py` & `urllib3_future-2.7.904/test/test_util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/test_wait.py` & `urllib3_future-2.7.904/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/tz_stub.py` & `urllib3_future-2.7.904/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/duplicate_san.pem` & `urllib3_future-2.7.904/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/test_resolver.py` & `urllib3_future-2.7.904/test/contrib/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/test_socks.py` & `urllib3_future-2.7.904/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/asynchronous/test_resolver.py` & `urllib3_future-2.7.904/test/contrib/asynchronous/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/asynchronous/test_socks.py` & `urllib3_future-2.7.904/test/contrib/asynchronous/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/contrib/hface/test_stream_matrix.py` & `urllib3_future-2.7.904/test/contrib/hface/test_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_chunked_transfer.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_connection.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_connectionpool.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_happy_eyeballs.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_https.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_https.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_no_ssl.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_poolmanager.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/test_socketlevel.py` & `urllib3_future-2.7.904/test/with_dummyserver/test_socketlevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_connectionpool.py` & `urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_happy_eyeballs.py` & `urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_dummyserver/asynchronous/test_poolmanager.py` & `urllib3_future-2.7.904/test/with_dummyserver/asynchronous/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/__init__.py` & `urllib3_future-2.7.904/test/with_traefik/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_conn_info.py` & `urllib3_future-2.7.904/test/with_traefik/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_connection.py` & `urllib3_future-2.7.904/test/with_traefik/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_connection_multiplexed.py` & `urllib3_future-2.7.904/test/with_traefik/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.904/test/with_traefik/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_protolevel.py` & `urllib3_future-2.7.904/test/with_traefik/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_proxy.py` & `urllib3_future-2.7.904/test/with_traefik/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_send_data.py` & `urllib3_future-2.7.904/test/with_traefik/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_stream.py` & `urllib3_future-2.7.904/test/with_traefik/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/test_svn.py` & `urllib3_future-2.7.904/test/with_traefik/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_conn_info.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connection.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connection_multiplexed.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_protolevel.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_proxy.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_send_data.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_stream.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/test/with_traefik/asynchronous/test_svn.py` & `urllib3_future-2.7.904/test/with_traefik/asynchronous/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/LICENSE.txt` & `urllib3_future-2.7.904/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/README.md` & `urllib3_future-2.7.904/README.md`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/hatch_build.py` & `urllib3_future-2.7.904/hatch_build.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.903/pyproject.toml` & `urllib3_future-2.7.904/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
-  "qh3>=0.14.0,<1.0.0; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version >= '3.8' and python_version < '3.11'))",
+  "qh3>=1.0.3,<2.0.0; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_machine == 'x86_64' or platform_machine == 's390x' or platform_machine == 'aarch64' or platform_machine == 'armv7l' or platform_machine == 'ppc64le' or platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine == 'arm64') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version < '3.11'))",
   "h11>=0.11.0,<1.0.0",
   "h2>=4.0.0,<5.0.0",
 ]
 
 [project.optional-dependencies]
 brotli = [
   "brotli>=1.0.9; platform_python_implementation == 'CPython'",
```

### Comparing `urllib3_future-2.7.903/PKG-INFO` & `urllib3_future-2.7.904/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: urllib3-future
-Version: 2.7.903
+Version: 2.7.904
 Summary: urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async interfaces
 Project-URL: Changelog, https://github.com/jawah/urllib3.future/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3future.readthedocs.io
 Project-URL: Code, https://github.com/jawah/urllib3.future
 Project-URL: Issue tracker, https://github.com/jawah/urllib3.future/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: h11<1.0.0,>=0.11.0
 Requires-Dist: h2<5.0.0,>=4.0.0
-Requires-Dist: qh3<1.0.0,>=0.14.0; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version >= '3.8' and python_version < '3.11'))
+Requires-Dist: qh3<2.0.0,>=1.0.3; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_machine == 'x86_64' or platform_machine == 's390x' or platform_machine == 'aarch64' or platform_machine == 'armv7l' or platform_machine == 'ppc64le' or platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine == 'arm64') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version < '3.11'))
 Provides-Extra: brotli
 Requires-Dist: brotli>=1.0.9; (platform_python_implementation == 'CPython') and extra == 'brotli'
 Requires-Dist: brotlicffi>=0.8.0; (platform_python_implementation != 'CPython') and extra == 'brotli'
 Provides-Extra: qh3
 Requires-Dist: qh3<1.0.0,>=0.14.0; extra == 'qh3'
 Provides-Extra: secure
 Provides-Extra: socks
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.903 Summary:
+Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.904 Summary:
 urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async
 interfaces Project-URL: Changelog, https://github.com/jawah/urllib3.future/
 blob/main/CHANGES.rst Project-URL: Documentation, https://
 urllib3future.readthedocs.io Project-URL: Code, https://github.com/jawah/
 urllib3.future Project-URL: Issue tracker, https://github.com/jawah/
 urllib3.future/issues Author-email: Andrey Petrov
 shazow.net> Maintainer-email: "Ahmed R. TAHRI"
@@ -18,25 +18,28 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.7 Requires-
 Dist: h11<1.0.0,>=0.11.0 Requires-Dist: h2<5.0.0,>=4.0.0 Requires-Dist:
-qh3<1.0.0,>=0.14.0; (platform_system == 'Darwin' or platform_system ==
-'Windows' or platform_system == 'Linux') and (platform_python_implementation ==
-'CPython' or (platform_python_implementation == 'PyPy' and python_version >=
-'3.8' and python_version < '3.11')) Provides-Extra: brotli Requires-Dist:
-brotli>=1.0.9; (platform_python_implementation == 'CPython') and extra ==
-'brotli' Requires-Dist: brotlicffi>=0.8.0; (platform_python_implementation !=
-'CPython') and extra == 'brotli' Provides-Extra: qh3 Requires-Dist:
-qh3<1.0.0,>=0.14.0; extra == 'qh3' Provides-Extra: secure Provides-Extra: socks
-Requires-Dist: python-socks<3.0,>=2.0; extra == 'socks' Provides-Extra: zstd
-Requires-Dist: zstandard>=0.18.0; extra == 'zstd' Description-Content-Type:
-text/markdown
+qh3<2.0.0,>=1.0.3; (platform_system == 'Darwin' or platform_system == 'Windows'
+or platform_system == 'Linux') and (platform_machine == 'x86_64' or
+platform_machine == 's390x' or platform_machine == 'aarch64' or
+platform_machine == 'armv7l' or platform_machine == 'ppc64le' or
+platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine
+== 'arm64') and (platform_python_implementation == 'CPython' or
+(platform_python_implementation == 'PyPy' and python_version < '3.11'))
+Provides-Extra: brotli Requires-Dist: brotli>=1.0.9;
+(platform_python_implementation == 'CPython') and extra == 'brotli' Requires-
+Dist: brotlicffi>=0.8.0; (platform_python_implementation != 'CPython') and
+extra == 'brotli' Provides-Extra: qh3 Requires-Dist: qh3<1.0.0,>=0.14.0; extra
+== 'qh3' Provides-Extra: secure Provides-Extra: socks Requires-Dist: python-
+socks<3.0,>=2.0; extra == 'socks' Provides-Extra: zstd Requires-Dist:
+zstandard>=0.18.0; extra == 'zstd' Description-Content-Type: text/markdown
                       ************ [[uurrlllliibb33..ffuuttuurree llooggoo]] ************
                         _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]
 urllib3.future is as BoringSSL is to OpenSSL but to urllib3 (except support is
                                  available!)
                    â¨ð° Enjoy HTTP like its 2024 ð°â¨
           ð° Promotional offer, get everything and more for 40k 00$!
 â¡ urllib3.future is a powerful, *user-friendly* HTTP client for Python.
```

